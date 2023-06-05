# Comparing `tmp/featurebyte-0.2.2.tar.gz` & `tmp/featurebyte-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebyte-0.2.2.tar", max compression
+gzip compressed data, was "featurebyte-0.3.0.tar", max compression
```

## Comparing `featurebyte-0.2.2.tar` & `featurebyte-0.3.0.tar`

### file list

```diff
@@ -1,519 +1,526 @@
--rw-r--r--   0        0        0     3860 2023-05-10 09:27:03.133494 featurebyte-0.2.2/LICENSE
--rw-r--r--   0        0        0    19763 2023-05-10 09:27:03.133494 featurebyte-0.2.2/README.md
--rw-r--r--   0        0        0    17369 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/__init__.py
--rw-r--r--   0        0        0     2017 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/__main__.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/__init__.py
--rw-r--r--   0        0        0    34410 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/api_object.py
--rw-r--r--   0        0        0     4213 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/api_object_util.py
--rw-r--r--   0        0        0     5101 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/asat_aggregator.py
--rw-r--r--   0        0        0     5521 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/base_aggregator.py
--rw-r--r--   0        0        0    31366 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/base_table.py
--rw-r--r--   0        0        0     2728 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/batch_feature_table.py
--rw-r--r--   0        0        0     3001 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/batch_request_table.py
--rw-r--r--   0        0        0    35630 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/catalog.py
--rw-r--r--   0        0        0     1475 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/catalog_decorator.py
--rw-r--r--   0        0        0    10795 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/catalog_get_by_id_mixin.py
--rw-r--r--   0        0        0    10122 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/change_view.py
--rw-r--r--   0        0        0     6286 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/credential.py
--rw-r--r--   0        0        0     6463 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/data_source.py
--rw-r--r--   0        0        0    11149 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/deployment.py
--rw-r--r--   0        0        0     8452 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/dimension_table.py
--rw-r--r--   0        0        0     3107 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/dimension_view.py
--rw-r--r--   0        0        0    11648 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/entity.py
--rw-r--r--   0        0        0    20619 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/event_table.py
--rw-r--r--   0        0        0    15542 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/event_view.py
--rw-r--r--   0        0        0    42872 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature.py
--rw-r--r--   0        0        0    14818 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_group.py
--rw-r--r--   0        0        0    14837 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_job.py
--rw-r--r--   0        0        0     7302 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    55017 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_list.py
--rw-r--r--   0        0        0     4116 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_namespace.py
--rw-r--r--   0        0        0     9214 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_store.py
--rw-r--r--   0        0        0     1999 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_util.py
--rw-r--r--   0        0        0      557 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_validation_util.py
--rw-r--r--   0        0        0    14478 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/groupby.py
--rw-r--r--   0        0        0     2793 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/historical_feature_table.py
--rw-r--r--   0        0        0    15040 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/item_table.py
--rw-r--r--   0        0        0    11752 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/item_view.py
--rw-r--r--   0        0        0     2619 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/lag.py
--rw-r--r--   0        0        0     4903 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/materialized_table.py
--rw-r--r--   0        0        0     2972 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/observation_table.py
--rw-r--r--   0        0        0      713 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/periodic_task.py
--rw-r--r--   0        0        0     6792 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/relationship.py
--rw-r--r--   0        0        0     3474 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/request_column.py
--rw-r--r--   0        0        0    19938 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/scd_table.py
--rw-r--r--   0        0        0     6023 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/scd_view.py
--rw-r--r--   0        0        0     3119 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/simple_aggregator.py
--rw-r--r--   0        0        0    41315 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/source_table.py
--rw-r--r--   0        0        0     5581 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/table.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/online_serving/__init__.py
--rw-r--r--   0        0        0      707 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/online_serving/python.tpl
--rw-r--r--   0        0        0      132 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/online_serving/shell.tpl
--rw-r--r--   0        0        0    54064 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/view.py
--rw-r--r--   0        0        0     8368 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/window_aggregator.py
--rw-r--r--   0        0        0     1607 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/window_validator.py
--rw-r--r--   0        0        0     6870 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/app.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/__init__.py
--rw-r--r--   0        0        0     3116 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/date_util.py
--rw-r--r--   0        0        0      956 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/descriptor.py
--rw-r--r--   0        0        0      636 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/dict_util.py
--rw-r--r--   0        0        0     2090 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/doc_util.py
--rw-r--r--   0        0        0      630 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/allowed_classes.py
--rw-r--r--   0        0        0    16036 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/autodoc_processor.py
--rw-r--r--   0        0        0     1419 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/constants.py
--rw-r--r--   0        0        0     4280 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/custom_nav.py
--rw-r--r--   0        0        0     8560 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/doc_types.py
--rw-r--r--   0        0        0    40991 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/documentation_layout.py
--rw-r--r--   0        0        0     6909 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/extract_csv.py
--rw-r--r--   0        0        0     3479 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/formatters.py
--rw-r--r--   0        0        0    30799 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
--rw-r--r--   0        0        0      877 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/markdown_extension/extension.py
--rw-r--r--   0        0        0     5660 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/pydantic_field_docs.py
--rw-r--r--   0        0        0    15649 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/resource_extractor.py
--rw-r--r--   0        0        0      519 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/resource_util.py
--rw-r--r--   0        0        0      200 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/util.py
--rw-r--r--   0        0        0     1262 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/env_util.py
--rw-r--r--   0        0        0     3925 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/join_utils.py
--rw-r--r--   0        0        0     4198 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/model_util.py
--rw-r--r--   0        0        0      815 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/path_util.py
--rw-r--r--   0        0        0      451 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/singleton.py
--rw-r--r--   0        0        0     1084 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/tile_util.py
--rw-r--r--   0        0        0     2629 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/typing.py
--rw-r--r--   0        0        0    11086 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/utils.py
--rw-r--r--   0        0        0     3979 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/validator.py
--rw-r--r--   0        0        0    12440 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/config.py
--rw-r--r--   0        0        0     1366 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/conftest.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/__init__.py
--rw-r--r--   0        0        0    15372 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/count_dict.py
--rw-r--r--   0        0        0    23624 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/datetime.py
--rw-r--r--   0        0        0    15884 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/string.py
--rw-r--r--   0        0        0     8902 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/frame.py
--rw-r--r--   0        0        0    11843 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/generic.py
--rw-r--r--   0        0        0    16742 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/mixin.py
--rw-r--r--   0        0        0    38017 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/core/series.py
--rw-r--r--   0        0        0     1257 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/core/timedelta.py
--rw-r--r--   0        0        0     6393 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/core/util.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/__init__.py
--rw-r--r--   0        0        0      697 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/__main__.py
--rw-r--r--   0        0        0     5546 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/app.py
--rw-r--r--   0        0        0     3125 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/creditcard.sql
--rw-r--r--   0        0        0     1154 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/doctest_grocery.sql
--rw-r--r--   0        0        0     2200 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/grocery.sql
--rw-r--r--   0        0        0     5757 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/healthcare.sql
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/docker/__init__.py
--rw-r--r--   0        0        0     4477 2023-05-10 09:27:45.097215 featurebyte-0.2.2/featurebyte/docker/featurebyte.yml
--rw-r--r--   0        0        0     9732 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/docker/manager.py
--rw-r--r--   0        0        0     8578 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/enum.py
--rw-r--r--   0        0        0     8602 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/exception.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/__init__.py
--rw-r--r--   0        0        0    10392 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/manager.py
--rw-r--r--   0        0        0     2911 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/model.py
--rw-r--r--   0        0        0     3997 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/sql_template.py
--rw-r--r--   0        0        0     3693 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/logging.py
--rw-r--r--   0        0        0     9353 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/middleware.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/__init__.py
--rw-r--r--   0        0        0      604 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/migration_data_service.py
--rw-r--r--   0        0        0     1664 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/model.py
--rw-r--r--   0        0        0     8423 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/run.py
--rw-r--r--   0        0        0     1442 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/service/__init__.py
--rw-r--r--   0        0        0     9710 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/service/data_warehouse.py
--rw-r--r--   0        0        0     9181 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/service/mixin.py
--rw-r--r--   0        0        0      646 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/__init__.py
--rw-r--r--   0        0        0    10813 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/base.py
--rw-r--r--   0        0        0      617 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/batch_feature_table.py
--rw-r--r--   0        0        0     1726 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/batch_request_table.py
--rw-r--r--   0        0        0     2377 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/catalog.py
--rw-r--r--   0        0        0     1572 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/context.py
--rw-r--r--   0        0        0     5888 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/credential.py
--rw-r--r--   0        0        0     1333 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/deployment.py
--rw-r--r--   0        0        0     2026 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/dimension_table.py
--rw-r--r--   0        0        0     3618 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/entity.py
--rw-r--r--   0        0        0     3051 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/entity_validation.py
--rw-r--r--   0        0        0     3551 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/event_table.py
--rw-r--r--   0        0        0    12545 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature.py
--rw-r--r--   0        0        0     3750 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    20900 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature_list.py
--rw-r--r--   0        0        0     7606 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature_store.py
--rw-r--r--   0        0        0      644 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/historical_feature_table.py
--rw-r--r--   0        0        0     2919 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/item_table.py
--rw-r--r--   0        0        0     1620 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/materialized_table.py
--rw-r--r--   0        0        0     2113 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/observation_table.py
--rw-r--r--   0        0        0     3738 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/online_store.py
--rw-r--r--   0        0        0     1433 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/parent_serving.py
--rw-r--r--   0        0        0     2891 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/periodic_task.py
--rw-r--r--   0        0        0     1492 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/persistent.py
--rw-r--r--   0        0        0     1024 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/proxy_table.py
--rw-r--r--   0        0        0     4325 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/relationship.py
--rw-r--r--   0        0        0      944 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/relationship_analysis.py
--rw-r--r--   0        0        0     7865 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/request_input.py
--rw-r--r--   0        0        0     3554 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/scd_table.py
--rw-r--r--   0        0        0     1435 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/semantic.py
--rw-r--r--   0        0        0     1085 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/task.py
--rw-r--r--   0        0        0     3269 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/tile.py
--rw-r--r--   0        0        0      154 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/__init__.py
--rw-r--r--   0        0        0     9396 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/audit.py
--rw-r--r--   0        0        0    21712 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/base.py
--rw-r--r--   0        0        0     9772 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/mongo.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/__init__.py
--rw-r--r--   0        0        0     2533 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/algorithm.py
--rw-r--r--   0        0        0     2988 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/enum.py
--rw-r--r--   0        0        0    13774 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/graph.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/graph_node/__init__.py
--rw-r--r--   0        0        0     4592 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/graph_node/base.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/model/__init__.py
--rw-r--r--   0        0        0      873 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/model/column_info.py
--rw-r--r--   0        0        0    12700 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/model/common_table.py
--rw-r--r--   0        0        0     1707 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/critical_data_info.py
--rw-r--r--   0        0        0     5475 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/feature_job_setting.py
--rw-r--r--   0        0        0    19142 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/graph.py
--rw-r--r--   0        0        0    23860 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/table.py
--rw-r--r--   0        0        0     1076 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/__init__.py
--rw-r--r--   0        0        0     5236 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/agg_func.py
--rw-r--r--   0        0        0    24107 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/base.py
--rw-r--r--   0        0        0     5224 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/binary.py
--rw-r--r--   0        0        0    15941 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/cleaning_operation.py
--rw-r--r--   0        0        0     7756 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/count_dict.py
--rw-r--r--   0        0        0     7059 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/date.py
--rw-r--r--   0        0        0    56948 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/generic.py
--rw-r--r--   0        0        0    17015 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/input.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/__init__.py
--rw-r--r--   0        0        0      873 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/column.py
--rw-r--r--   0        0        0    21929 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/operation.py
--rw-r--r--   0        0        0    15033 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/sdk_code.py
--rw-r--r--   0        0        0       47 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
--rw-r--r--   0        0        0     7393 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/mixin.py
--rw-r--r--   0        0        0    21084 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/nested.py
--rw-r--r--   0        0        0     3238 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/request.py
--rw-r--r--   0        0        0     2054 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/scalar.py
--rw-r--r--   0        0        0     5743 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/schema.py
--rw-r--r--   0        0        0     5461 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/string.py
--rw-r--r--   0        0        0     4824 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/unary.py
--rw-r--r--   0        0        0     1042 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/validator.py
--rw-r--r--   0        0        0     1050 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/pruning_util.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/__init__.py
--rw-r--r--   0        0        0    26782 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/adapter.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/__init__.py
--rw-r--r--   0        0        0     6677 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/asat.py
--rw-r--r--   0        0        0    16281 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/base.py
--rw-r--r--   0        0        0     5739 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/item.py
--rw-r--r--   0        0        0     3801 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/latest.py
--rw-r--r--   0        0        0     9549 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/lookup.py
--rw-r--r--   0        0        0     3811 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/request_table.py
--rw-r--r--   0        0        0    26795 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/window.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/__init__.py
--rw-r--r--   0        0        0     5560 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/aggregate.py
--rw-r--r--   0        0        0    12647 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/base.py
--rw-r--r--   0        0        0     2723 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/binary.py
--rw-r--r--   0        0        0     5740 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/count_dict.py
--rw-r--r--   0        0        0    10724 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/datetime.py
--rw-r--r--   0        0        0     7163 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/generic.py
--rw-r--r--   0        0        0     2409 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/groupby.py
--rw-r--r--   0        0        0     2593 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/input.py
--rw-r--r--   0        0        0     1449 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/is_in.py
--rw-r--r--   0        0        0     6208 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join.py
--rw-r--r--   0        0        0     6138 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join_feature.py
--rw-r--r--   0        0        0     2291 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/literal.py
--rw-r--r--   0        0        0      878 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/request.py
--rw-r--r--   0        0        0     8360 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/string.py
--rw-r--r--   0        0        0    11638 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/tile.py
--rw-r--r--   0        0        0     5170 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/track_changes.py
--rw-r--r--   0        0        0     5157 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/unary.py
--rw-r--r--   0        0        0     2536 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/util.py
--rw-r--r--   0        0        0     7070 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/builder.py
--rw-r--r--   0        0        0     4909 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/common.py
--rw-r--r--   0        0        0     1704 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/dataframe.py
--rw-r--r--   0        0        0     1966 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/expression.py
--rw-r--r--   0        0        0    20450 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/feature_compute.py
--rw-r--r--   0        0        0    15450 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/feature_historical.py
--rw-r--r--   0        0        0     3694 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/feature_preview.py
--rw-r--r--   0        0        0     4449 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/groupby_helper.py
--rw-r--r--   0        0        0      426 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/__init__.py
--rw-r--r--   0        0        0     3344 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/base.py
--rw-r--r--   0        0        0    27934 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/preview.py
--rw-r--r--   0        0        0     6685 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/tile.py
--rw-r--r--   0        0        0     4027 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/materialisation.py
--rw-r--r--   0        0        0    17988 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving.py
--rw-r--r--   0        0        0      659 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving_util.py
--rw-r--r--   0        0        0     5042 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/parent_serving.py
--rw-r--r--   0        0        0    15948 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/scd_helper.py
--rw-r--r--   0        0        0    19950 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/specs.py
--rw-r--r--   0        0        0     2206 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/template.py
--rw-r--r--   0        0        0    14905 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/tile_compute.py
--rw-r--r--   0        0        0     3793 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/tile_util.py
--rw-r--r--   0        0        0     9354 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/tiling.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/__init__.py
--rw-r--r--   0        0        0     5184 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/base.py
--rw-r--r--   0        0        0     5201 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/flattening.py
--rw-r--r--   0        0        0     6716 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/operation_structure.py
--rw-r--r--   0        0        0    20327 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/pruning.py
--rw-r--r--   0        0        0    10248 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/reconstruction.py
--rw-r--r--   0        0        0     6264 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/sdk_code.py
--rw-r--r--   0        0        0     5951 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/util.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/__init__.py
--rw-r--r--   0        0        0     4367 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/app_container.py
--rw-r--r--   0        0        0     4340 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/app_container_config.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_feature_table/__init__.py
--rw-r--r--   0        0        0     4832 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_feature_table/api.py
--rw-r--r--   0        0        0     4616 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_request_table/__init__.py
--rw-r--r--   0        0        0     4860 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_request_table/api.py
--rw-r--r--   0        0        0     3137 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_request_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/catalog/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/catalog/api.py
--rw-r--r--   0        0        0     2524 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/catalog/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/__init__.py
--rw-r--r--   0        0        0    10576 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/base.py
--rw-r--r--   0        0        0     3761 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/base_materialized_table.py
--rw-r--r--   0        0        0     5515 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/base_table.py
--rw-r--r--   0        0        0      886 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/schema.py
--rw-r--r--   0        0        0      400 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/util.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/context/__init__.py
--rw-r--r--   0        0        0     3107 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/context/api.py
--rw-r--r--   0        0        0     1596 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/context/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/credential/__init__.py
--rw-r--r--   0        0        0     4605 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/credential/api.py
--rw-r--r--   0        0        0     3071 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/credential/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/deployment/__init__.py
--rw-r--r--   0        0        0     5604 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/deployment/api.py
--rw-r--r--   0        0        0    10416 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/deployment/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/dimension_table/__init__.py
--rw-r--r--   0        0        0     4181 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/dimension_table/api.py
--rw-r--r--   0        0        0     1674 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/dimension_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/entity/__init__.py
--rw-r--r--   0        0        0     5145 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/entity/api.py
--rw-r--r--   0        0        0     2718 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/entity/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/event_table/__init__.py
--rw-r--r--   0        0        0     4689 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/event_table/api.py
--rw-r--r--   0        0        0     1818 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/event_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature/__init__.py
--rw-r--r--   0        0        0     5928 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature/api.py
--rw-r--r--   0        0        0    14144 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/__init__.py
--rw-r--r--   0        0        0     5449 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/api.py
--rw-r--r--   0        0        0     4703 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list/__init__.py
--rw-r--r--   0        0        0     7867 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list/api.py
--rw-r--r--   0        0        0    15191 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/api.py
--rw-r--r--   0        0        0     4891 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_namespace/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_namespace/api.py
--rw-r--r--   0        0        0     7134 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_store/__init__.py
--rw-r--r--   0        0        0     7999 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_store/api.py
--rw-r--r--   0        0        0    12891 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_store/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/historical_feature_table/__init__.py
--rw-r--r--   0        0        0     5367 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/historical_feature_table/api.py
--rw-r--r--   0        0        0     5557 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/historical_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/item_table/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/item_table/api.py
--rw-r--r--   0        0        0     1514 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/item_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/observation_table/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/observation_table/api.py
--rw-r--r--   0        0        0     3157 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/observation_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/periodic_tasks/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/periodic_tasks/api.py
--rw-r--r--   0        0        0      540 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/periodic_tasks/controller.py
--rw-r--r--   0        0        0    16075 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/registry.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/relationship_info/__init__.py
--rw-r--r--   0        0        0     4157 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/relationship_info/api.py
--rw-r--r--   0        0        0     4582 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/relationship_info/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/scd_table/__init__.py
--rw-r--r--   0        0        0     3768 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/scd_table/api.py
--rw-r--r--   0        0        0     1969 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/scd_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/semantic/__init__.py
--rw-r--r--   0        0        0     3733 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/semantic/api.py
--rw-r--r--   0        0        0     1362 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/semantic/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/table/__init__.py
--rw-r--r--   0        0        0     1469 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/table/api.py
--rw-r--r--   0        0        0      464 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/table/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/task/__init__.py
--rw-r--r--   0        0        0     1045 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/task/api.py
--rw-r--r--   0        0        0     1837 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/task/controller.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/temp_data/__init__.py
--rw-r--r--   0        0        0      581 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/temp_data/api.py
--rw-r--r--   0        0        0     1353 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/temp_data/controller.py
--rw-r--r--   0        0        0      180 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/batch_feature_table.py
--rw-r--r--   0        0        0      842 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/batch_request_table.py
--rw-r--r--   0        0        0     1511 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/catalog.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/common/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/common/base.py
--rw-r--r--   0        0        0     3662 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/common/operation.py
--rw-r--r--   0        0        0     1508 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/context.py
--rw-r--r--   0        0        0     3657 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/credential.py
--rw-r--r--   0        0        0     1686 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/deployment.py
--rw-r--r--   0        0        0      981 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/dimension_table.py
--rw-r--r--   0        0        0     1684 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/entity.py
--rw-r--r--   0        0        0     2391 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/event_table.py
--rw-r--r--   0        0        0     5238 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature.py
--rw-r--r--   0        0        0     3383 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     3430 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_list.py
--rw-r--r--   0        0        0     1278 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_list_namespace.py
--rw-r--r--   0        0        0     1965 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_namespace.py
--rw-r--r--   0        0        0     3589 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_store.py
--rw-r--r--   0        0        0     1591 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/historical_feature_table.py
--rw-r--r--   0        0        0    10287 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/info.py
--rw-r--r--   0        0        0      991 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/item_table.py
--rw-r--r--   0        0        0      599 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/materialized_table.py
--rw-r--r--   0        0        0      909 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/observation_table.py
--rw-r--r--   0        0        0      459 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/periodic_task.py
--rw-r--r--   0        0        0     1450 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/relationship_info.py
--rw-r--r--   0        0        0     1190 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/request_table.py
--rw-r--r--   0        0        0     1376 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/scd_table.py
--rw-r--r--   0        0        0      914 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/semantic.py
--rw-r--r--   0        0        0     2415 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/table.py
--rw-r--r--   0        0        0     1012 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/task.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/__init__.py
--rw-r--r--   0        0        0      333 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/progress.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/base.py
--rw-r--r--   0        0        0      610 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0      602 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1382 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     1328 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0      725 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     1215 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0      589 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/observation_table.py
--rw-r--r--   0        0        0      500 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/test.py
--rw-r--r--   0        0        0      416 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/tile.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/service/__init__.py
--rw-r--r--   0        0        0    28027 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/base_document.py
--rw-r--r--   0        0        0      524 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/base_service.py
--rw-r--r--   0        0        0     5195 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/base_table_document.py
--rw-r--r--   0        0        0     1846 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/batch_feature_table.py
--rw-r--r--   0        0        0     2715 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/batch_request_table.py
--rw-r--r--   0        0        0     2303 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/catalog.py
--rw-r--r--   0        0        0     5515 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/context.py
--rw-r--r--   0        0        0     5558 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/credential.py
--rw-r--r--   0        0        0     4782 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/default_version_mode.py
--rw-r--r--   0        0        0    16572 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/deploy.py
--rw-r--r--   0        0        0      478 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/deployment.py
--rw-r--r--   0        0        0      674 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/dimension_table.py
--rw-r--r--   0        0        0     2199 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/entity.py
--rw-r--r--   0        0        0     7515 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/entity_validation.py
--rw-r--r--   0        0        0      618 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/event_table.py
--rw-r--r--   0        0        0     9590 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature.py
--rw-r--r--   0        0        0     3535 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     8863 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_list.py
--rw-r--r--   0        0        0      572 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_list_namespace.py
--rw-r--r--   0        0        0     4048 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_list_status.py
--rw-r--r--   0        0        0      564 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_namespace.py
--rw-r--r--   0        0        0    15409 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_readiness.py
--rw-r--r--   0        0        0      603 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_store.py
--rw-r--r--   0        0        0    11950 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_store_warehouse.py
--rw-r--r--   0        0        0     2939 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/historical_feature_table.py
--rw-r--r--   0        0        0    41009 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/info.py
--rw-r--r--   0        0        0      604 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/item_table.py
--rw-r--r--   0        0        0     4788 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/materialized_table.py
--rw-r--r--   0        0        0     4396 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/mixin.py
--rw-r--r--   0        0        0     6202 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/observation_table.py
--rw-r--r--   0        0        0     9257 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/online_enable.py
--rw-r--r--   0        0        0     4504 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/online_serving.py
--rw-r--r--   0        0        0     7266 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/parent_serving.py
--rw-r--r--   0        0        0      437 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/periodic_task.py
--rw-r--r--   0        0        0    25560 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/preview.py
--rw-r--r--   0        0        0     9285 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/relationship.py
--rw-r--r--   0        0        0     2288 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/relationship_info.py
--rw-r--r--   0        0        0      590 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/scd_table.py
--rw-r--r--   0        0        0      600 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/semantic.py
--rw-r--r--   0        0        0     2703 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/session_manager.py
--rw-r--r--   0        0        0     7932 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/session_validator.py
--rw-r--r--   0        0        0     1051 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/table.py
--rw-r--r--   0        0        0    16758 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/table_columns_info.py
--rw-r--r--   0        0        0     2241 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/table_status.py
--rw-r--r--   0        0        0    10315 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/task_manager.py
--rw-r--r--   0        0        0      779 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/user_service.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/validator/__init__.py
--rw-r--r--   0        0        0     3704 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/validator/materialized_table_delete.py
--rw-r--r--   0        0        0    11567 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/validator/production_ready_validator.py
--rw-r--r--   0        0        0    15770 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/version.py
--rw-r--r--   0        0        0    14878 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/view_construction.py
--rw-r--r--   0        0        0     4180 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/working_schema.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/__init__.py
--rw-r--r--   0        0        0    26285 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/base.py
--rw-r--r--   0        0        0    13141 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/base_spark.py
--rw-r--r--   0        0        0     4211 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/databricks.py
--rw-r--r--   0        0        0      434 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/enum.py
--rw-r--r--   0        0        0     4993 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/hive.py
--rw-r--r--   0        0        0     5107 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/manager.py
--rw-r--r--   0        0        0     4777 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/simple_storage.py
--rw-r--r--   0        0        0    14675 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/snowflake.py
--rw-r--r--   0        0        0     8393 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/spark.py
--rw-r--r--   0        0        0     3479 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/sqlite.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/__init__.py
--rw-r--r--   0        0        0     3198 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/base.py
--rw-r--r--   0        0        0     2743 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/common.py
--rw-r--r--   0        0        0        6 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/databricks/.gitignore
--rw-r--r--   0        0        0      957 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
--rw-r--r--   0        0        0      476 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
--rw-r--r--   0        0        0      171 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
--rw-r--r--   0        0        0      610 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
--rw-r--r--   0        0        0      177 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
--rw-r--r--   0        0        0      188 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
--rw-r--r--   0        0        0     1491 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_GET_RANK.sql
--rw-r--r--   0        0        0      397 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
--rw-r--r--   0        0        0      559 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
--rw-r--r--   0        0        0      559 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
--rw-r--r--   0        0        0      653 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
--rw-r--r--   0        0        0      292 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_ONLINE_STORE_MAPPING.sql
--rw-r--r--   0        0        0      299 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_FEATURE_MAPPING.sql
--rw-r--r--   0        0        0      212 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_JOB_MONITOR.sql
--rw-r--r--   0        0        0      153 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0      526 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql
--rw-r--r--   0        0        0        6 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/.gitignore
--rw-r--r--   0        0        0      304 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_ONLINE_STORE_MAPPING.sql
--rw-r--r--   0        0        0      311 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_FEATURE_MAPPING.sql
--rw-r--r--   0        0        0      228 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_JOB_MONITOR.sql
--rw-r--r--   0        0        0      191 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0      531 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_REGISTRY.sql
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/__init__.py
--rw-r--r--   0        0        0    27440 2023-05-10 09:29:01.548808 featurebyte-0.2.2/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
--rw-r--r--   0        0        0     1922 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_common.py
--rw-r--r--   0        0        0     6290 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_generate.py
--rw-r--r--   0        0        0     3529 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_generate_entity_tracking.py
--rw-r--r--   0        0        0    10092 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_generate_schedule.py
--rw-r--r--   0        0        0     7534 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_monitor.py
--rw-r--r--   0        0        0     3491 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_registry.py
--rw-r--r--   0        0        0     6139 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_schedule_online_store.py
--rw-r--r--   0        0        0      239 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/base.py
--rw-r--r--   0        0        0     3640 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/local.py
--rw-r--r--   0        0        0      415 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/local_temp.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/__init__.py
--rw-r--r--   0        0        0    14758 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/manager.py
--rw-r--r--   0        0        0     2918 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/scheduler.py
--rw-r--r--   0        0        0      411 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/sql_template.py
--rw-r--r--   0        0        0    25685 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/tile_cache.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/credential.py
--rw-r--r--   0        0        0     1532 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/messaging.py
--rw-r--r--   0        0        0      665 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/persistent.py
--rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/snowflake/__init__.py
--rw-r--r--   0        0        0      462 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/snowflake/sql.py
--rw-r--r--   0        0        0      765 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/storage.py
--rw-r--r--   0        0        0     1537 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/__init__.py
--rw-r--r--   0        0        0      170 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/enum.py
--rw-r--r--   0        0        0     3873 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/process_store.py
--rw-r--r--   0        0        0     1159 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/progress.py
--rw-r--r--   0        0        0     2502 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/schedulers.py
--rw-r--r--   0        0        0      107 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/start.py
--rw-r--r--   0        0        0      214 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/base.py
--rw-r--r--   0        0        0     3718 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0     2243 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1795 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     7130 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     3954 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     4321 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0     2572 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/mixin.py
--rw-r--r--   0        0        0     2226 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/observation_table.py
--rw-r--r--   0        0        0      626 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/test_task.py
--rw-r--r--   0        0        0     1904 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/tile_task.py
--rw-r--r--   0        0        0     4155 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task_executor.py
--rw-r--r--   0        0        0     7687 2023-05-10 09:27:43.361220 featurebyte-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    24787 1970-01-01 00:00:00.000000 featurebyte-0.2.2/setup.py
--rw-r--r--   0        0        0    23245 1970-01-01 00:00:00.000000 featurebyte-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-06-05 04:27:45.211716 featurebyte-0.3.0/LICENSE
+-rw-r--r--   0        0        0    19816 2023-06-05 04:27:45.211716 featurebyte-0.3.0/README.md
+-rw-r--r--   0        0        0    14195 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/__init__.py
+-rw-r--r--   0        0        0     2017 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/__init__.py
+-rw-r--r--   0        0        0    30557 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/api_object.py
+-rw-r--r--   0        0        0     3975 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/api_object_util.py
+-rw-r--r--   0        0        0     4985 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/asat_aggregator.py
+-rw-r--r--   0        0        0     5521 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/base_aggregator.py
+-rw-r--r--   0        0        0    37589 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/base_table.py
+-rw-r--r--   0        0        0     4790 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/batch_feature_table.py
+-rw-r--r--   0        0        0     5019 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/batch_request_table.py
+-rw-r--r--   0        0        0    35381 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/catalog.py
+-rw-r--r--   0        0        0     1475 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/catalog_decorator.py
+-rw-r--r--   0        0        0    10842 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/catalog_get_by_id_mixin.py
+-rw-r--r--   0        0        0    11517 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/change_view.py
+-rw-r--r--   0        0        0     6600 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/credential.py
+-rw-r--r--   0        0        0     6540 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/data_source.py
+-rw-r--r--   0        0        0    13660 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/deployment.py
+-rw-r--r--   0        0        0     9699 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/dimension_table.py
+-rw-r--r--   0        0        0     3107 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/dimension_view.py
+-rw-r--r--   0        0        0    12242 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/entity.py
+-rw-r--r--   0        0        0    22561 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/event_table.py
+-rw-r--r--   0        0        0    16044 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/event_view.py
+-rw-r--r--   0        0        0    46149 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature.py
+-rw-r--r--   0        0        0    15414 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_group.py
+-rw-r--r--   0        0        0    15001 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_job.py
+-rw-r--r--   0        0        0     8770 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    62689 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_list.py
+-rw-r--r--   0        0        0     4116 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_namespace.py
+-rw-r--r--   0        0        0    10016 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_store.py
+-rw-r--r--   0        0        0     1999 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_util.py
+-rw-r--r--   0        0        0      557 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_validation_util.py
+-rw-r--r--   0        0        0    18206 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/groupby.py
+-rw-r--r--   0        0        0     4927 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/historical_feature_table.py
+-rw-r--r--   0        0        0    16661 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/item_table.py
+-rw-r--r--   0        0        0    11752 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/item_view.py
+-rw-r--r--   0        0        0     2909 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/lag.py
+-rw-r--r--   0        0        0     4909 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/materialized_table.py
+-rw-r--r--   0        0        0     4952 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/observation_table.py
+-rw-r--r--   0        0        0      721 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/periodic_task.py
+-rw-r--r--   0        0        0     8442 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/relationship.py
+-rw-r--r--   0        0        0     3474 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/request_column.py
+-rw-r--r--   0        0        0     5018 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/savable_api_object.py
+-rw-r--r--   0        0        0    21162 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/scd_table.py
+-rw-r--r--   0        0        0     6023 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/scd_view.py
+-rw-r--r--   0        0        0     3119 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/simple_aggregator.py
+-rw-r--r--   0        0        0    46157 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/source_table.py
+-rw-r--r--   0        0        0     5522 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/table.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/online_serving/__init__.py
+-rw-r--r--   0        0        0      707 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/online_serving/python.tpl
+-rw-r--r--   0        0        0      132 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/online_serving/shell.tpl
+-rw-r--r--   0        0        0    60163 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/view.py
+-rw-r--r--   0        0        0     8368 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/window_aggregator.py
+-rw-r--r--   0        0        0     1607 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/window_validator.py
+-rw-r--r--   0        0        0     6870 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/app.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/__init__.py
+-rw-r--r--   0        0        0     3116 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/date_util.py
+-rw-r--r--   0        0        0      956 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/descriptor.py
+-rw-r--r--   0        0        0      636 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/dict_util.py
+-rw-r--r--   0        0        0     2090 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/doc_util.py
+-rw-r--r--   0        0        0      692 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/allowed_classes.py
+-rw-r--r--   0        0        0    16036 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/autodoc_processor.py
+-rw-r--r--   0        0        0     1419 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/constants.py
+-rw-r--r--   0        0        0     4280 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/custom_nav.py
+-rw-r--r--   0        0        0     8560 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/doc_types.py
+-rw-r--r--   0        0        0    43070 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/documentation_layout.py
+-rw-r--r--   0        0        0     7430 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/extract_csv.py
+-rw-r--r--   0        0        0     3479 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/formatters.py
+-rw-r--r--   0        0        0    31657 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
+-rw-r--r--   0        0        0      877 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/markdown_extension/extension.py
+-rw-r--r--   0        0        0     5660 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/pydantic_field_docs.py
+-rw-r--r--   0        0        0    16371 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/resource_extractor.py
+-rw-r--r--   0        0        0      519 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/resource_util.py
+-rw-r--r--   0        0        0      200 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/util.py
+-rw-r--r--   0        0        0     1262 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/env_util.py
+-rw-r--r--   0        0        0     6740 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/formatting_util.py
+-rw-r--r--   0        0        0     3925 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/join_utils.py
+-rw-r--r--   0        0        0     4198 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/model_util.py
+-rw-r--r--   0        0        0      815 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/path_util.py
+-rw-r--r--   0        0        0     1062 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/progress.py
+-rw-r--r--   0        0        0      451 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/singleton.py
+-rw-r--r--   0        0        0     1084 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/tile_util.py
+-rw-r--r--   0        0        0     2629 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/typing.py
+-rw-r--r--   0        0        0    10491 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/utils.py
+-rw-r--r--   0        0        0     4699 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/validator.py
+-rw-r--r--   0        0        0    12486 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/config.py
+-rw-r--r--   0        0        0     1366 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/__init__.py
+-rw-r--r--   0        0        0    15412 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/count_dict.py
+-rw-r--r--   0        0        0    23735 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/datetime.py
+-rw-r--r--   0        0        0    10051 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/feature_datetime.py
+-rw-r--r--   0        0        0     8454 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/feature_string.py
+-rw-r--r--   0        0        0    15765 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/string.py
+-rw-r--r--   0        0        0     8902 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/frame.py
+-rw-r--r--   0        0        0    11843 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/generic.py
+-rw-r--r--   0        0        0    16742 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/mixin.py
+-rw-r--r--   0        0        0    37956 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/core/series.py
+-rw-r--r--   0        0        0     1484 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/core/timedelta.py
+-rw-r--r--   0        0        0     6393 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/__main__.py
+-rw-r--r--   0        0        0     5546 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/app.py
+-rw-r--r--   0        0        0     3125 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/creditcard.sql
+-rw-r--r--   0        0        0     1154 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/doctest_grocery.sql
+-rw-r--r--   0        0        0     2200 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/grocery.sql
+-rw-r--r--   0        0        0     5757 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/healthcare.sql
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/docker/__init__.py
+-rw-r--r--   0        0        0     4518 2023-06-05 04:28:22.551558 featurebyte-0.3.0/featurebyte/docker/featurebyte.yml
+-rw-r--r--   0        0        0    10343 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/docker/manager.py
+-rw-r--r--   0        0        0     9199 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/enum.py
+-rw-r--r--   0        0        0     9244 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/exception.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/__init__.py
+-rw-r--r--   0        0        0    10392 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/manager.py
+-rw-r--r--   0        0        0     2911 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/model.py
+-rw-r--r--   0        0        0     3997 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/sql_template.py
+-rw-r--r--   0        0        0     3667 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_utility.py
+-rw-r--r--   0        0        0     4145 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/logging.py
+-rw-r--r--   0        0        0     7839 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/migration_data_service.py
+-rw-r--r--   0        0        0     1664 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/model.py
+-rw-r--r--   0        0        0     8423 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/run.py
+-rw-r--r--   0        0        0     1442 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/service/__init__.py
+-rw-r--r--   0        0        0     9762 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/service/data_warehouse.py
+-rw-r--r--   0        0        0     9181 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/service/mixin.py
+-rw-r--r--   0        0        0      646 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/__init__.py
+-rw-r--r--   0        0        0    10813 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/base.py
+-rw-r--r--   0        0        0      617 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/batch_feature_table.py
+-rw-r--r--   0        0        0     1726 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/batch_request_table.py
+-rw-r--r--   0        0        0     2377 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/catalog.py
+-rw-r--r--   0        0        0     1572 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/context.py
+-rw-r--r--   0        0        0     8513 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/credential.py
+-rw-r--r--   0        0        0     1333 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/deployment.py
+-rw-r--r--   0        0        0     2026 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/dimension_table.py
+-rw-r--r--   0        0        0     3618 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/entity.py
+-rw-r--r--   0        0        0     3051 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/entity_validation.py
+-rw-r--r--   0        0        0     3551 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/event_table.py
+-rw-r--r--   0        0        0    11926 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature.py
+-rw-r--r--   0        0        0     3750 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    21070 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature_list.py
+-rw-r--r--   0        0        0     7606 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature_store.py
+-rw-r--r--   0        0        0      644 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/historical_feature_table.py
+-rw-r--r--   0        0        0     2919 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/item_table.py
+-rw-r--r--   0        0        0     1620 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/materialized_table.py
+-rw-r--r--   0        0        0     2113 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/observation_table.py
+-rw-r--r--   0        0        0     3738 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/online_store.py
+-rw-r--r--   0        0        0     1433 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/parent_serving.py
+-rw-r--r--   0        0        0     2891 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/periodic_task.py
+-rw-r--r--   0        0        0     1492 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/persistent.py
+-rw-r--r--   0        0        0     1024 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/proxy_table.py
+-rw-r--r--   0        0        0     4330 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/relationship.py
+-rw-r--r--   0        0        0      944 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/relationship_analysis.py
+-rw-r--r--   0        0        0     7865 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/request_input.py
+-rw-r--r--   0        0        0     3554 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/scd_table.py
+-rw-r--r--   0        0        0     1435 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/semantic.py
+-rw-r--r--   0        0        0     1085 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/task.py
+-rw-r--r--   0        0        0     3269 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/tile.py
+-rw-r--r--   0        0        0      154 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/__init__.py
+-rw-r--r--   0        0        0     9396 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/audit.py
+-rw-r--r--   0        0        0    21712 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/base.py
+-rw-r--r--   0        0        0     9824 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/mongo.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/algorithm.py
+-rw-r--r--   0        0        0     2988 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/enum.py
+-rw-r--r--   0        0        0    16847 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/graph.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/graph_node/__init__.py
+-rw-r--r--   0        0        0     4592 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/graph_node/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/__init__.py
+-rw-r--r--   0        0        0      873 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/column_info.py
+-rw-r--r--   0        0        0    12700 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/common_table.py
+-rw-r--r--   0        0        0     1707 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/critical_data_info.py
+-rw-r--r--   0        0        0     6699 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/feature_job_setting.py
+-rw-r--r--   0        0        0    19282 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/graph.py
+-rw-r--r--   0        0        0    23872 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/table.py
+-rw-r--r--   0        0        0     1076 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/__init__.py
+-rw-r--r--   0        0        0     5236 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/agg_func.py
+-rw-r--r--   0        0        0    28374 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/base.py
+-rw-r--r--   0        0        0     5224 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/binary.py
+-rw-r--r--   0        0        0    17953 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/cleaning_operation.py
+-rw-r--r--   0        0        0     7797 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/count_dict.py
+-rw-r--r--   0        0        0     7293 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/date.py
+-rw-r--r--   0        0        0    60575 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/generic.py
+-rw-r--r--   0        0        0    17049 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/input.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/__init__.py
+-rw-r--r--   0        0        0      873 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/column.py
+-rw-r--r--   0        0        0    21929 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/operation.py
+-rw-r--r--   0        0        0    19397 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/sdk_code.py
+-rw-r--r--   0        0        0       47 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
+-rw-r--r--   0        0        0     7393 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/mixin.py
+-rw-r--r--   0        0        0    21084 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/nested.py
+-rw-r--r--   0        0        0     3272 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/request.py
+-rw-r--r--   0        0        0     2054 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/scalar.py
+-rw-r--r--   0        0        0     6696 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/schema.py
+-rw-r--r--   0        0        0     5461 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/string.py
+-rw-r--r--   0        0        0     4824 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/unary.py
+-rw-r--r--   0        0        0     1042 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/validator.py
+-rw-r--r--   0        0        0     1050 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/pruning_util.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/__init__.py
+-rw-r--r--   0        0        0    27339 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/adapter.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/__init__.py
+-rw-r--r--   0        0        0     7198 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/asat.py
+-rw-r--r--   0        0        0    16281 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/base.py
+-rw-r--r--   0        0        0     5739 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/item.py
+-rw-r--r--   0        0        0     3801 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/latest.py
+-rw-r--r--   0        0        0     9549 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/lookup.py
+-rw-r--r--   0        0        0     3811 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/request_table.py
+-rw-r--r--   0        0        0    26795 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/window.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/__init__.py
+-rw-r--r--   0        0        0     5560 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/aggregate.py
+-rw-r--r--   0        0        0    12647 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/base.py
+-rw-r--r--   0        0        0     2723 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/binary.py
+-rw-r--r--   0        0        0     5740 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/count_dict.py
+-rw-r--r--   0        0        0    10724 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/datetime.py
+-rw-r--r--   0        0        0     7163 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/generic.py
+-rw-r--r--   0        0        0     2409 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/groupby.py
+-rw-r--r--   0        0        0     2593 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/input.py
+-rw-r--r--   0        0        0     1449 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/is_in.py
+-rw-r--r--   0        0        0     6208 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join.py
+-rw-r--r--   0        0        0     6138 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join_feature.py
+-rw-r--r--   0        0        0     2291 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/literal.py
+-rw-r--r--   0        0        0      878 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/request.py
+-rw-r--r--   0        0        0     8360 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/string.py
+-rw-r--r--   0        0        0    11741 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/tile.py
+-rw-r--r--   0        0        0     5170 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/track_changes.py
+-rw-r--r--   0        0        0     5157 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/unary.py
+-rw-r--r--   0        0        0     2536 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/util.py
+-rw-r--r--   0        0        0     7070 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/builder.py
+-rw-r--r--   0        0        0     4909 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/common.py
+-rw-r--r--   0        0        0     1704 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/dataframe.py
+-rw-r--r--   0        0        0     1966 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/expression.py
+-rw-r--r--   0        0        0    20348 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/feature_compute.py
+-rw-r--r--   0        0        0    28059 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/feature_historical.py
+-rw-r--r--   0        0        0     3694 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/feature_preview.py
+-rw-r--r--   0        0        0     4449 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/groupby_helper.py
+-rw-r--r--   0        0        0      426 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/__init__.py
+-rw-r--r--   0        0        0     3344 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/base.py
+-rw-r--r--   0        0        0    27934 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/preview.py
+-rw-r--r--   0        0        0     6685 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/tile.py
+-rw-r--r--   0        0        0     4027 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/materialisation.py
+-rw-r--r--   0        0        0    17988 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving.py
+-rw-r--r--   0        0        0      659 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving_util.py
+-rw-r--r--   0        0        0     5042 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/parent_serving.py
+-rw-r--r--   0        0        0    15948 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/scd_helper.py
+-rw-r--r--   0        0        0    20783 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/specs.py
+-rw-r--r--   0        0        0     2206 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/template.py
+-rw-r--r--   0        0        0    13029 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/tile_compute.py
+-rw-r--r--   0        0        0     3793 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/tile_util.py
+-rw-r--r--   0        0        0     9354 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/tiling.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/__init__.py
+-rw-r--r--   0        0        0     5184 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/base.py
+-rw-r--r--   0        0        0     5201 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/flattening.py
+-rw-r--r--   0        0        0     6716 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/operation_structure.py
+-rw-r--r--   0        0        0    20327 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/pruning.py
+-rw-r--r--   0        0        0    10248 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/reconstruction.py
+-rw-r--r--   0        0        0    13262 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/sdk_code.py
+-rw-r--r--   0        0        0     5951 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/util.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/__init__.py
+-rw-r--r--   0        0        0     4367 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/app_container.py
+-rw-r--r--   0        0        0     4340 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/app_container_config.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_feature_table/__init__.py
+-rw-r--r--   0        0        0     4832 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_feature_table/api.py
+-rw-r--r--   0        0        0     4616 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_request_table/__init__.py
+-rw-r--r--   0        0        0     4860 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_request_table/api.py
+-rw-r--r--   0        0        0     3137 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_request_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/catalog/__init__.py
+-rw-r--r--   0        0        0     4307 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/catalog/api.py
+-rw-r--r--   0        0        0     2524 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/catalog/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/common/__init__.py
+-rw-r--r--   0        0        0    10579 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/base.py
+-rw-r--r--   0        0        0     3761 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/base_materialized_table.py
+-rw-r--r--   0        0        0     5515 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/base_table.py
+-rw-r--r--   0        0        0      886 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/schema.py
+-rw-r--r--   0        0        0      400 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/util.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/context/__init__.py
+-rw-r--r--   0        0        0     3107 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/context/api.py
+-rw-r--r--   0        0        0     1596 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/context/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/credential/__init__.py
+-rw-r--r--   0        0        0     4605 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/credential/api.py
+-rw-r--r--   0        0        0     3071 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/credential/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/deployment/__init__.py
+-rw-r--r--   0        0        0     5604 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/deployment/api.py
+-rw-r--r--   0        0        0    10416 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/deployment/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/dimension_table/__init__.py
+-rw-r--r--   0        0        0     4181 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/dimension_table/api.py
+-rw-r--r--   0        0        0     1674 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/dimension_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/entity/__init__.py
+-rw-r--r--   0        0        0     5145 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/entity/api.py
+-rw-r--r--   0        0        0     2718 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/entity/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/event_table/__init__.py
+-rw-r--r--   0        0        0     4689 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/event_table/api.py
+-rw-r--r--   0        0        0     1818 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/event_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature/__init__.py
+-rw-r--r--   0        0        0     6378 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature/api.py
+-rw-r--r--   0        0        0    15348 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/api.py
+-rw-r--r--   0        0        0     4703 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list/__init__.py
+-rw-r--r--   0        0        0     7085 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list/api.py
+-rw-r--r--   0        0        0    13578 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/__init__.py
+-rw-r--r--   0        0        0     4324 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/api.py
+-rw-r--r--   0        0        0     6989 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_namespace/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_namespace/api.py
+-rw-r--r--   0        0        0     7126 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_store/__init__.py
+-rw-r--r--   0        0        0     7999 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_store/api.py
+-rw-r--r--   0        0        0    12891 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_store/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/historical_feature_table/__init__.py
+-rw-r--r--   0        0        0     5367 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/historical_feature_table/api.py
+-rw-r--r--   0        0        0     5557 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/historical_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/item_table/__init__.py
+-rw-r--r--   0        0        0     3832 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/item_table/api.py
+-rw-r--r--   0        0        0     1514 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/item_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/observation_table/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/observation_table/api.py
+-rw-r--r--   0        0        0     3157 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/observation_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/periodic_tasks/__init__.py
+-rw-r--r--   0        0        0     1583 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/periodic_tasks/api.py
+-rw-r--r--   0        0        0      540 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/periodic_tasks/controller.py
+-rw-r--r--   0        0        0    16128 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/registry.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/relationship_info/__init__.py
+-rw-r--r--   0        0        0     4202 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/relationship_info/api.py
+-rw-r--r--   0        0        0     4602 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/relationship_info/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/scd_table/__init__.py
+-rw-r--r--   0        0        0     3768 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/scd_table/api.py
+-rw-r--r--   0        0        0     1969 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/scd_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/semantic/__init__.py
+-rw-r--r--   0        0        0     3733 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/semantic/api.py
+-rw-r--r--   0        0        0     1362 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/semantic/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/table/__init__.py
+-rw-r--r--   0        0        0     1469 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/table/api.py
+-rw-r--r--   0        0        0      464 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/task/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/task/api.py
+-rw-r--r--   0        0        0     1837 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/task/controller.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/temp_data/__init__.py
+-rw-r--r--   0        0        0      581 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/temp_data/api.py
+-rw-r--r--   0        0        0     1353 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/temp_data/controller.py
+-rw-r--r--   0        0        0      180 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/batch_feature_table.py
+-rw-r--r--   0        0        0      842 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/batch_request_table.py
+-rw-r--r--   0        0        0     1511 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/catalog.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/common/__init__.py
+-rw-r--r--   0        0        0     1068 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/common/base.py
+-rw-r--r--   0        0        0     3662 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/common/operation.py
+-rw-r--r--   0        0        0     1508 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/context.py
+-rw-r--r--   0        0        0     3658 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/credential.py
+-rw-r--r--   0        0        0     1686 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/deployment.py
+-rw-r--r--   0        0        0      981 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/dimension_table.py
+-rw-r--r--   0        0        0     1684 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/entity.py
+-rw-r--r--   0        0        0     2391 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/event_table.py
+-rw-r--r--   0        0        0     7337 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature.py
+-rw-r--r--   0        0        0     4664 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     3758 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_list.py
+-rw-r--r--   0        0        0     1460 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_list_namespace.py
+-rw-r--r--   0        0        0     1965 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_namespace.py
+-rw-r--r--   0        0        0     3589 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_store.py
+-rw-r--r--   0        0        0     1591 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/historical_feature_table.py
+-rw-r--r--   0        0        0    10583 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/info.py
+-rw-r--r--   0        0        0      991 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/item_table.py
+-rw-r--r--   0        0        0      599 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/materialized_table.py
+-rw-r--r--   0        0        0      909 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/observation_table.py
+-rw-r--r--   0        0        0      459 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/periodic_task.py
+-rw-r--r--   0        0        0     1460 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/relationship_info.py
+-rw-r--r--   0        0        0     1190 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/request_table.py
+-rw-r--r--   0        0        0     1376 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/scd_table.py
+-rw-r--r--   0        0        0      914 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/semantic.py
+-rw-r--r--   0        0        0     2415 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/table.py
+-rw-r--r--   0        0        0     1012 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/task.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/progress.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/__init__.py
+-rw-r--r--   0        0        0     2829 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/base.py
+-rw-r--r--   0        0        0      520 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_create.py
+-rw-r--r--   0        0        0      610 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0      602 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1382 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     1328 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0      725 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     1215 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0      589 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/observation_table.py
+-rw-r--r--   0        0        0      500 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/test.py
+-rw-r--r--   0        0        0      416 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/tile.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/__init__.py
+-rw-r--r--   0        0        0    28027 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/base_document.py
+-rw-r--r--   0        0        0      524 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/base_service.py
+-rw-r--r--   0        0        0     5195 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/base_table_document.py
+-rw-r--r--   0        0        0     1846 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/batch_feature_table.py
+-rw-r--r--   0        0        0     2715 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/batch_request_table.py
+-rw-r--r--   0        0        0     2303 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/catalog.py
+-rw-r--r--   0        0        0     5515 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/context.py
+-rw-r--r--   0        0        0     5558 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/credential.py
+-rw-r--r--   0        0        0     4782 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/default_version_mode.py
+-rw-r--r--   0        0        0    18158 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/deploy.py
+-rw-r--r--   0        0        0      478 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/deployment.py
+-rw-r--r--   0        0        0      674 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/dimension_table.py
+-rw-r--r--   0        0        0     2199 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/entity.py
+-rw-r--r--   0        0        0     7515 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/entity_validation.py
+-rw-r--r--   0        0        0      618 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/event_table.py
+-rw-r--r--   0        0        0    11435 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature.py
+-rw-r--r--   0        0        0     3535 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    10881 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_list.py
+-rw-r--r--   0        0        0      572 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_list_namespace.py
+-rw-r--r--   0        0        0     4048 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_list_status.py
+-rw-r--r--   0        0        0      564 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_namespace.py
+-rw-r--r--   0        0        0    15409 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_readiness.py
+-rw-r--r--   0        0        0      603 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_store.py
+-rw-r--r--   0        0        0    15423 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_store_warehouse.py
+-rw-r--r--   0        0        0     2939 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/historical_feature_table.py
+-rw-r--r--   0        0        0    42750 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/info.py
+-rw-r--r--   0        0        0      604 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/item_table.py
+-rw-r--r--   0        0        0     4788 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/materialized_table.py
+-rw-r--r--   0        0        0     4396 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/mixin.py
+-rw-r--r--   0        0        0     6202 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/observation_table.py
+-rw-r--r--   0        0        0     9257 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/online_enable.py
+-rw-r--r--   0        0        0     4504 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/online_serving.py
+-rw-r--r--   0        0        0     7266 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/parent_serving.py
+-rw-r--r--   0        0        0      437 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/periodic_task.py
+-rw-r--r--   0        0        0    25370 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/preview.py
+-rw-r--r--   0        0        0     9285 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/relationship.py
+-rw-r--r--   0        0        0     2303 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/relationship_info.py
+-rw-r--r--   0        0        0      590 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/scd_table.py
+-rw-r--r--   0        0        0      600 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/semantic.py
+-rw-r--r--   0        0        0     2703 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/session_manager.py
+-rw-r--r--   0        0        0     7932 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/session_validator.py
+-rw-r--r--   0        0        0     1051 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/table.py
+-rw-r--r--   0        0        0    16758 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/table_columns_info.py
+-rw-r--r--   0        0        0     2241 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/table_status.py
+-rw-r--r--   0        0        0    10862 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/task_manager.py
+-rw-r--r--   0        0        0      779 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/user_service.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/validator/__init__.py
+-rw-r--r--   0        0        0     3704 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/validator/materialized_table_delete.py
+-rw-r--r--   0        0        0    11567 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/validator/production_ready_validator.py
+-rw-r--r--   0        0        0    15798 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/version.py
+-rw-r--r--   0        0        0    14878 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/service/view_construction.py
+-rw-r--r--   0        0        0     4180 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/service/working_schema.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/__init__.py
+-rw-r--r--   0        0        0    26478 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/base.py
+-rw-r--r--   0        0        0    14634 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/base_spark.py
+-rw-r--r--   0        0        0     5643 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/databricks.py
+-rw-r--r--   0        0        0      434 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/enum.py
+-rw-r--r--   0        0        0     4993 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/hive.py
+-rw-r--r--   0        0        0     5107 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/manager.py
+-rw-r--r--   0        0        0     7592 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/simple_storage.py
+-rw-r--r--   0        0        0    14756 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/snowflake.py
+-rw-r--r--   0        0        0     8393 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/spark.py
+-rw-r--r--   0        0        0     3479 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/sqlite.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/__init__.py
+-rw-r--r--   0        0        0     3198 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/base.py
+-rw-r--r--   0        0        0     2743 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/common.py
+-rw-r--r--   0        0        0        6 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/databricks/.gitignore
+-rw-r--r--   0        0        0      957 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
+-rw-r--r--   0        0        0      476 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
+-rw-r--r--   0        0        0      171 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
+-rw-r--r--   0        0        0      610 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
+-rw-r--r--   0        0        0      177 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
+-rw-r--r--   0        0        0      188 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
+-rw-r--r--   0        0        0     1491 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_GET_RANK.sql
+-rw-r--r--   0        0        0      397 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
+-rw-r--r--   0        0        0      559 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
+-rw-r--r--   0        0        0      559 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
+-rw-r--r--   0        0        0      653 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
+-rw-r--r--   0        0        0      292 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_ONLINE_STORE_MAPPING.sql
+-rw-r--r--   0        0        0      299 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_FEATURE_MAPPING.sql
+-rw-r--r--   0        0        0      212 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_JOB_MONITOR.sql
+-rw-r--r--   0        0        0      153 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0      526 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql
+-rw-r--r--   0        0        0        6 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/.gitignore
+-rw-r--r--   0        0        0      304 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_ONLINE_STORE_MAPPING.sql
+-rw-r--r--   0        0        0      311 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_FEATURE_MAPPING.sql
+-rw-r--r--   0        0        0      228 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_JOB_MONITOR.sql
+-rw-r--r--   0        0        0      191 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0      531 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_REGISTRY.sql
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/__init__.py
+-rw-r--r--   0        0        0    29690 2023-06-05 04:29:41.147176 featurebyte-0.3.0/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
+-rw-r--r--   0        0        0     2001 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_common.py
+-rw-r--r--   0        0        0     5878 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_generate.py
+-rw-r--r--   0        0        0     3566 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_generate_entity_tracking.py
+-rw-r--r--   0        0        0     9817 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_generate_schedule.py
+-rw-r--r--   0        0        0     7297 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_monitor.py
+-rw-r--r--   0        0        0     3491 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_registry.py
+-rw-r--r--   0        0        0     6139 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_schedule_online_store.py
+-rw-r--r--   0        0        0      239 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/__init__.py
+-rw-r--r--   0        0        0     4999 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/base.py
+-rw-r--r--   0        0        0     3640 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/local.py
+-rw-r--r--   0        0        0      415 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/local_temp.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/__init__.py
+-rw-r--r--   0        0        0    14347 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/manager.py
+-rw-r--r--   0        0        0     2918 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/scheduler.py
+-rw-r--r--   0        0        0      411 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/sql_template.py
+-rw-r--r--   0        0        0    28505 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/tile_cache.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/__init__.py
+-rw-r--r--   0        0        0     1909 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/credential.py
+-rw-r--r--   0        0        0     1532 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/messaging.py
+-rw-r--r--   0        0        0      534 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/persistent.py
+-rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/snowflake/__init__.py
+-rw-r--r--   0        0        0      462 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/snowflake/sql.py
+-rw-r--r--   0        0        0      765 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/storage.py
+-rw-r--r--   0        0        0     1537 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/enum.py
+-rw-r--r--   0        0        0     3873 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/process_store.py
+-rw-r--r--   0        0        0     1159 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/progress.py
+-rw-r--r--   0        0        0     2502 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/schedulers.py
+-rw-r--r--   0        0        0      107 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/start.py
+-rw-r--r--   0        0        0      214 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/base.py
+-rw-r--r--   0        0        0     4603 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/batch_feature_create.py
+-rw-r--r--   0        0        0     3718 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0     2243 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1795 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     7130 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     3954 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     4321 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0     2604 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/mixin.py
+-rw-r--r--   0        0        0     2226 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/observation_table.py
+-rw-r--r--   0        0        0      626 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/test_task.py
+-rw-r--r--   0        0        0     1904 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/tile_task.py
+-rw-r--r--   0        0        0     5407 2023-06-05 04:27:45.251716 featurebyte-0.3.0/featurebyte/worker/task_executor.py
+-rw-r--r--   0        0        0     7717 2023-06-05 04:28:21.203564 featurebyte-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    23050 1970-01-01 00:00:00.000000 featurebyte-0.3.0/PKG-INFO
```

### Comparing `featurebyte-0.2.2/LICENSE` & `featurebyte-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/README.md` & `featurebyte-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,24 @@
 
 ### Create
 - Create and share state-of-the-art ML features effortlessly
 - Search and reuse features to create feature lists tailored to your use case
 
 ``` python
 # Get view from catalog
-invoices = catalog.get_view("INVOICES")
-# Customer average spend over past 5 weeks
-features = invoices.groupby(
-    "CustomerId"
-).aggregate_over(
+invoice_view = catalog.get_view("GROCERYINVOICE")
+# Declare features of total spent by customer in the past 7 and 28 days
+customer_purchases = invoice_view.groupby("GroceryCustomerGuid").aggregate_over(
     "Amount",
-    method="avg",
-    feature_names=["AvgSpend5w"],
+    method="sum",
+    feature_names=["CustomerTotalSpent_7d", "CustomerTotalSpent_28d"],
     fill_value=0,
-    windows=["5w"]
+    windows=['7d', '28d']
 )
-# Save feature
-features["AvgSpend5w"].save()
+customer_purchases.save()
 ```
 
 ### Experiment
 - Immediately access historical features through automated backfilling - let FeatureByte handle the complexity of time-aware SQL
 - Experiment on live data at scale, innovating faster
 - Iterate rapidly with different feature lists to create more accurate models
 
@@ -231,41 +228,41 @@
 
 ``` python
 # Get items and product view from the catalog
 items_view = catalog.get_view("INVOICEITEMS")
 product_view = catalog.get_view("GROCERYPRODUCT")
 # Join product view to items view
 items_view = items_view.join(product_view)
-# Get Customer purchases across product group over the past 4 weeks
-customer_inventory_28d = items_view.groupby(
+# Get Customer purchases across product group in the past 4 weeks
+customer_basket_28d = items_view.groupby(
     by_keys = "GroceryCustomerGuid", category=”ProductGroup”
 ).aggregate_over(
    "TotalCost",
     method=fb.AggFunc.SUM,
-    feature_names=["CustomerInventory_28d"],
+    feature_names=["CustomerBasket_28d"],
     windows=['28d']
 )
 # Get customer view and join it to items view
 customer_view = catalog.get_view("GROCERYCUSTOMER")
 items_view = items_view.join(customer_view)
 # Get Purchases of Customers living in the same state
-# across product group over the past 4 weeks
-state_inventory_28d = items_view.groupby(
+# across product group in the past 4 weeks
+state_basket_28d = items_view.groupby(
     by_keys="State", category="ProductGroup"
 ).aggregate_over(
    "TotalCost",
     method=fb.AggFunc.SUM,
-    feature_names=["StateInventory_28d"],
+    feature_names=["StateBasket_28d"],
     windows=['28d']
 )
 # Create a feature that measures the similarity of a customer purchases
 # and purchases of customers living in the same state
 customer_state_similarity_28d = \
-    customer_inventory_28d["CustomerInventory_28d"].cd.cosine_similarity(
-        state_inventory_28d["StateInventory_28d"]
+    customer_basket_28d["CustomerBasket_28d"].cd.cosine_similarity(
+        state_basket_28d["StateBasket_28d"]
     )
 # save the new feature
 customer_state_similarity_28d.name = \
     "Customer Similarity with purchases in the same state over 28 days"
 customer_state_similarity_28d.save()
 ```
```

### Comparing `featurebyte-0.2.2/featurebyte/__init__.py` & `featurebyte-0.3.0/featurebyte/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Python Library for FeatureOps"""
 from typing import Any, List, Optional
 
-import inspect
 import sys
 from http import HTTPStatus
 
 import pandas as pd
 
 from featurebyte.api.batch_feature_table import BatchFeatureTable
 from featurebyte.api.batch_request_table import BatchRequestTable
@@ -47,17 +46,20 @@
 from featurebyte.docker.manager import stop_app as _stop_app
 from featurebyte.enum import AggFunc, SourceType, StorageType
 from featurebyte.exception import (
     FeatureByteException,
     InvalidSettingsError,
     RecordRetrievalException,
 )
+from featurebyte.feature_utility import list_unsaved_features
 from featurebyte.logging import get_logger
 from featurebyte.models.credential import (
     AccessTokenCredential,
+    AzureBlobStorageCredential,
+    GCSStorageCredential,
     S3StorageCredential,
     UsernamePasswordCredential,
 )
 from featurebyte.models.feature import DefaultVersionMode
 from featurebyte.models.feature_list import FeatureListStatus
 from featurebyte.models.feature_store import TableStatus
 from featurebyte.query_graph.model.feature_job_setting import (
@@ -361,105 +363,14 @@
         columns=["_id"] + columns,
     ).rename(columns={"_id": "id"})
     if include_id:
         return output_df
     return output_df.drop(columns=["id"])
 
 
-def list_unsaved_features() -> pd.DataFrame:
-    """
-    List all unsaved features in the current session.
-
-    Returns
-    -------
-    pd.DataFrame
-        List of unsaved features
-
-    Examples
-    --------
-    >>> customer_gender = catalog.get_view("GROCERYCUSTOMER")["Gender"].as_feature(
-    ...     feature_name="Customer Gender"
-    ... )
-    >>> fb.list_unsaved_features()[["variable_name", "name", "catalog", "active_catalog"]]
-         variable_name             name  catalog  active_catalog
-    0  customer_gender  Customer Gender  grocery            True
-    """
-    processed_variables = set()
-    unsaved_features = []
-    client = Configurations().get_client()
-
-    def _is_saved(feature: Feature) -> bool:
-        """
-        Check if a feature is saved.
-
-        Parameters
-        ----------
-        feature: Feature
-            Feature to check
-
-        Returns
-        -------
-        bool
-        """
-        response = client.get(
-            url=f"/feature/{feature.id}", headers={"active-catalog-id": str(feature.catalog_id)}
-        )
-        if response.status_code == HTTPStatus.OK:
-            return True
-        return False
-
-    # get list of frame info from the current call stack
-    call_stack = inspect.stack()
-    # skip the first frame, which is the current function, to get the caller's frame
-    caller_frame_info = call_stack[1]
-    # check caller's local variables first, then global variables for unsaved features
-    caller_variables = [caller_frame_info.frame.f_locals, caller_frame_info.frame.f_globals]
-    for variables in caller_variables:
-        for var_name, var_obj in variables.items():
-            # global variable may be overriden by local variable
-            if var_name in processed_variables:
-                continue
-            if isinstance(var_obj, Feature) and not _is_saved(var_obj):
-                unsaved_features.append(
-                    {
-                        "object_id": str(var_obj.id),
-                        "variable_name": var_name,
-                        "name": var_obj.name,
-                        "catalog_id": var_obj.catalog_id,
-                    }
-                )
-            elif isinstance(var_obj, BaseFeatureGroup):
-                for name, feature in var_obj.feature_objects.items():
-                    if not _is_saved(feature):
-                        unsaved_features.append(
-                            {
-                                "object_id": str(feature.id),
-                                "variable_name": f'{var_name}["{name}"]',
-                                "name": feature.name,
-                                "catalog_id": feature.catalog_id,
-                            }
-                        )
-            processed_variables.add(var_name)
-
-    if unsaved_features:
-        catalogs = Catalog.list(include_id=True)
-        return (
-            pd.DataFrame(unsaved_features)
-            .merge(
-                catalogs.rename({"name": "catalog", "active": "active_catalog"}, axis=1),
-                left_on="catalog_id",
-                right_on="id",
-                how="left",
-            )[["object_id", "variable_name", "name", "catalog", "active_catalog"]]
-            .sort_values("object_id")
-            .reset_index(drop=True)
-        )
-    return pd.DataFrame(columns=["object_id", "variable_name", "name", "catalog", "active_catalog"])
-
-
 __all__ = [
     # API objects
     "BatchFeatureTable",
     "BatchRequestTable",
     "Catalog",
     "ChangeView",
     "DatabricksDetails",
@@ -487,16 +398,18 @@
     "SourceTable",
     "SnowflakeDetails",
     "SparkDetails",
     "to_timedelta",
     "Table",
     "TableFeatureJobSetting",
     # credentials
+    "AzureBlobStorageCredential",
     "AccessTokenCredential",
     "Credential",
+    "GCSStorageCredential",
     "S3StorageCredential",
     "UsernamePasswordCredential",
     # enums
     "AggFunc",
     "FeatureListStatus",
     "SourceType",
     "StorageType",
@@ -514,14 +427,16 @@
     "ColumnCleaningOperation",
     "TableCleaningOperation",
     "PeriodicTask",
     # services
     "start",
     "stop",
     "playground",
+    # utility
+    "list_unsaved_features",
 ]
 
 
 def log_env_summary() -> None:
     """
     Print environment summary.
```

### Comparing `featurebyte-0.2.2/featurebyte/__main__.py` & `featurebyte-0.3.0/featurebyte/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/api_object.py` & `featurebyte-0.3.0/featurebyte/api/api_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,23 +17,22 @@
 from bson.objectid import ObjectId
 from cachetools import TTLCache, cachedmethod
 from cachetools.keys import hashkey
 from pandas import DataFrame
 from requests.models import Response
 from typeguard import typechecked
 
-from featurebyte.api.api_object_util import PrettyDict, ProgressThread
+from featurebyte.api.api_object_util import ProgressThread
 from featurebyte.common.env_util import get_alive_bar_additional_params
+from featurebyte.common.formatting_util import InfoDict
 from featurebyte.common.utils import construct_repr_string
 from featurebyte.config import Configurations
 from featurebyte.exception import (
     DuplicatedRecordException,
-    ObjectHasBeenSavedError,
     RecordCreationException,
-    RecordDeletionException,
     RecordRetrievalException,
     RecordUpdateException,
 )
 from featurebyte.logging import get_logger
 from featurebyte.models.base import FeatureByteBaseDocumentModel, FeatureByteBaseModel
 from featurebyte.schema.task import TaskStatus
 
@@ -110,21 +109,34 @@
     _get_schema = FeatureByteBaseDocumentModel
     _list_fields = ["name", "created_at"]
     _list_foreign_keys: List[ForeignKeyMapping] = []
 
     # global api object cache shared by all the ApiObject class & its child classes
     _cache: Any = TTLCache(maxsize=1024, ttl=1)
 
+    def _repr_html_(self) -> str:
+        """
+        HTML representation of the object
+
+        Returns
+        -------
+        str
+        """
+        try:
+            return InfoDict(self.info()).to_html()
+        except (RecordCreationException, RecordRetrievalException):
+            # object has not been saved yet
+            return repr(self)
+
     def __repr__(self) -> str:
-        info_repr = ""
         try:
             info_repr = repr(self.info())
         except (RecordCreationException, RecordRetrievalException):
             # object has not been saved yet
-            pass
+            info_repr = super().__repr__()
 
         return construct_repr_string(self, info_repr)
 
     @property  # type: ignore
     @cachedmethod(cache=operator.attrgetter("_cache"), key=get_api_object_cache_key)
     def cached_model(self: ModelT) -> ModelT:
         """
@@ -716,15 +728,17 @@
         ------
         RecordRetrievalException
             When the object cannot be found, or we have received an unexpected response status code.
         """
         client = Configurations().get_client()
         response = client.get(url=f"{self._route}/{self.id}/info", params={"verbose": verbose})
         if response.status_code == HTTPStatus.OK:
-            return PrettyDict(response.json())
+            info = response.json()
+            info["class_name"] = self.__class__.__name__
+            return InfoDict(info)
         raise RecordRetrievalException(response, "Failed to retrieve object info.")
 
     @classmethod
     def _poll_async_task(
         cls,
         task_response: Response,
         delay: float = POLLING_INTERVAL,
@@ -865,121 +879,7 @@
         update_response = client.patch(url=route, json=payload)
         if update_response.status_code != HTTPStatus.OK:
             raise RecordUpdateException(response=update_response)
         if update_response.json():
             self._poll_async_task(task_response=update_response, delay=delay, retrieve_result=False)
         # call get to update the object cache as retrieve result is False
         self.get_by_id(self.id)
-
-
-class SavableApiObject(ApiObject):
-    """
-    ApiObject contains common methods used to interact with API routes
-    """
-
-    def _get_create_payload(self) -> dict[str, Any]:
-        """
-        Construct payload used for post route
-
-        Returns
-        -------
-        dict[str, Any]
-        """
-        return self.json_dict(exclude_none=True)
-
-    def _pre_save_operations(self, conflict_resolution: ConflictResolution) -> None:
-        """
-        Operations to be executed before saving the api object
-
-        Parameters
-        ----------
-        conflict_resolution: ConflictResolution
-            "raise" raises error when then counters conflict error (default)
-            "retrieve" handle conflict error by retrieving object with the same name
-        """
-        _ = conflict_resolution
-
-    @typechecked
-    def save(self, conflict_resolution: ConflictResolution = "raise") -> None:
-        """
-        Save an object to the persistent data store.
-
-        A conflict could be triggered when the object being saved has violated a uniqueness check at the persistent
-        data store. For example, the same object ID could have been used by another record that is already stored.
-
-        In these scenarios, we can either raise an error or retrieve the object with the same name, depending on the
-        conflict resolution parameter passed in. The default behavior is to raise an error.
-
-        Parameters
-        ----------
-        conflict_resolution: ConflictResolution
-            "raise" will raise an error when we encounter a conflict error.
-            "retrieve" will handle the conflict error by retrieving the object with the same name.
-
-        Raises
-        ------
-        ObjectHasBeenSavedError
-            If the object has been saved before.
-        DuplicatedRecordException
-            When a record with the same key exists at the persistent data store.
-        RecordCreationException
-            When we fail to save the new object (general failure).
-
-        Examples
-        --------
-        Note that the examples below are not exhaustive.
-
-        Save a new Entity object.
-
-        >>> entity = fb.Entity(name="grocerycustomer_example", serving_names=["GROCERYCUSTOMERGUID"])  # doctest: +SKIP
-        >>> entity.save()  # doctest: +SKIP
-        None
-
-        Calling save again returns an error.
-
-        >>> entity = fb.Entity(name="grocerycustomer", serving_names=["GROCERYCUSTOMERGUID"])  # doctest: +SKIP
-        >>> entity.save()  # doctest: +SKIP
-        >>> entity.save()  # doctest: +SKIP
-        Entity (id: <entity.id>) has been saved before.
-        """
-        if self.saved and conflict_resolution == "raise":
-            raise ObjectHasBeenSavedError(
-                f'{type(self).__name__} (id: "{self.id}") has been saved before.'
-            )
-
-        self._pre_save_operations(conflict_resolution=conflict_resolution)
-        client = Configurations().get_client()
-        response = client.post(url=self._route, json=self._get_create_payload())
-        retrieve_object = False
-        if response.status_code != HTTPStatus.CREATED:
-            if response.status_code == HTTPStatus.CONFLICT:
-                if conflict_resolution == "retrieve":
-                    retrieve_object = True
-                else:
-                    raise DuplicatedRecordException(response=response)
-            if not retrieve_object:
-                raise RecordCreationException(response=response)
-
-        if retrieve_object:
-            assert self.name is not None
-            object_dict = self._get_object_dict_by_name(name=self.name)
-        else:
-            object_dict = response.json()
-
-        self._update_cache(object_dict)  # update api object cache store
-        type(self).__init__(
-            self,
-            **object_dict,
-            **self._get_init_params_from_object(),
-        )
-
-
-class DeletableApiObject(ApiObject):
-    """
-    DeleteMixin contains common methods used to delete an object
-    """
-
-    def _delete(self) -> None:
-        client = Configurations().get_client()
-        response = client.delete(url=f"{self._route}/{self.id}")
-        if response.status_code != HTTPStatus.OK:
-            raise RecordDeletionException(response, "Failed to delete the specified object.")
```

### Comparing `featurebyte-0.2.2/featurebyte/api/api_object_util.py` & `featurebyte-0.3.0/featurebyte/api/api_object_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 API Object Util
 """
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
 import ctypes
 import threading
 
-from rich.pretty import pretty_repr
-
 from featurebyte.config import Configurations
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.logging import get_logger
 
 logger = get_logger(__name__)
 
 
@@ -80,23 +78,14 @@
                 ctypes.c_long(thread_id), ctypes.py_object(SystemExit)
             )
             if res > 1:
                 ctypes.pythonapi.PyThreadState_SetAsyncExc(thread_id, 0)
                 logger.warning("Exception raise failure")
 
 
-class PrettyDict(Dict[str, Any]):
-    """
-    Dict with prettified representation
-    """
-
-    def __repr__(self) -> str:
-        return pretty_repr(dict(self), expand_all=True, indent_size=2)
-
-
 class NameAttributeUpdatableMixin:
     """
     This mixin is used to handle the case when name of the api object is updatable.
     """
 
     def __getattribute__(self, item: str) -> Any:
         """
```

### Comparing `featurebyte-0.2.2/featurebyte/api/asat_aggregator.py` & `featurebyte-0.3.0/featurebyte/api/asat_aggregator.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,17 +136,14 @@
 
         if method == AggFunc.LATEST:
             raise ValueError("latest aggregation method is not supported for aggregated_asat")
 
         if feature_name is None:
             raise ValueError("feature_name is required")
 
-        if self.category is not None:
-            raise ValueError("category is not supported for aggregate_asat")
-
         view = cast(SCDView, self.view)
         for key in self.keys:
             if key == view.natural_key_column:
                 raise ValueError(
                     "Natural key column cannot be used as a groupby key in aggregate_asat"
                 )
```

### Comparing `featurebyte-0.2.2/featurebyte/api/base_aggregator.py` & `featurebyte-0.3.0/featurebyte/api/base_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/base_table.py` & `featurebyte-0.3.0/featurebyte/api/base_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 DataColumn class
 """
+# pylint: disable=too-many-lines
 from __future__ import annotations
 
 from typing import Any, ClassVar, List, Literal, Optional, Tuple, Type, TypeVar, Union, cast
 
 from datetime import datetime
 from http import HTTPStatus
 
 import pandas as pd
 from bson.objectid import ObjectId
 from pandas import DataFrame
 from pydantic import Field
 from typeguard import typechecked
 
-from featurebyte.api.api_object import ApiObject, ForeignKeyMapping, SavableApiObject
+from featurebyte.api.api_object import ApiObject, ForeignKeyMapping
 from featurebyte.api.entity import Entity
+from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.api.source_table import AbstractTableData, SourceTable
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.config import Configurations
 from featurebyte.core.mixin import GetAttrMixin, ParentMixin
 from featurebyte.enum import TableDataType, ViewMode
 from featurebyte.exception import DuplicatedRecordException, RecordRetrievalException
 from featurebyte.models.base import FeatureByteBaseModel, PydanticObjectId
@@ -63,14 +65,49 @@
         -------
         ColumnInfo
         """
         column_info = next(col for col in self.parent.columns_info if col.name == self.name)
         return cast(ColumnInfo, column_info)
 
     @property
+    def cleaning_operations(self) -> List[CleaningOperation]:
+        """
+        Cleaning operations applied to the column of the table.
+
+        Returns
+        -------
+        List[CleaningOperation]
+            List of cleaning operations applied to the column of the table.
+
+        Examples
+        --------
+        Show the list of cleaning operations of the event table amount column after updating the critical
+        data info.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(
+        ...    cleaning_operations=[
+        ...        fb.MissingValueImputation(imputed_value=0),
+        ...    ]
+        ... )
+        >>> event_table["Amount"].cleaning_operations
+        [MissingValueImputation(imputed_value=0, type=missing)]
+
+        Empty list of column cleaning operations of the event table amount column.
+
+        >>> event_table["Amount"].update_critical_data_info(cleaning_operations=[])
+        >>> event_table["Amount"].cleaning_operations
+        []
+        """
+        for column_cleaning_operations in self.parent.column_cleaning_operations:
+            if column_cleaning_operations.column_name == self.name:
+                return cast(List[CleaningOperation], column_cleaning_operations.cleaning_operations)
+        return []
+
+    @property
     def feature_store(self) -> FeatureStoreModel:
         """
         Feature store used by parent frame
 
         Returns
         -------
         FeatureStoreModel
@@ -253,14 +290,35 @@
         after_cleaning: bool
             Whether to apply cleaning operations.
 
         Returns
         -------
         pd.DataFrame
             Preview rows of the table column.
+
+        Examples
+        --------
+        Preview a table without cleaning operations.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> description = event_table.preview(limit=5)
+
+
+        Preview a table after cleaning operations have been applied.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(  # doctest: +SKIP
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...   ]
+        ... )
+        >>> description = event_table.preview(
+        ...   limit=5,
+        ...   after_cleaning=True
+        ... )
         """
         return self.parent.preview(limit=limit, after_cleaning=after_cleaning)[[self.info.name]]
 
     @typechecked
     def shape(self, after_cleaning: bool = False) -> Tuple[int, int]:
         """
         Return the shape of the table column.
@@ -309,14 +367,35 @@
         after_cleaning: bool
             Whether to sample the table after cleaning
 
         Returns
         -------
         pd.DataFrame
             Sampled rows from the table column.
+
+        Examples
+        --------
+        Sample 3 rows from the table.
+        >>> sample = catalog.get_table("GROCERYINVOICE")["Amount"].sample(3)
+
+
+        Sample 3 rows from the table with timestamps after cleaning operations have been applied.
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(  # doctest: +SKIP
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...   ]
+        ... )
+        >>> event_table["Amount"].sample(  # doctest: +SKIP
+        ...   size=3,
+        ...   seed=111,
+        ...   from_timestamp=datetime(2019, 1, 1),
+        ...   to_timestamp=datetime(2023, 12, 31),
+        ...   after_cleaning=True,
+        ... )
         """
         return self.parent.sample(
             size=size,
             seed=seed,
             from_timestamp=from_timestamp,
             to_timestamp=to_timestamp,
             after_cleaning=after_cleaning,
@@ -348,14 +427,39 @@
         after_cleaning: bool
             Whether to compute description statistics after cleaning.
 
         Returns
         -------
         pd.DataFrame
             Summary of the table column.
+
+        Examples
+        --------
+        Describe a table without cleaning operations
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> description = event_table["Amount"].describe(
+        ...   from_timestamp=datetime(2020, 1, 1),
+        ...   to_timestamp=datetime(2020, 1, 31),
+        ... )
+
+
+        Describe a table after cleaning operations have been applied.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(  # doctest: +SKIP
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...   ]
+        ... )
+        >>> description = event_table["Amount"].describe(
+        ...   from_timestamp=datetime(2020, 1, 1),
+        ...   to_timestamp=datetime(2020, 1, 31),
+        ...   after_cleaning=True
+        ... )
         """
         return self.parent.describe(
             size=size,
             seed=seed,
             from_timestamp=from_timestamp,
             to_timestamp=to_timestamp,
             after_cleaning=after_cleaning,
@@ -457,14 +561,19 @@
         the column.
 
         Returns
         -------
         List[ColumnInfo]
             List of column information.
 
+        Examples
+        --------
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> column_info = event_table.columns_info
+
         See Also
         --------
         - [Table.column_cleaning_operations](/reference/featurebyte.api.base_table.TableApiObject.column_cleaning_operations)
         - [TableColumn.update_critical_data_info](/reference/featurebyte.api.base_table.TableColumn.update_critical_data_info)
         """
         try:
             return self.cached_model.columns_info  # pylint: disable=no-member
@@ -533,31 +642,50 @@
         try:
             return self.cached_model.record_creation_timestamp_column  # pylint: disable=no-member
         except RecordRetrievalException:
             return self.internal_record_creation_timestamp_column
 
     @property
     def column_cleaning_operations(self) -> List[ColumnCleaningOperation]:
+        # pylint: disable=line-too-long
         """
         List of column cleaning operations associated with this table. Column cleaning operation is a list of
         cleaning operations to be applied to a column of this table.
 
         Returns
         -------
         List[ColumnCleaningOperation]
             List of column cleaning operations
 
         Examples
         --------
-        Show the list of column cleaning operations of an event table
+        Show the list of column cleaning operations of an event table.
 
         >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...     fb.ValueBeyondEndpointImputation(
+        ...       type="less_than", end_point=0, imputed_value=0
+        ...     ),
+        ...   ]
+        ... )
+        >>> event_table.column_cleaning_operations
+        [ColumnCleaningOperation(column_name='Amount', cleaning_operations=[MissingValueImputation(imputed_value=0, type=missing), ValueBeyondEndpointImputation(imputed_value=0, type=less_than, end_point=0)])]
+
+        Empty list of column cleaning operations after resetting the cleaning operations.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(
+        ...   cleaning_operations=[]
+        ... )
         >>> event_table.column_cleaning_operations
         []
 
+
         See Also
         --------
         - [Table.columns_info](/reference/featurebyte.api.base_table.TableApiObject.columns_info)
         - [TableColumn.update_critical_data_info](/reference/featurebyte.api.base_table.TableColumn.update_critical_data_info)
         """
         return [
             ColumnCleaningOperation(
@@ -711,21 +839,42 @@
         after_cleaning: bool
             Whether to apply cleaning operations.
 
         Returns
         -------
         pd.DataFrame
             Summary of the table.
+
+        Examples
+        --------
+        Describe a table without cleaning operations
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> description = event_table.describe(
+        ...   from_timestamp=datetime(2020, 1, 1),
+        ...   to_timestamp=datetime(2020, 1, 31),
+        ... )
+
+
+        Describe a table after cleaning operations have been applied.
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(  # doctest: +SKIP
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...   ]
+        ... )
+        >>> description = event_table.describe(
+        ...   from_timestamp=datetime(2020, 1, 1),
+        ...   to_timestamp=datetime(2020, 1, 31),
+        ...   after_cleaning=True
+        ... )
         """
         return super().describe(size, seed, from_timestamp, to_timestamp, after_cleaning)
 
     @typechecked
-    def preview(  # pylint: disable=useless-parent-delegation
-        self, limit: int = 10, after_cleaning: bool = False
-    ) -> pd.DataFrame:
+    def preview(self, limit: int = 10, after_cleaning: bool = False) -> pd.DataFrame:
         """
         Returns a DataFrame that contains a selection of rows of the table. By default, the materialization process
         occurs before any cleaning operations that were defined at the table level.
 
         Parameters
         ----------
         limit: int
@@ -733,14 +882,35 @@
         after_cleaning: bool
             Whether to apply cleaning operations.
 
         Returns
         -------
         pd.DataFrame
             Preview rows of the table.
+
+        Examples
+        --------
+        Preview a table without cleaning operations.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> description = event_table.preview(limit=5)
+
+
+        Preview a table after cleaning operations have been applied.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(  # doctest: +SKIP
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...   ]
+        ... )
+        >>> description = event_table.preview(
+        ...   limit=5,
+        ...   after_cleaning=True
+        ... )
         """
         return super().preview(limit=limit, after_cleaning=after_cleaning)
 
     @typechecked
     def __getitem__(self, item: str) -> TableColumn:
         """
         Retrieve column from the table
@@ -807,15 +977,15 @@
             Table status
 
         Examples
         --------
         Update table status
 
         >>> event_table = catalog.get_table("GROCERYINVOICE")
-        >>> event_table.update_status(TableStatus.PUBLIC_DRAFT)
+        >>> event_table.update_status(fb.TableStatus.PUBLIC_DRAFT)
         """
         self.update(update_payload={"status": str(status)}, allow_update_local=False)
 
     @staticmethod
     def _validate_view_mode_params(
         view_mode: ViewMode,
         drop_column_names: Optional[List[str]],
```

### Comparing `featurebyte-0.2.2/featurebyte/api/batch_feature_table.py` & `featurebyte-0.3.0/featurebyte/worker/task/mixin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 """
-BatchFeatureTable class
+Mixin classes for tasks
 """
 from __future__ import annotations
 
-import pandas as pd
+from typing import Any, AsyncIterator, Callable
 
-from featurebyte.api.api_object import ApiObject, ForeignKeyMapping
-from featurebyte.api.batch_request_table import BatchRequestTable
-from featurebyte.api.feature_store import FeatureStore
-from featurebyte.api.materialized_table import MaterializedTableMixin
-from featurebyte.common.doc_util import FBAutoDoc
-from featurebyte.models.batch_feature_table import BatchFeatureTableModel
-from featurebyte.schema.batch_feature_table import BatchFeatureTableListRecord
+from contextlib import asynccontextmanager
 
+from featurebyte.logging import get_logger
+from featurebyte.models.feature_store import FeatureStoreModel
+from featurebyte.query_graph.node.schema import TableDetails
+from featurebyte.schema.worker.task.base import BaseTaskPayload
+from featurebyte.session.base import BaseSession
+from featurebyte.session.manager import SessionManager
 
-class BatchFeatureTable(BatchFeatureTableModel, ApiObject, MaterializedTableMixin):
+logger = get_logger(__name__)
+
+
+class DataWarehouseMixin:
     """
-    BatchFeatureTable class
+    DataWarehouseMixin contains common methods for tasks that interact with data warehouses.
     """
 
-    __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.BatchFeatureTable")
-
-    _route = "/batch_feature_table"
-    _list_schema = BatchFeatureTableListRecord
-    _get_schema = BatchFeatureTableModel
-    _list_fields = [
-        "name",
-        "feature_store_name",
-        "batch_request_table_name",
-        "shape",
-        "created_at",
-    ]
-    _list_foreign_keys = [
-        ForeignKeyMapping("feature_store_id", FeatureStore, "feature_store_name"),
-        ForeignKeyMapping("batch_request_table_id", BatchRequestTable, "batch_request_table_name"),
-    ]
+    payload: BaseTaskPayload
+    get_credential: Callable[..., Any]
 
-    def preview(self, limit: int = 10) -> pd.DataFrame:
+    async def get_db_session(self, feature_store: FeatureStoreModel) -> BaseSession:
         """
-        Returns a DataFrame that contains a selection of rows of the batch feature table.
+        Get the database session
 
         Parameters
         ----------
-        limit: int
-            Maximum number of return rows.
+        feature_store: FeatureStoreModel
+            The feature store model
 
         Returns
         -------
-        pd.DataFrame
-            Preview rows of the table.
+        BaseSession
         """
-        return super().preview(limit=limit)
-
-    def sample(self, size: int = 10, seed: int = 1234) -> pd.DataFrame:
+        session_manager = SessionManager(
+            credentials={
+                feature_store.name: await self.get_credential(
+                    user_id=self.payload.user_id,
+                    feature_store_name=feature_store.name,
+                )
+            }
+        )
+        return await session_manager.get_session(feature_store)
+
+    @asynccontextmanager
+    async def drop_table_on_error(
+        self, db_session: BaseSession, table_details: TableDetails
+    ) -> AsyncIterator[None]:
         """
-        Returns a DataFrame that contains a random selection of rows of the batch feature table based on a
-        specified size and seed for sampling control.
+        Drop the table on error
 
         Parameters
         ----------
-        size: int
-            Maximum number of rows to sample.
-        seed: int
-            Seed to use for random sampling.
-
-        Returns
-        -------
-        pd.DataFrame
-            Sampled rows from the table.
-        """
-        return super().sample(size=size, seed=seed)
-
-    def describe(self, size: int = 0, seed: int = 1234) -> pd.DataFrame:
-        """
-        Returns descriptive statistics of the batch feature table.
-
-        Parameters
-        ----------
-        size: int
-            Maximum number of rows to sample. If 0, all rows will be used.
-        seed: int
-            Seed to use for random sampling.
-
-        Returns
-        -------
-        pd.DataFrame
-            Summary of the table.
-        """
-        return super().describe(size=size, seed=seed)
+        db_session: BaseSession
+            The database session
+        table_details: TableDetails
+            The table details
+
+        Yields
+        ------
+        AsyncIterator[None]
+            The async iterator
+
+        Raises
+        ------
+        Exception
+            If error occurs within the context
+        """
+        try:
+            yield
+        except Exception as exc:
+            logger.error(
+                "Failed to create request table. Dropping table.",
+                extra={"error": str(exc), "task_payload": self.payload.dict()},
+            )
+            assert table_details.schema_name is not None
+            assert table_details.database_name is not None
+            await db_session.drop_table(
+                table_name=table_details.table_name,
+                schema_name=table_details.schema_name,
+                database_name=table_details.database_name,
+                if_exists=True,
+            )
+            raise exc
```

### Comparing `featurebyte-0.2.2/featurebyte/api/catalog.py` & `featurebyte-0.3.0/featurebyte/api/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typing import Any, Dict, List, Literal, Optional, Union
 
 import pandas as pd
 from bson import ObjectId
 from pydantic import Field
 from typeguard import typechecked
 
-from featurebyte.api.api_object import SavableApiObject
 from featurebyte.api.api_object_util import NameAttributeUpdatableMixin
 from featurebyte.api.batch_feature_table import BatchFeatureTable
 from featurebyte.api.batch_request_table import BatchRequestTable
 from featurebyte.api.catalog_decorator import update_and_reset_catalog
 from featurebyte.api.catalog_get_by_id_mixin import CatalogGetByIdMixin
 from featurebyte.api.data_source import DataSource
 from featurebyte.api.deployment import Deployment
@@ -24,14 +23,15 @@
 from featurebyte.api.feature_job_setting_analysis import FeatureJobSettingAnalysis
 from featurebyte.api.feature_list import FeatureList
 from featurebyte.api.feature_store import FeatureStore
 from featurebyte.api.historical_feature_table import HistoricalFeatureTable
 from featurebyte.api.observation_table import ObservationTable
 from featurebyte.api.periodic_task import PeriodicTask
 from featurebyte.api.relationship import Relationship
+from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.api.table import Table
 from featurebyte.api.view import View
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.logging import get_logger
 from featurebyte.models.base import PydanticObjectId, activate_catalog, get_active_catalog_id
 from featurebyte.models.catalog import CatalogModel
@@ -89,17 +89,15 @@
         except RecordRetrievalException:
             return self.internal_default_feature_store_ids
 
     def _get_create_payload(self) -> Dict[str, Any]:
         data = CatalogCreate(**self.json_dict())
         return data.json_dict()
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         Returns a dictionary that summarizes the essential information of a Catalog object. The dictionary includes
         the following keys:
 
         - `name`: The name of the Catalog object.
         - `created_at`: The timestamp indicating when the Catalog object was created.
         - `updated_at`: The timestamp indicating when the Catalog object was last updated.
@@ -141,19 +139,14 @@
 
         Returns
         -------
         Catalog
 
         Examples
         --------
-        >>> catalog = Catalog.activate("default")
-        >>> catalog.list_tables()[["name", "type"]]
-        Empty DataFrame
-        Columns: [name, type]
-        Index: []
         >>> catalog = Catalog.activate("grocery")
         >>> catalog.list_tables()[["name", "type"]]
                         name             type
         0     GROCERYPRODUCT  dimension_table
         1    GROCERYCUSTOMER        scd_table
         2       INVOICEITEMS       item_table
         3     GROCERYINVOICE      event_table
@@ -300,15 +293,15 @@
         Returns
         -------
         list[dict[str, Any]]
         """
         return self._get_audit_history(field_name="name")
 
     @classmethod
-    def get(cls, name: str) -> Catalog:  # pylint: disable=useless-parent-delegation
+    def get(cls, name: str) -> Catalog:
         """
         Gets a Catalog object by its name.
 
         Parameters
         ----------
         name: str
             Name of the catalog to retrieve.
@@ -318,22 +311,20 @@
         Catalog
             Catalog object.
 
         Examples
         --------
         Get a Catalog object that is already saved.
 
-        >>> catalog = fb.Catalog.get("catalog_name")  # doctest: +SKIP
+        >>> catalog = fb.Catalog.get(<catalog_name>)  # doctest: +SKIP
         """
         return super().get(name)
 
     @classmethod
-    def get_by_id(  # pylint: disable=useless-parent-delegation
-        cls, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
-    ) -> Catalog:
+    def get_by_id(cls, id: ObjectId) -> Catalog:  # pylint: disable=redefined-builtin,invalid-name
         """
         Returns a Catalog object by its unique identifier (ID).
 
         Parameters
         ----------
         id: ObjectId
             Catalog unique identifier ID.
@@ -348,17 +339,15 @@
         Get a Catalog object that is already saved.
 
         >>> fb.Catalog.get_by_id(<catalog_id>)  # doctest: +SKIP
         """
         return super().get_by_id(id=id)
 
     @classmethod
-    def list(
-        cls, include_id: Optional[bool] = True
-    ) -> pd.DataFrame:  # pylint: disable=useless-parent-delegation
+    def list(cls, include_id: Optional[bool] = True) -> pd.DataFrame:
         """
         Returns a DataFrame containing information on catalogs such as their names, creation dates, and active status.
 
         Parameters
         ----------
         include_id: Optional[bool]
             Whether to include id in the list.
@@ -442,26 +431,34 @@
         Returns
         -------
         pd.DataFrame
             Table of features
 
         Examples
         --------
-        List saved features.
+        List all features saved in the catalog.
 
         >>> features = catalog.list_features()
+
+
+        List all features having grocerycustomer or frenchstate as primary entity.
+
+        >>> customer_or_state_features = catalog.list_features(
+        ...   primary_entity = ["grocerycustomer", "frenchstate"]
+        ... )
         """
         return Feature.list(
             include_id=include_id, primary_entity=primary_entity, primary_table=primary_table
         )
 
     @update_and_reset_catalog
     def list_feature_lists(
         self,
         include_id: Optional[bool] = True,
+        primary_entity: Optional[Union[str, List[str]]] = None,
         entity: Optional[str] = None,
         table: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         Returns a DataFrame that contains various attributes of the registered feature lists. These attributes
         include the names of the feature lists, the number of features in each list, their status, whether they have
         been deployed in production, the percentage of production ready features of their default version, the tables
@@ -470,31 +467,34 @@
         The resulting DataFrame can be filtered based on the primary entity of the feature lists or the tables
         utilized by the feature lists.
 
         Parameters
         ----------
         include_id: Optional[bool]
             Whether to include id in the list.
+        primary_entity: Optional[Union[str, List[str]]] = None,
+            Name of entity used to filter results. If multiple entities are provided, the filtered results will
+            contain feature lists that are associated with all the entities.
         entity: Optional[str]
             Name of entity used to filter results.
         table: Optional[str]
             Name of table used to filter results.
 
         Returns
         -------
         pd.DataFrame
             Table of feature lists.
 
         Examples
         --------
-        List saved feature lists.
-
         >>> feature_lists = catalog.list_feature_lists()
         """
-        return FeatureList.list(include_id=include_id, entity=entity, table=table)
+        return FeatureList.list(
+            include_id=include_id, primary_entity=primary_entity, entity=entity, table=table
+        )
 
     @update_and_reset_catalog
     def list_tables(
         self, include_id: Optional[bool] = True, entity: Optional[str] = None
     ) -> pd.DataFrame:
         """
         Returns a DataFrame that contains various attributes of the registered tables in the catalog, such as their
@@ -512,16 +512,14 @@
         Returns
         -------
         pd.DataFrame
             Dataframe of tables
 
         Examples
         --------
-        List saved tables.
-
         >>> tables = catalog.list_tables()
         """
         return Table.list(include_id=include_id, entity=entity)
 
     @update_and_reset_catalog
     def list_relationships(
         self, include_id: Optional[bool] = True, relationship_type: Optional[Literal[tuple(RelationshipType)]] = None  # type: ignore
@@ -561,25 +559,14 @@
         ...     "relationship_type",
         ...     "entity",
         ...     "related_entity",
         ... ]]
           relationship_type           entity   related_entity
         0      child_parent   groceryinvoice  grocerycustomer
         1      child_parent  grocerycustomer      frenchstate
-
-        List all child-parent relationships.
-
-        >>> catalog.list_relationships(relationship_type="child_parent")[[
-        ...     "relationship_type",
-        ...     "entity",
-        ...     "related_entity",
-        ... ]]
-          relationship_type           entity   related_entity
-        0      child_parent   groceryinvoice  grocerycustomer
-        1      child_parent  grocerycustomer      frenchstate
         """
         return Relationship.list(include_id=include_id, relationship_type=relationship_type)
 
     @update_and_reset_catalog
     def list_feature_job_setting_analyses(
         self,
         include_id: Optional[bool] = True,
@@ -645,16 +632,14 @@
         Returns
         -------
         pd.DataFrame
             Table of entities.
 
         Examples
         --------
-        List saved entities.
-
         >>> entities = catalog.list_entities()
         """
         return Entity.list(include_id=include_id)
 
     @update_and_reset_catalog
     def list_periodic_tasks(self, include_id: Optional[bool] = True) -> pd.DataFrame:
         """
@@ -801,16 +786,14 @@
         Returns
         -------
         DataSource
             Data source object
 
         Examples
         --------
-        Get data source.
-
         >>> data_source = catalog.get_data_source()
         """
         assert (
             len(self.internal_default_feature_store_ids) == 1
         ), "No active catalog in this session. Please activate an existing catalog or create a new one to proceed."
         feature_store = FeatureStore.get_by_id(id=self.internal_default_feature_store_ids[0])
         return feature_store.get_data_source()  # pylint: disable=no-member
@@ -831,16 +814,14 @@
         Returns
         -------
         View
             View object.
 
         Examples
         --------
-        Get an event view from an event table.
-
         >>> event_view = catalog.get_view("GROCERYINVOICE")
         """
         table = Table.get(name=table_name)
         return table.get_view()  # type: ignore[no-any-return]
 
     @update_and_reset_catalog
     def get_feature(self, name: str, version: Optional[str] = None) -> Feature:
@@ -861,17 +842,23 @@
         Returns
         -------
         Feature
             Feature object.
 
         Examples
         --------
-        Get a saved feature.
+        Get a default version of a feature by its name space.
 
         >>> feature = catalog.get_feature("InvoiceAmountAvg_60days")
+
+        Get a specific version of a feature by specifying its version name.
+
+        >>> feature = catalog.get_feature(  # doctest: +SKIP
+        ...   "InvoiceAmountAvg_60days", version=<version_name>
+        ... )
         """
         return Feature.get(name=name, version=version)
 
     @update_and_reset_catalog
     def get_feature_list(self, name: str, version: Optional[str] = None) -> FeatureList:
         """
         Gets a FeatureList object from the catalog by specifying the feature list's name and, optionally,
@@ -888,16 +875,14 @@
         Returns
         -------
         FeatureList
             Feature list object.
 
         Examples
         --------
-        Get a saved feature list.
-
         >>> feature_list = catalog.get_feature_list("invoice_feature_list")
         """
         return FeatureList.get(name=name, version=version)
 
     @update_and_reset_catalog
     def get_table(self, name: str) -> Any:
         """
@@ -915,16 +900,14 @@
         Returns
         -------
         Any
             Retrieved table.
 
         Examples
         --------
-        Get a saved table.
-
         >>> item_table = catalog.get_table("INVOICEITEMS")
         """
         return Table.get(name=name)
 
     @update_and_reset_catalog
     def get_relationship(self, name: str) -> Relationship:
         """
@@ -984,16 +967,14 @@
         Returns
         -------
         FeatureJobSettingAnalysis
             Feature job setting analysis object.
 
         Examples
         --------
-        Get a saved feature job setting analysis.
-
         >>> feature_job_setting_analysis = catalog.get_feature_job_setting_analysis("analysis_name")  # doctest: +SKIP
         """
         return FeatureJobSettingAnalysis.get(name=name)
 
     @update_and_reset_catalog
     def get_feature_store(self, name: str) -> FeatureStore:
         """
@@ -1033,16 +1014,14 @@
         Returns
         -------
         Entity
             Entity object.
 
         Examples
         --------
-        Get a saved entity.
-
         >>> entity = catalog.get_entity("grocerycustomer")
         """
         return Entity.get(name=name)
 
     @update_and_reset_catalog
     def get_periodic_task(self, name: str) -> PeriodicTask:
         """
```

### Comparing `featurebyte-0.2.2/featurebyte/api/catalog_decorator.py` & `featurebyte-0.3.0/featurebyte/api/catalog_decorator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/catalog_get_by_id_mixin.py` & `featurebyte-0.3.0/featurebyte/api/catalog_get_by_id_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         Feature
             Feature object.
 
         Examples
         --------
         Get a saved feature.
 
-        >>> feature = catalog.get_feature_by_id(ObjectId())  # doctest: +SKIP
+        >>> feature = catalog.get_feature_by_id(<Feature_Object_Id>)  # doctest: +SKIP
         """
         return Feature.get_by_id(id=id)
 
     @update_and_reset_catalog
     def get_feature_list_by_id(
         self, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> FeatureList:
@@ -124,15 +124,15 @@
         FeatureList
             Feature list object.
 
         Examples
         --------
         Get a saved feature list.
 
-        >>> feature_list = catalog.get_feature_list_by_id(ObjectId())  # doctest: +SKIP
+        >>> feature_list = catalog.get_feature_list_by_id(<Feature_Object_ID>)  # doctest: +SKIP
         """
         return FeatureList.get_by_id(id=id)
 
     @update_and_reset_catalog
     def get_table_by_id(
         self, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> Any:
@@ -149,15 +149,15 @@
         Any
             Retrieved table.
 
         Examples
         --------
         Get a saved table.
 
-        >>> item_table = catalog.get_table_by_id(ObjectId())  # doctest: +SKIP
+        >>> item_table = catalog.get_table_by_id(<table_Object_ID>)  # doctest: +SKIP
         """
         return Table.get_by_id(id=id)
 
     @update_and_reset_catalog
     def get_relationship_by_id(
         self, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> Relationship:
@@ -174,15 +174,15 @@
         Relationship
             Relationship object.
 
         Examples
         --------
         Get a saved relationship.
 
-        >>> relationship = catalog.get_relationship_by_id(ObjectId())  # doctest: +SKIP
+        >>> relationship = catalog.get_relationship_by_id(<Relationship_Object_ID>)  # doctest: +SKIP
         """
         return Relationship.get_by_id(id=id)
 
     @update_and_reset_catalog
     def get_feature_job_setting_analysis_by_id(
         self, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> FeatureJobSettingAnalysis:
@@ -249,15 +249,15 @@
         Entity
             Entity object.
 
         Examples
         --------
         Get a saved entity.
 
-        >>> entity = catalog.get_entity_by_id(ObjectId())  # doctest: +SKIP
+        >>> entity = catalog.get_entity_by_id(<Entity_Object_ID>)  # doctest: +SKIP
         """
         return Entity.get_by_id(id=id)
 
     @update_and_reset_catalog
     def get_periodic_task_by_id(
         self, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> PeriodicTask:
```

### Comparing `featurebyte-0.2.2/featurebyte/api/change_view.py` & `featurebyte-0.3.0/featurebyte/api/change_view.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 ChangeView class
 """
 from __future__ import annotations
 
-from typing import Any, ClassVar, Optional, Tuple
+from typing import Any, ClassVar, List, Optional, Tuple, Union
 
 from datetime import datetime
 
 from pydantic import Field
 from typeguard import typechecked
 
 from featurebyte.api.lag import LaggableViewColumn
@@ -23,14 +23,59 @@
     """
     ChangeViewColumn class
     """
 
     # documentation metadata
     __fbautodoc__ = FBAutoDoc()
 
+    @typechecked
+    def lag(
+        self: ChangeViewColumn, entity_columns: Union[str, List[str]], offset: int = 1
+    ) -> ChangeViewColumn:
+        """
+        Lag is a transform that enables the retrieval of the preceding value associated with a particular entity in
+        a view.
+
+        This makes it feasible to compute essential features, such as those that depend on inter-event time
+        and the proximity to the previous point.
+
+        Parameters
+        ----------
+        entity_columns : str | list[str]
+            Entity columns used when retrieving the lag value.
+        offset : int
+            The number of rows backward from which to retrieve a value.
+
+        Returns
+        -------
+        ChangeViewColumn
+
+        Raises
+        ------
+        ValueError
+            If a lag operation has already been applied to the column.
+
+        Examples
+        --------
+        Get a ChangeView to track changes in Customer's State.
+
+        >>> scd_table = catalog.get_table("GROCERYCUSTOMER")
+        >>> change_view = scd_table.get_change_view(
+        ...   track_changes_column="State"
+        ... )
+
+
+        Create a new column that indicates the prior past_State for a Customer
+
+        >>> lagged_column = change_view["past_State"].lag("GroceryCustomerGuid")
+
+        # noqa: DAR402
+        """
+        return super().lag(entity_columns, offset)
+
 
 class ChangeView(View, GroupByMixin):
     """
     A ChangeView object is used to capture changes in SCDTable object in an easy manner. This is useful as
     changes in SCDTable may constitute powerful features such as:
 
     - how many times has a customer moved in the past 6 months?
```

### Comparing `featurebyte-0.2.2/featurebyte/api/credential.py` & `featurebyte-0.3.0/featurebyte/api/credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
 from pydantic import Field
 from typeguard import typechecked
 
-from featurebyte.api.api_object import DeletableApiObject, ForeignKeyMapping, SavableApiObject
+from featurebyte.api.api_object import ForeignKeyMapping
 from featurebyte.api.feature_store import FeatureStore
+from featurebyte.api.savable_api_object import DeletableApiObject, SavableApiObject
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.credential import (
     DatabaseCredential,
     DatabaseCredentialType,
     StorageCredential,
     StorageCredentialType,
@@ -21,14 +22,23 @@
 from featurebyte.schema.credential import CredentialCreate, CredentialRead, CredentialUpdate
 
 
 @typechecked
 class Credential(DeletableApiObject, SavableApiObject):
     """
     Credential class is the data model used to represent your credentials that are persisted.
+
+    Examples
+    --------
+    >>> credential = Credential(  # doctest: +SKIP
+    ...   name=feature_store.name,
+    ...   feature_store_id=feature_store.id,
+    ...   database_credential=database_credential,
+    ...   storage_credential=storage_credential,
+    ... )
     """
 
     # documentation metadata
     __fbautodoc__ = FBAutoDoc(
         proxy_class="featurebyte.Credential",
         skip_params_and_signature_in_class_docs=True,
     )
```

### Comparing `featurebyte-0.2.2/featurebyte/api/data_source.py` & `featurebyte-0.3.0/featurebyte/api/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,16 @@
             Name of schema.
 
         Returns
         -------
         List[str]
             List of tables.
 
+            **Note**: Tables with names that begins with `__` are excluded.
+
         Raises
         ------
         RecordRetrievalException
             Failed to retrieve database table list
 
         Examples
         --------
```

### Comparing `featurebyte-0.2.2/featurebyte/api/deployment.py` & `featurebyte-0.3.0/featurebyte/api/deployment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 Deployment module
 """
 from __future__ import annotations
 
-from typing import Literal
+from typing import Literal, Optional
 
 import json
 import os
 
+import pandas as pd
+from bson import ObjectId
 from jinja2 import Template
 from typeguard import typechecked
 
 from featurebyte.api.api_object import ApiObject, ForeignKeyMapping
 from featurebyte.api.batch_feature_table import BatchFeatureTable
 from featurebyte.api.batch_request_table import BatchRequestTable
 from featurebyte.api.entity import Entity
 from featurebyte.api.feature_job import FeatureJobStatusResult
 from featurebyte.api.feature_list import FeatureList
 from featurebyte.api.table import Table
 from featurebyte.common.doc_util import FBAutoDoc
-from featurebyte.common.utils import CodeStr
+from featurebyte.common.formatting_util import CodeStr
 from featurebyte.config import Configurations
 from featurebyte.exception import FeatureListNotOnlineEnabledError
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.deployment import DeploymentModel
 from featurebyte.schema.batch_feature_table import BatchFeatureTableCreate
 from featurebyte.schema.deployment import DeploymentUpdate
 
@@ -84,20 +86,30 @@
         PydanticObjectId
         """
         return self.cached_model.feature_list_id
 
     def enable(self) -> None:
         """
         Enable the deployment.
+
+        Examples
+        --------
+        >>> deployment = catalog.get_deployment(<deployment_name>)  # doctest: +SKIP
+        >>> deployment.enable()  # doctest: +SKIP
         """
         self.patch_async_task(route=f"{self._route}/{self.id}", payload={"enabled": True})
 
     def disable(self) -> None:
         """
         Disable the deployment.
+
+        Examples
+        --------
+        >>> deployment = catalog.get_deployment(<deployment_name>)  # doctest: +SKIP
+        >>> deployment.disable()  # doctest: +SKIP
         """
         self.patch_async_task(route=f"{self._route}/{self.id}", payload={"enabled": False})
 
     @typechecked
     def compute_batch_feature_table(
         self,
         batch_request_table: BatchRequestTable,
@@ -113,14 +125,22 @@
             Batch request table contains required serving names columns
         batch_feature_table_name: str
             Name of the batch feature table to be created
 
         Returns
         -------
         BatchFeatureTable
+
+        Examples
+        --------
+        >>. deployment = catalog.get_deployment(<deployment_name>)  # doctest: +SKIP
+        >>> batch_features = deployment.compute_batch_feature_table(  # doctest: +SKIP
+        ...   batch_request_table=batch_request_table,
+        ...   batch_feature_table_name = <batch_feature_table_name>
+        ... )
         """
         payload = BatchFeatureTableCreate(
             name=batch_feature_table_name,
             feature_store_id=batch_request_table.location.feature_store_id,
             batch_request_table_id=batch_request_table.id,
             deployment_id=self.id,
         )
@@ -170,15 +190,15 @@
                     Entity serving name values to used for serving request
                 Returns
                 -------
                 pd.DataFrame
                 "
                 response = requests.post(
                     url="http://localhost:8080/deployment/{deployment.id}/online_features",
-                    headers={{"Content-Type": "application/json", "active-catalog-id": "63eda344d0313fb925f7883a"}},
+                    headers={{"Content-Type": "application/json", "active-catalog-id": "{catalog.id}"}},
                     json={{"entity_serving_names": entity_serving_names}},
                 )
                 assert response.status_code == 200, response.json()
                 return pd.DataFrame.from_dict(response.json()["features"])
             request_features([{{"cust_id": "sample_cust_id"}}])
 
         Retrieve shell script template when "language" is set to "sh"
@@ -187,17 +207,17 @@
         >>> deployment = feature_list.deploy()  # doctest: +SKIP
         >>> deployment.enable()  # doctest: +SKIP
         >>> deployment.get_online_serving_code(language="sh")  # doctest: +SKIP
             \\#!/bin/sh
             curl -X POST
                 -H 'Content-Type: application/json' \\
                 -H 'Authorization: Bearer token' \\
-                -H 'active-catalog-id: 63eda344d0313fb925f7883a' \\
+                -H 'active-catalog-id: {catalog.id}' \\
                 -d '{{"entity_serving_names": [{{"cust_id": "sample_cust_id"}}]}}' \\
-                http://localhost:8080/deployment/641cf594f74f839cf9297884/online_features
+                http://localhost:8080/deployment/{deployment.id}/online_features
 
         See Also
         --------
         - [FeatureList.deploy](/reference/featurebyte.api.feature_list.FeatureList.deploy/)
         - [Deployment.enable](/reference/featurebyte.api.deployment.Deployment.enable/)
         """
         # pylint: disable=too-many-locals
@@ -289,7 +309,79 @@
         -------
         FeatureJobStatusResult
         """
         return FeatureList.get_by_id(self.feature_list_id).get_feature_jobs_status(
             job_history_window=job_history_window,
             job_duration_tolerance=job_duration_tolerance,
         )
+
+    @classmethod
+    def get(cls, name: str) -> Deployment:
+        """
+        Gets a Deployment object by its name.
+
+        Parameters
+        ----------
+        name: str
+            Name of the deployment to retrieve.
+
+        Returns
+        -------
+        Deployment
+            Deployment object.
+
+        Examples
+        --------
+        Get a Deployment object that is already saved.
+
+        >>> deployment = fb.Deployment.get(<deployment_name>)  # doctest: +SKIP
+        """
+        return super().get(name)
+
+    @classmethod
+    def get_by_id(
+        cls, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
+    ) -> Deployment:
+        """
+        Returns a Deployment object by its unique identifier (ID).
+
+        Parameters
+        ----------
+        id: ObjectId
+            Deployment unique identifier ID.
+
+        Returns
+        -------
+        Deployment
+            Deployment object.
+
+        Examples
+        --------
+        Get a Deployment object that is already saved.
+
+        >>> fb.Deployment.get_by_id(<deployment_id>)  # doctest: +SKIP
+        """
+        return cls._get_by_id(id=id)
+
+    @classmethod
+    def list(cls, include_id: Optional[bool] = True) -> pd.DataFrame:
+        """
+        Returns a DataFrame that lists the deployments by their names, feature list names, feature list versions,
+        number of features, and whether the features are enabled.
+
+        Parameters
+        ----------
+        include_id: Optional[bool]
+            Whether to include id in the list.
+
+        Returns
+        -------
+        DataFrame
+            Table of objects.
+
+        Examples
+        --------
+        List all deployments.
+
+        >>> deployments = fb.Deployment.list()
+        """
+        return super().list(include_id=include_id)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/dimension_table.py` & `featurebyte-0.3.0/featurebyte/api/dimension_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 DimensionTable class
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar, List, Literal, Optional, Type, cast
 
+from bson import ObjectId
 from pydantic import Field, StrictStr, root_validator
 
 from featurebyte.api.base_table import TableApiObject
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.validator import construct_data_model_root_validator
 from featurebyte.enum import DBVarType, TableDataType, ViewMode
 from featurebyte.exception import RecordRetrievalException
@@ -116,18 +117,35 @@
         Returns
         -------
         DimensionView
             DimensionView object constructed from the source table.
 
         Examples
         --------
-        Get a DimensionView.
+        Get a DimensionView in automated mode.
 
-        >>> dimension_table = fb.Table.get("GROCERYPRODUCT")
+        >>> dimension_table = catalog.get_table("GROCERYPRODUCT")
         >>> dimension_view = dimension_table.get_view()
+
+
+        Get a DimensionView in manual mode.
+
+        >>> dimension_table = catalog.get_table("GROCERYPRODUCT")
+        >>> dimension_view = dimension_table.get_view(
+        ...   view_mode="manual",
+        ...   drop_column_names=[],
+        ...   column_cleaning_operations=[
+        ...     fb.ColumnCleaningOperation(
+        ...       column_name="ProductGroup",
+        ...       cleaning_operations=[
+        ...         fb.MissingValueImputation(imputed_value="Unknown"),
+        ...       ],
+        ...     )
+        ...   ],
+        ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.dimension_view import DimensionView
 
         self._validate_view_mode_params(
             view_mode=view_mode,
             drop_column_names=drop_column_names,
@@ -187,7 +205,32 @@
             return self.cached_model.dimension_id_column
         except RecordRetrievalException:
             return self.internal_dimension_id_column
 
     @property
     def timestamp_column(self) -> Optional[str]:
         return None
+
+    @classmethod
+    def get_by_id(
+        cls, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
+    ) -> DimensionTable:
+        """
+        Returns a DimensionTable object by its unique identifier (ID).
+
+        Parameters
+        ----------
+        id: ObjectId
+            DimensionTable unique identifier ID.
+
+        Returns
+        -------
+        DimensionTable
+            DimensionTable object.
+
+        Examples
+        --------
+        Get a DimensionTable object that is already saved.
+
+        >>> fb.DimensionTable.get_by_id(<dimension_table_id>)  # doctest: +SKIP
+        """
+        return cls._get_by_id(id=id)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/dimension_view.py` & `featurebyte-0.3.0/featurebyte/api/dimension_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/entity.py` & `featurebyte-0.3.0/featurebyte/api/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 
 from http import HTTPStatus
 
 from bson import ObjectId
 from pydantic import Field
 from typeguard import typechecked
 
-from featurebyte.api.api_object import SavableApiObject
 from featurebyte.api.api_object_util import NameAttributeUpdatableMixin
+from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.config import Configurations
 from featurebyte.exception import RecordRetrievalException, RecordUpdateException
+from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.entity import EntityModel, ParentEntity
 from featurebyte.schema.entity import EntityCreate, EntityUpdate
 
 
 class Entity(NameAttributeUpdatableMixin, SavableApiObject):
     """
     Entity class to represent an entity in FeatureByte.
@@ -78,14 +79,30 @@
         """
         try:
             return self.cached_model.serving_names
         except RecordRetrievalException:
             return self.internal_serving_names
 
     @property
+    def catalog_id(self) -> PydanticObjectId:
+        """
+        Returns the unique identifier (ID) of the Catalog that is associated with the Entity object.
+
+        Returns
+        -------
+        PydanticObjectId
+            Catalog ID of the entity.
+
+        See Also
+        --------
+        - [Catalog](/reference/featurebyte.api.catalog.Catalog)
+        """
+        return self.cached_model.catalog_id  # pylint: disable=no-member
+
+    @property
     def serving_name(self) -> str:
         """
         First serving name of the entity serving names. An entity's serving names is the name of the unique
         identifier that is used to identify the entity during a preview or serving request. Typically, the
         serving name for an entity is the name of the primary key (or natural key) of the table that
         represents the entity.
 
@@ -319,17 +336,15 @@
         parent_entity = Entity.get(parent_entity_name)
         post_response = client.delete(
             f"{self._route}/{self.id}/parent/{parent_entity.id}",
         )
         if post_response.status_code != HTTPStatus.OK:
             raise RecordUpdateException(post_response)
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         Returns a dictionary that summarizes the essential information of an Entity object. The dictionary contains
         the following keys:
 
         - `name`: The name of the Entity object.
         - `created_at`: The timestamp indicating when the Entity object was created.
         - `updated_at`: The timestamp indicating when the Entity object was last updated.
@@ -342,9 +357,14 @@
         verbose: bool
             Control verbose level of the summary.
 
         Returns
         -------
         Dict[str, Any]
             Key-value mapping of properties of the object.
+
+        Examples
+        --------
+        >>> entity = catalog.get_entity("grocerycustomer")
+        >>> entity.info()  # doctest: +SKIP
         """
         return super().info(verbose)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/event_table.py` & `featurebyte-0.3.0/featurebyte/api/event_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, List, Literal, Optional, Type, Union, cast
 
 from datetime import datetime
 
 import pandas as pd
+from bson import ObjectId
 from pydantic import Field, StrictStr, root_validator
 from typeguard import typechecked
 
 from featurebyte.api.base_table import TableApiObject
 from featurebyte.api.feature_job_setting_analysis import FeatureJobSettingAnalysis
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.validator import construct_data_model_root_validator
@@ -136,18 +137,38 @@
         Returns
         -------
         EventView
             EventView object constructed from the source table.
 
         Examples
         --------
-        Get an EventView.
+        Get an EventView in automated mode.
 
-        >>> event_table = fb.Table.get("GROCERYINVOICE")
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
         >>> event_view = event_table.get_view()
+
+
+        Get an EventView in manual mode.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_view = event_table.get_view(
+        ...   view_mode="manual",
+        ...   drop_column_names=["record_available_at"],
+        ...   column_cleaning_operations=[
+        ...     fb.ColumnCleaningOperation(
+        ...       column_name="Amount",
+        ...       cleaning_operations=[
+        ...         fb.MissingValueImputation(imputed_value=0),
+        ...         fb.ValueBeyondEndpointImputation(
+        ...           type="less_than", end_point=0, imputed_value=None
+        ...         )
+        ...       ],
+        ...     )
+        ...   ],
+        ... )
         """
         from featurebyte.api.event_view import EventView  # pylint: disable=import-outside-toplevel
 
         self._validate_view_mode_params(
             view_mode=view_mode,
             drop_column_names=drop_column_names,
             column_cleaning_operations=column_cleaning_operations,
@@ -281,41 +302,65 @@
 
         Returns
         -------
         list[dict[str, Any]]
         """
         return self._get_audit_history(field_name="default_feature_job_setting")
 
+    @classmethod
+    def get_by_id(
+        cls, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
+    ) -> EventTable:
+        """
+        Returns an EventTable object by its unique identifier (ID).
+
+        Parameters
+        ----------
+        id: ObjectId
+            EventTable unique identifier ID.
+
+        Returns
+        -------
+        EventTable
+            EventTable object.
+
+        Examples
+        --------
+        Get an EventTable object that is already saved.
+
+        >>> fb.EventTable.get_by_id(<event_table_id>)  # doctest: +SKIP
+        """
+        return cls._get_by_id(id=id)
+
     @typechecked
     def update_default_feature_job_setting(self, feature_job_setting: FeatureJobSetting) -> None:
         """
         Update default feature job setting
 
         Parameters
         ----------
         feature_job_setting: FeatureJobSetting
             Feature job setting object
 
         Examples
         --------
-
-        Configure a feature job to run daily at 12am
+        Configure a feature job setting to run daily at 1:05 am with a blind spot of 10 minutes.
 
         >>> from featurebyte import FeatureJobSetting
         >>> new_feature_job_setting = FeatureJobSetting(
-        ...   blind_spot="0",
+        ...   blind_spot="10m",
         ...   frequency="24h",
-        ...   time_modulo_frequency="0",
+        ...   time_modulo_frequency="65m",
         ... )
 
-        Update default feature job setting to the new feature job setting
 
-        >>> event_table = catalog.get_table("GROCERYINVOICE")
-        >>> event_table.update_default_feature_job_setting(new_feature_job_setting)
+        Update default feature job setting to the new feature job setting.
 
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table.update_default_feature_job_setting(new_feature_job_setting)  # doctest: +SKIP
         """
         self.update(
             update_payload={"default_feature_job_setting": feature_job_setting.dict()},
             allow_update_local=True,
             add_internal_prefix=True,
         )
 
@@ -374,30 +419,37 @@
 
         Returns
         -------
         FeatureJobSettingAnalysis
 
         Examples
         --------
+        Create new feature job setting analysis on the saved event table with the following configuration:
 
-        Create new feature job setting analysis on the saved event table. It could also be called without
-        any parameters with default values.
+        - analysis should cover the last 2 weeks,
+        - recommendation for the feature job frequency period should be at least one hour,
+        - recent late data warehouse updates should be excluded in the analysis, as it is expected they won't occur
+          again because your instances have been upsized
+        - tolerance for late data is incresed to 0.5%.
 
         >>> from datetime import datetime
         >>> event_table = catalog.get_table("GROCERYINVOICE")
-        >>> event_table.create_new_feature_job_setting_analysis(  # doctest: +SKIP
+        >>> analysis = event_table.create_new_feature_job_setting_analysis(  # doctest: +SKIP
         ...   analysis_date=datetime.utcnow(),
-        ...   analysis_length=3600,
-        ...   min_featurejob_period=100,
+        ...   analysis_length=60*60*24*7*12,
+        ...   min_featurejob_period=60*60,
         ...   exclude_late_job=True,
         ...   blind_spot_buffer_setting=10,
         ...   job_time_buffer_setting=5,
-        ...   late_data_allowance=0.1,
+        ...   late_data_allowance=0.5/100,
         ... )
 
+        The analysis could also be called with default values.
+        >>> default_analysis = event_table.create_new_feature_job_setting_analysis()  # doctest: +SKIP
+
         """
         payload = FeatureJobSettingAnalysisCreate(
             event_table_id=self.id,
             analysis_date=analysis_date,
             analysis_length=analysis_length,
             min_featurejob_period=min_featurejob_period,
             exclude_late_job=exclude_late_job,
```

### Comparing `featurebyte-0.2.2/featurebyte/api/event_view.py` & `featurebyte-0.3.0/featurebyte/api/event_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, Optional, cast
 
 import copy
 
+from bson import ObjectId
 from pydantic import Field
 
 from featurebyte.api.lag import LaggableViewColumn
 from featurebyte.api.view import GroupByMixin, RawMixin, View
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.typing import validate_type_is_feature
 from featurebyte.enum import TableDataType
 from featurebyte.exception import EventViewMatchingEntityColumnNotFound
-from featurebyte.models.base import PydanticObjectId
 from featurebyte.query_graph.enum import GraphNodeType, NodeOutputType, NodeType
 from featurebyte.query_graph.model.column_info import ColumnInfo
 from featurebyte.query_graph.model.feature_job_setting import FeatureJobSetting
 from featurebyte.query_graph.node.input import EventTableInputNodeParameters, InputNode
 
 if TYPE_CHECKING:
     from featurebyte.api.feature import Feature
@@ -264,57 +264,57 @@
             entity column name
 
         Raises
         ------
         ValueError
             raised when the feature is created from more than one entity
         """
-        entity_columns = feature.entity_identifiers
+        entity_columns = feature.graph.get_entity_columns(node_name=feature.node_name)
         if len(entity_columns) != 1:
             raise ValueError(
                 "The feature should only be based on one entity. We are currently unable to add features "
                 "that are created from more, or less than one entity."
             )
         return entity_columns[0]
 
     @staticmethod
-    def _get_feature_entity_id(feature: Feature) -> PydanticObjectId:
+    def _get_feature_entity_id(feature: Feature) -> ObjectId:
         """
         Get the entity ID of the feature.
 
         Parameters
         ----------
         feature: Feature
             feature to get entity column for
 
         Returns
         -------
-        PydanticObjectId
+        ObjectId
             entity ID
 
         Raises
         ------
         ValueError
             raised when the feature is created from more than one entity
         """
-        entity_ids = feature.entity_ids
+        entity_ids = feature.graph.get_entity_ids(node_name=feature.node_name)
         if len(entity_ids) != 1:
             raise ValueError(
                 "The feature should only be based on one entity. We are currently unable to add features "
                 "that are created from more than one entity."
             )
         return entity_ids[0]
 
-    def _get_col_with_entity_id(self, entity_id: PydanticObjectId) -> Optional[str]:
+    def _get_col_with_entity_id(self, entity_id: ObjectId) -> Optional[str]:
         """
         Tries to find a single column with the matching entity ID.
 
         Parameters
         ----------
-        entity_id: PydanticObjectId
+        entity_id: ObjectId
             entity ID to search for
 
         Returns
         -------
         Optional[str]
             the column name with matching entity ID, None if no matches are found, or if there are multiple matches.
         """
@@ -395,18 +395,25 @@
         EventView
             The EventView with the new feature added.
 
         Examples
         --------
         Add feature to an EventView.
 
-        >>> event_view = catalog.get_view("GROCERYINVOICE")
-        >>> feature = catalog.get_feature("InvoiceCount")
-        >>> event_view = event_view.add_feature("invoice_count", feature)
-
+        >>> items_view = catalog.get_view("INVOICEITEMS")
+        >>> # Group items by the column GroceryInvoiceGuid that references the customer entity
+        >>> items_by_invoice = items_view.groupby("GroceryInvoiceGuid")  # doctest: +SKIP
+        >>> # Get the number of items in each invoice
+        >>> invoice_item_count = items_by_invoice.aggregate(  # doctest: +SKIP
+        ...   None,
+        ...   method=fb.AggFunc.COUNT,
+        ...   feature_name="InvoiceItemCount",
+        ... )
+        >>> event_view = catalog.get_view("GROCERYINVOICE")  # doctest: +SKIP
+        >>> event_view = event_view.add_feature("InvoiceItemCount", invoice_item_count)  # doctest: +SKIP
         """
         validate_type_is_feature(feature, "feature")
 
         # Validation
         self._validate_feature_addition(new_column_name, feature, entity_column)
 
         # Add join node
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature.py` & `featurebyte-0.3.0/featurebyte/api/feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,71 +10,64 @@
 from http import HTTPStatus
 
 import pandas as pd
 from bson import ObjectId
 from pydantic import Field, root_validator
 from typeguard import typechecked
 
-from featurebyte.api.api_object import ConflictResolution, DeletableApiObject, SavableApiObject
+from featurebyte.api.api_object import ConflictResolution
 from featurebyte.api.entity import Entity
 from featurebyte.api.feature_job import FeatureJobMixin
 from featurebyte.api.feature_namespace import FeatureNamespace
 from featurebyte.api.feature_store import FeatureStore
 from featurebyte.api.feature_util import FEATURE_COMMON_LIST_FIELDS, FEATURE_LIST_FOREIGN_KEYS
 from featurebyte.api.feature_validation_util import assert_is_lookup_feature
+from featurebyte.api.savable_api_object import DeletableApiObject, SavableApiObject
 from featurebyte.common.descriptor import ClassInstanceMethodDescriptor
 from featurebyte.common.doc_util import FBAutoDoc
+from featurebyte.common.formatting_util import CodeStr
 from featurebyte.common.typing import Scalar, ScalarSequence
-from featurebyte.common.utils import CodeStr, dataframe_from_json, enforce_observation_set_row_order
+from featurebyte.common.utils import dataframe_from_json, enforce_observation_set_row_order
 from featurebyte.config import Configurations
 from featurebyte.core.accessor.count_dict import CdAccessorMixin
-from featurebyte.core.generic import ProtectedColumnsQueryObject
+from featurebyte.core.accessor.feature_datetime import FeatureDtAccessorMixin
+from featurebyte.core.accessor.feature_string import FeatureStrAccessorMixin
 from featurebyte.core.series import FrozenSeries, FrozenSeriesT, Series
 from featurebyte.exception import RecordCreationException, RecordRetrievalException
 from featurebyte.feature_manager.model import ExtendedFeatureModel
 from featurebyte.logging import get_logger
-from featurebyte.models.base import PydanticObjectId, VersionIdentifier
-from featurebyte.models.feature import (
-    DefaultVersionMode,
-    FeatureModel,
-    FeatureReadiness,
-    FrozenFeatureModel,
-)
+from featurebyte.models.base import PydanticObjectId, VersionIdentifier, get_active_catalog_id
+from featurebyte.models.feature import DefaultVersionMode, FeatureModel, FeatureReadiness
 from featurebyte.models.feature_store import FeatureStoreModel
 from featurebyte.models.relationship_analysis import derive_primary_entity
 from featurebyte.models.tile import TileSpec
 from featurebyte.query_graph.enum import NodeOutputType, NodeType
 from featurebyte.query_graph.model.common_table import TabularSource
 from featurebyte.query_graph.model.feature_job_setting import TableFeatureJobSetting
 from featurebyte.query_graph.node.cleaning_operation import TableCleaningOperation
-from featurebyte.query_graph.node.generic import (
-    AliasNode,
-    GroupByNode,
-    ItemGroupbyNode,
-    ProjectNode,
-)
+from featurebyte.query_graph.node.generic import AliasNode, ProjectNode
 from featurebyte.schema.feature import (
     FeatureCreate,
     FeatureModelResponse,
     FeaturePreview,
     FeatureSQL,
     FeatureUpdate,
 )
 
 logger = get_logger(__name__)
 
 
 class Feature(
-    ProtectedColumnsQueryObject,
     Series,
-    FrozenFeatureModel,
     DeletableApiObject,
     SavableApiObject,
     CdAccessorMixin,
     FeatureJobMixin,
+    FeatureDtAccessorMixin,
+    FeatureStrAccessorMixin,
 ):  # pylint: disable=too-many-public-methods
     """
     A feature is input data that is used to train Machine Learning models and compute predictions.
 
     These features can sometimes be derived from attributes already present in the source tables. For instance, a
     customer churn model can use features obtained directly from a customer profile table, such as age, gender,
     income, and location.
@@ -103,14 +96,19 @@
     _list_fields = [
         "name",
         "version",
         *FEATURE_COMMON_LIST_FIELDS,
     ]
     _list_foreign_keys = FEATURE_LIST_FOREIGN_KEYS
 
+    # pydantic instance variable (internal use)
+    internal_catalog_id: PydanticObjectId = Field(
+        default_factory=get_active_catalog_id, alias="catalog_id"
+    )
+
     def _get_init_params_from_object(self) -> dict[str, Any]:
         return {"feature_store": self.feature_store}
 
     def _get_create_payload(self) -> dict[str, Any]:
         data = FeatureCreate(**self.json_dict())
         return data.json_dict()
 
@@ -124,18 +122,91 @@
         if "feature_store" not in values:
             tabular_source = values.get("tabular_source")
             if isinstance(tabular_source, dict):
                 feature_store_id = TabularSource(**tabular_source).feature_store_id
                 values["feature_store"] = FeatureStore.get_by_id(id=feature_store_id)
         return values
 
+    @property
+    def version(self) -> str:
+        """
+        Returns the version identifier of a Feature object.
+
+        Returns
+        -------
+        str
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("CustomerProductGroupCounts_7d")
+        >>> feature.version  # doctest: +SKIP
+        'V230323'
+        """
+        return cast(FeatureModel, self.cached_model).version.to_str()
+
+    @property
+    def catalog_id(self) -> ObjectId:
+        """
+        Returns the catalog ID that is associated with the Feature object.
+
+        Returns
+        -------
+        ObjectId
+            Catalog ID of the table.
+
+        See Also
+        --------
+        - [Catalog](/reference/featurebyte.api.catalog.Catalog)
+        """
+        try:
+            return cast(FeatureModel, self.cached_model).catalog_id
+        except RecordRetrievalException:
+            return self.internal_catalog_id
+
+    @property
+    def entity_ids(self) -> Sequence[ObjectId]:
+        """
+        Returns the entity IDs associated with the Feature object.
+
+        Returns
+        -------
+        Sequence[ObjectId]
+        """
+        try:
+            return cast(FeatureModel, self.cached_model).entity_ids
+        except RecordRetrievalException:
+            return self.graph.get_entity_ids(node_name=self.node_name)
+
+    @property
+    def table_ids(self) -> Sequence[ObjectId]:
+        """
+        Returns the table IDs used by the Feature object.
+
+        Returns
+        -------
+        Sequence[ObjectId]
+        """
+        try:
+            return cast(FeatureModel, self.cached_model).table_ids
+        except RecordRetrievalException:
+            return self.graph.get_table_ids(node_name=self.node_name)
+
+    @property
+    def feature_list_ids(self) -> Sequence[ObjectId]:
+        """
+        Returns the feature list IDs that use the Feature object.
+
+        Returns
+        -------
+        Sequence[ObjectId]
+        """
+        return cast(FeatureModel, self.cached_model).feature_list_ids
+
     @typechecked
-    def isin(  # pylint: disable=useless-parent-delegation
-        self: FrozenSeriesT, other: Union[FrozenSeries, ScalarSequence]
-    ) -> FrozenSeriesT:
+    def isin(self: FrozenSeriesT, other: Union[FrozenSeries, ScalarSequence]) -> FrozenSeriesT:
         """
         Identifies if each element is contained in a sequence of values represented by the `other` parameter.
 
         Parameters
         ----------
         other: Union[FrozenSeries, ScalarSequence]
             The sequence of values to check for membership. `other` can be a predefined list of values, or a Cross
@@ -155,17 +226,15 @@
         >>> lookup_feature = catalog.get_feature("ProductGroupLookup")
         >>> dictionary_feature = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = lookup_feature.isin(dictionary_feature)
         >>> new_feature.name = "CustomerHasProductGroup_7d"
         """
         return super().isin(other)  # type: ignore[no-any-return,misc]
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         Returns a dictionary that summarizes the essential information of an Feature object. The dictionary contains
         the following keys:
 
         - `created_at`: The timestamp indicating when the Feature object was created.
         - `name`: The name of the Feature object.
         - `updated_at`: The timestamp indicating when the Feature object was last updated.
@@ -196,14 +265,19 @@
         verbose: bool
             Control verbose level of the summary.
 
         Returns
         -------
         Dict[str, Any]
             Key-value mapping of properties of the object.
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
+        >>> feature.info()  # doctest: +SKIP
         """
         return super().info(verbose)
 
     @classmethod
     def get(cls, name: str, version: Optional[str] = None) -> Feature:
         """
         Retrieve the Feature from the persistent data store given the object's name, and version.
@@ -334,25 +408,33 @@
         pd.DataFrame
             Table of features with the same name
 
         Examples
         --------
         >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature.list_versions()  # doctest: +SKIP
-                name  version  dtype readiness  online_enabled             table    entities              created_at
-            0  sum_1d  V230323  FLOAT     DRAFT           False  [sf_event_table]  [customer] 2023-03-23 06:19:35.838
+                 name  version  dtype readiness  online_enabled             table    entities              created_at  is_default
+            0  sum_1d  V230323  FLOAT     DRAFT           False  [sf_event_table]  [customer] 2023-03-23 06:19:35.838        True
         """
-        return self._list(include_id=include_id, params={"name": self.name})
+        output = self._list(include_id=True, params={"name": self.name})
+        default_feature_id = self.feature_namespace.default_feature_id
+        output["is_default"] = output["id"] == default_feature_id
+        columns = output.columns
+        if not include_id:
+            columns = [column for column in columns if column != "id"]
+        return output[columns]
 
     def delete(self) -> None:
         """
-        Delete a feature. A feature can only be deleted if
-        * the feature readiness is DRAFT
-        * the feature is not used in any feature list
-        * the feature is not a default feature with manual version mode
+        Deletes a feature from the persistent data store. A feature can only be deleted from the persistent data
+        store if:
+
+        - the feature readiness is DRAFT
+        - the feature is not used in any feature list
+        - the feature is not a default feature with manual version mode
 
         Examples
         --------
         Delete a feature.
 
         >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature.delete()  # doctest: +SKIP
@@ -413,64 +495,24 @@
             node_output_type=NodeOutputType.SERIES,
             input_nodes=[node],
         )
         self.node_name = new_node.name
         return super().__setattr__(key, value)
 
     @property
-    def protected_attributes(self) -> List[str]:
-        """
-        List of protected attributes used to extract protected_columns
-
-        Returns
-        -------
-        List[str]
-        """
-        return ["entity_identifiers"]
-
-    @property
-    def entity_identifiers(self) -> List[str]:
-        """
-        Entity identifiers column names
-
-        Returns
-        -------
-        List[str]
-        """
-        entity_ids: list[str] = []
-        for node in self.graph.iterate_nodes(target_node=self.node, node_type=NodeType.GROUPBY):
-            entity_ids.extend(cast(GroupByNode, node).parameters.keys)
-        for node in self.graph.iterate_nodes(
-            target_node=self.node, node_type=NodeType.ITEM_GROUPBY
-        ):
-            entity_ids.extend(cast(ItemGroupbyNode, node).parameters.keys)
-        return entity_ids
-
-    @property
-    def inherited_columns(self) -> set[str]:
-        """
-        Special columns set which will be automatically added to the object of same class
-        derived from current object
-
-        Returns
-        -------
-        set[str]
-        """
-        return set(self.entity_identifiers)
-
-    @property
     def feature_namespace(self) -> FeatureNamespace:
         """
         FeatureNamespace object of current feature
 
         Returns
         -------
         FeatureNamespace
         """
-        return FeatureNamespace.get_by_id(id=self.feature_namespace_id)
+        feature_namespace_id = cast(FeatureModel, self.cached_model).feature_namespace_id
+        return FeatureNamespace.get_by_id(id=feature_namespace_id)
 
     @property
     def readiness(self) -> FeatureReadiness:
         """
         Returns the readiness level of the feature object.
 
         Returns
@@ -552,41 +594,41 @@
         We check for this by looking to see by looking at the operation structure to see if it's time-based.
 
         Returns
         -------
         bool
             True if the feature is time based, False otherwise.
         """
-        operation_structure = self.extract_operation_structure()
+        operation_structure = self.graph.extract_operation_structure(self.node)
         return operation_structure.is_time_based
 
     @property
-    def is_datetime(self) -> bool:  # pylint: disable=useless-parent-delegation
+    def is_datetime(self) -> bool:
         """
         Returns whether the feature has a datetime data type.
 
         Returns
         -------
         bool
         """
         return super().is_datetime
 
     @property
-    def is_numeric(self) -> bool:  # pylint: disable=useless-parent-delegation
+    def is_numeric(self) -> bool:
         """
         Returns whether the feature has a numeric data type.
 
         Returns
         -------
         bool
         """
         return super().is_numeric
 
     @property
-    def saved(self) -> bool:  # pylint: disable=useless-parent-delegation
+    def saved(self) -> bool:
         """
         Returns whether the Feature object is saved and part of the catalog.
 
         Returns
         -------
         bool
         """
@@ -601,19 +643,24 @@
         feature is declared in the SDK and is stored in the FeatureByte Service.
 
         This file uses the same SDK syntax as the feature declaration and provides an explicit outline of the intended
         operations of the feature declaration, including those that are inherited but not explicitly declared by the
         user. These operations may include feature job settings and cleaning operations inherited from tables metadata.
 
         The feature definition file serves as the basis for generating the final logical execution graph, which is
-        then transpiled into platform-specific SQL (e.g. SnowSQL, SparkSQL) for feature materialization."
+        then transpiled into platform-specific SQL (e.g. SnowSQL, SparkSQL) for feature materialization.
 
         Returns
         -------
         str
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
+        >>> feature_definition = feature.definition
         """
         try:
             definition = self.cached_model.definition
             assert definition is not None, "Saved feature's definition should not be None."
         except RecordRetrievalException:
             definition = self._generate_code(to_format=True, to_use_saved_data=True)
         return CodeStr(definition)
@@ -631,34 +678,47 @@
         entities = []
         for entity_id in self.entity_ids:
             entities.append(Entity.get_by_id(entity_id))
         primary_entity = derive_primary_entity(entities)  # type: ignore
         return primary_entity
 
     @typechecked
-    def save(  # pylint: disable=useless-parent-delegation
-        self, conflict_resolution: ConflictResolution = "raise"
+    def save(
+        self, conflict_resolution: ConflictResolution = "raise", _id: Optional[ObjectId] = None
     ) -> None:
         """
         Adds a Feature object to the catalog.
 
         A conflict could be triggered when the object being saved has violated a uniqueness check at the catalog.
         If uniqueness is violated, you can either raise an error or retrieve the object with the same name, depending
         on the conflict resolution parameter passed in. The default behavior is to raise an error.
 
         Parameters
         ----------
         conflict_resolution: ConflictResolution
             "raise" will raise an error when we encounter a conflict error.
             "retrieve" will handle the conflict error by retrieving the object with the same name.
+        _id: Optional[ObjectId]
+            The object ID to be used when saving the object. If not provided, a new object ID will be generated.
+
+        Examples
+        --------
+        >>> grocery_invoice_view = catalog.get_view("GROCERYINVOICE")
+        >>> invoice_amount_avg_60days = grocery_invoice_view.groupby("GroceryCustomerGuid").aggregate_over(
+        ...   value_column="Amount",
+        ...   method="avg",
+        ...   feature_names=["InvoiceAmountAvg_60days"],
+        ...   windows=["60d"],
+        ... )["InvoiceAmountAvg_60days"]
+        >>> invoice_amount_avg_60days.save()  # doctest: +SKIP
         """
-        super().save(conflict_resolution=conflict_resolution)
+        super().save(conflict_resolution=conflict_resolution, _id=_id)
 
     @typechecked
-    def astype(  # pylint: disable=useless-parent-delegation
+    def astype(
         self: FrozenSeriesT,
         new_type: Union[Type[int], Type[float], Type[str], Literal["int", "float", "str"]],
     ) -> FrozenSeriesT:
         """
         Modifies the data type of a feature. It is useful when you need to convert feature values between numerical
         and string formats, or the other way around.
 
@@ -667,14 +727,20 @@
         new_type : Union[Type[int], Type[float], Type[str], Literal["int", "float", "str"]])
             Desired type after conversion. Type can be provided directly, or as a string.
 
         Returns
         -------
         FrozenSeriesT
             A new Series with converted variable type.
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
+        >>> string_invoice_count_feature = feature.astype(str)
+        >>> float_invoice_count_feature = feature.astype(float)
         """
         return super().astype(new_type=new_type)  # type: ignore[no-any-return,misc]
 
     def binary_op_series_params(
         self, other: Scalar | FrozenSeries | ScalarSequence
     ) -> dict[str, Any]:
         """
@@ -1045,15 +1111,15 @@
         readiness level as the default. If several versions share the same readiness level, the most recent one
         becomes the default.
 
         Examples
         --------
 
         >>> feature = catalog.get_feature("InvoiceCount_60days")
-        >>> feature.update_default_version_mode(DefaultVersionMode.MANUAL)
+        >>> feature.update_default_version_mode(fb.DefaultVersionMode.MANUAL)
         >>> feature.as_default_version()
         """
         self.feature_namespace.update(
             update_payload={"default_feature_id": self.id},
             allow_update_local=False,
         )
         assert self.feature_namespace.default_feature_id == self.id
@@ -1099,12 +1165,44 @@
         Parameters
         ----------
         other: Union[FrozenSeries, Sequence[Union[bool, int, float, str]]]
             other
         """
         assert_is_lookup_feature(self.node_types_lineage)
 
+    def isnull(self) -> Feature:
+        """
+        Returns a boolean Feature indicating whether each element is missing.
+
+        Returns
+        -------
+        Feature
+            Feature with boolean values
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
+        >>> new_feature = feature.isnull()
+        """
+        return super().isnull()
+
+    def notnull(self) -> Feature:
+        """
+        Returns a boolean Feature indicating whether each element is not null.
+
+        Returns
+        -------
+        Feature
+            Feature with boolean values
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
+        >>> new_feature = feature.notnull()
+        """
+        return super().notnull()
+
     # descriptors
     list_versions: ClassVar[ClassInstanceMethodDescriptor] = ClassInstanceMethodDescriptor(
         class_method=_list_versions,
         instance_method=_list_versions_with_same_name,
     )
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_group.py` & `featurebyte-0.3.0/featurebyte/api/feature_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Feature group module.
 """
 
 from __future__ import annotations
 
-from typing import Any, List, Optional, OrderedDict, Sequence, Tuple, Union, cast
+from typing import Any, List, Optional, OrderedDict, Sequence, Set, Tuple, Union, cast
 
 import collections
 import time
 from http import HTTPStatus
 
 import pandas as pd
+from bson import ObjectId
 from pydantic import Field, parse_obj_as, root_validator
 from typeguard import typechecked
 
 from featurebyte.api.api_object import ConflictResolution
 from featurebyte.api.entity import Entity
 from featurebyte.api.feature import Feature
 from featurebyte.common.doc_util import FBAutoDoc
@@ -113,15 +114,15 @@
         Returns the primary entity of the FeatureList object.
 
         Returns
         -------
         List[Entity]
             Primary entity
         """
-        entity_ids = set()
+        entity_ids: Set[ObjectId] = set()
         for feature in self._features:
             entity_ids.update(feature.entity_ids)
         primary_entity = derive_primary_entity(  # type: ignore
             [Entity.get_by_id(entity_id) for entity_id in entity_ids]
         )
         return primary_entity
 
@@ -183,14 +184,22 @@
         items: List[str]
             List of feature names to be dropped
 
         Returns
         -------
         FeatureGroup
             FeatureGroup object containing remaining feature(s)
+
+        Examples
+        --------
+        >>> features = fb.FeatureGroup([
+        ...     catalog.get_feature("InvoiceCount_60days"),
+        ...     catalog.get_feature("InvoiceAmountAvg_60days"),
+        ... ])
+        >>> amount_feature_group = features.drop(["InvoiceCount_60days"])
         """
         selected_feat_names = [
             feat_name for feat_name in self.feature_objects if feat_name not in items
         ]
         return self._subset_list_of_columns(selected_feat_names)
 
     def _get_feature_clusters(self) -> List[FeatureCluster]:
@@ -375,10 +384,18 @@
         on the conflict resolution parameter passed in. The default behavior is to raise an error.
 
         Parameters
         ----------
         conflict_resolution: ConflictResolution
             "raise" raises error when then counters conflict error (default)
             "retrieve" handle conflict error by retrieving the object with the same name
+
+        Examples
+        --------
+        >>> features = fb.FeatureGroup([
+        ...     catalog.get_feature("InvoiceCount_60days"),
+        ...     catalog.get_feature("InvoiceAmountAvg_60days"),
+        ... ])
+        >>> features.save()  # doctest: +SKIP
         """
         for feature_name in self.feature_names:
             self[feature_name].save(conflict_resolution=conflict_resolution)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_job.py` & `featurebyte-0.3.0/featurebyte/api/feature_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,19 @@
         -------
         FeatureJobStatusResult
 
         Raises
         ------
         RecordRetrievalException
             Preview request failed
+
+        Examples
+        --------
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
+        >>> feature.get_feature_jobs_status()  # doctest: +SKIP
         """
         client = Configurations().get_client()
         response = client.get(
             url=f"{self._route}/{self.id}/feature_job_logs?hour_limit={job_history_window}"
         )
         if response.status_code != HTTPStatus.OK:
             raise RecordRetrievalException(response)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_job_setting_analysis.py` & `featurebyte-0.3.0/featurebyte/api/feature_job_setting_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,21 @@
 
 class FeatureJobSettingAnalysis(FeatureJobSettingAnalysisModel, ApiObject):
     """
     The FeatureJobSettingAnalysis object contains the result of the analysis of the data availability and freshness of
     a table. The metadata held by the object includes a report and recommendation for the configuration of the feature
     job setting of features associated with the table. Additionally, you can perform a backtest of a manually
     configured feature job setting.
+
+    Examples
+    --------
+    >>> analysis = invoice_table.create_new_feature_job_setting_analysis(  # doctest: +SKIP
+    ...   analysis_date=pd.Timestamp('2023-04-10'),
+    ...   analysis_length=3600*24*28,
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.FeatureJobSettingAnalysis")
 
     # class variables
     _route = "/feature_job_setting_analysis"
     _list_schema = FeatureJobSettingAnalysisRecord
@@ -95,14 +102,19 @@
             params = {"event_table_id": str(event_table_id)}
         return cls._list(include_id=include_id, params=params)
 
     @typechecked
     def display_report(self) -> None:
         """
         Displays analysis report.
+
+        Examples
+        --------
+        >>> analysis = fb.FeatureJobSettingAnalysis.get_by_id(<analysis_id>)  # doctest: +SKIP
+        >>> analysis.display_report()  # doctest: +SKIP
         """
         display_html_in_notebook(self.analysis_report)
 
     @typechecked
     def download_report(self, output_path: Optional[Union[str, Path]] = None) -> Path:
         """
         Downloads analysis report.
@@ -116,14 +128,19 @@
         -------
         Path
 
         Raises
         ------
         FileExistsError
             File already exists at output path
+
+        Examples
+        --------
+        >>> analysis = fb.FeatureJobSettingAnalysis.get_by_id(<analysis_id>)  # doctest: +SKIP
+        >>> analysis.download_report()  # doctest: +SKIP
         """
         client = Configurations().get_client()
         response = client.get(f"{self._route}/{self.id}/report")
         file_name = response.headers["content-disposition"].split("filename=")[1].replace('"', "")
         output_path = output_path or Path(f"./{file_name}")
         output_path = Path(output_path)
 
@@ -139,14 +156,19 @@
         """
         Retrieves recommended feature job setting from the analysis.
 
         Returns
         -------
         FeatureJobSetting
             Recommended feature job setting
+
+        Examples
+        --------
+        >>> analysis = fb.FeatureJobSettingAnalysis.get_by_id(<analysis_id>)  # doctest: +SKIP
+        >>> feature_job_setting = analysis.get_recommendation()  # doctest: +SKIP
         """
         info = self.info()
         return FeatureJobSetting(**info["recommendation"])
 
     @typechecked
     def backtest(self, feature_job_setting: FeatureJobSetting) -> pd.DataFrame:
         """
@@ -156,14 +178,25 @@
         ----------
         feature_job_setting: FeatureJobSetting
             FeatureJobSetting to backtest
 
         Returns
         -------
         pd.DataFrame
+
+        Examples
+        --------
+        >>> analysis = fb.FeatureJobSettingAnalysis.get_by_id(<analysis_id>)  # doctest: +SKIP
+        >>> # Backtest a manual setting
+        >>> manual_setting = fb.FeatureJobSetting(  # doctest: +SKIP
+        ...   blind_spot="135s",
+        ...   frequency="60m",
+        ...   time_modulo_frequency="90s",
+        ... )
+        >>> backtest_result = analysis.backtest(feature_job_setting=manual_setting)  # doctest: +SKIP
         """
         payload = FeatureJobSettingAnalysisBacktest(
             feature_job_setting_analysis_id=self.id,
             frequency=feature_job_setting.frequency_seconds,
             job_time_modulo_frequency=feature_job_setting.time_modulo_frequency_seconds,
             blind_spot=feature_job_setting.blind_spot_seconds,
         )
@@ -178,17 +211,15 @@
         response = client.get(f"{output_url}.html")
         display_html_in_notebook(response.text)
 
         # download and return table
         response = client.get(f"{output_url}.parquet")
         return pd.read_parquet(path=BytesIO(response.content))
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         The info method provides comprehensive details about a FeatureJobSettingAnalysis object, which encompasses:
 
         - the creation time of the analysis,
         - the table analyzed,
         - the analysis configuration,
         - recommended feature job setting, and
@@ -199,19 +230,24 @@
         verbose: bool
             Control verbose level of the summary.
 
         Returns
         -------
         Dict[str, Any]
             Key-value mapping of properties of the object.
+
+        Examples
+        --------
+        >>> analysis = fb.FeatureJobSettingAnalysis.get_by_id(<analysis_id>)  # doctest: +SKIP
+        >>> analysis.info()  # doctest: +SKIP
         """
         return super().info(verbose)
 
     @classmethod
-    def get_by_id(  # pylint: disable=useless-parent-delegation
+    def get_by_id(
         cls, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> FeatureJobSettingAnalysis:
         """
         Retrieves an analysis of the data availability and freshness of a table. This returns a
         FeatureJobSettingAnalysis object that allows to access the result of the analysis.
 
         Parameters
@@ -219,9 +255,13 @@
         id: ObjectId
             Analysis unique identifier ID.
 
         Returns
         -------
         FeatureJobSettingAnalysis
             FeatureJobSettingAnalysis object.
+
+        Examples
+        --------
+        >>> analysis = fb.FeatureJobSettingAnalysis.get_by_id(<analysis_id>)  # doctest: +SKIP
         """
         return cls._get_by_id(id=id)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_list.py` & `featurebyte-0.3.0/featurebyte/api/feature_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,73 +18,71 @@
     Union,
     cast,
 )
 
 import collections
 from http import HTTPStatus
 
-import numpy as np
 import pandas as pd
 from alive_progress import alive_bar
 from bson.objectid import ObjectId
 from pydantic import Field, root_validator
 from typeguard import typechecked
 
 from featurebyte.api.api_object import (
     PAGINATED_CALL_PAGE_SIZE,
     ApiObject,
     ConflictResolution,
-    DeletableApiObject,
     ForeignKeyMapping,
-    SavableApiObject,
 )
 from featurebyte.api.base_table import TableApiObject
 from featurebyte.api.entity import Entity
 from featurebyte.api.feature import Feature
 from featurebyte.api.feature_group import BaseFeatureGroup, FeatureGroup
 from featurebyte.api.feature_job import FeatureJobMixin, FeatureJobStatusResult
 from featurebyte.api.feature_store import FeatureStore
 from featurebyte.api.historical_feature_table import HistoricalFeatureTable
 from featurebyte.api.observation_table import ObservationTable
+from featurebyte.api.savable_api_object import DeletableApiObject, SavableApiObject
 from featurebyte.common.descriptor import ClassInstanceMethodDescriptor
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.env_util import get_alive_bar_additional_params
-from featurebyte.common.model_util import get_version
 from featurebyte.common.utils import (
-    dataframe_from_arrow_stream,
+    convert_to_list_of_strings,
     dataframe_to_arrow_bytes,
     enforce_observation_set_row_order,
 )
 from featurebyte.config import Configurations
 from featurebyte.exception import (
     DuplicatedRecordException,
     RecordCreationException,
     RecordRetrievalException,
 )
 from featurebyte.feature_manager.model import ExtendedFeatureModel
-from featurebyte.models.base import PydanticObjectId, VersionIdentifier
+from featurebyte.models.base import PydanticObjectId, VersionIdentifier, get_active_catalog_id
 from featurebyte.models.feature import DefaultVersionMode
 from featurebyte.models.feature_list import (
     FeatureListModel,
-    FeatureListNamespaceModel,
     FeatureListStatus,
     FeatureReadinessDistribution,
-    FrozenFeatureListModel,
     FrozenFeatureListNamespaceModel,
 )
 from featurebyte.models.tile import TileSpec
 from featurebyte.query_graph.model.common_table import TabularSource
 from featurebyte.schema.deployment import DeploymentCreate
 from featurebyte.schema.feature_list import (
     FeatureListCreate,
     FeatureListGetHistoricalFeatures,
     FeatureListUpdate,
     FeatureVersionInfo,
 )
-from featurebyte.schema.feature_list_namespace import FeatureListNamespaceUpdate
+from featurebyte.schema.feature_list_namespace import (
+    FeatureListNamespaceModelResponse,
+    FeatureListNamespaceUpdate,
+)
 from featurebyte.schema.historical_feature_table import HistoricalFeatureTableCreate
 
 if TYPE_CHECKING:
     from featurebyte.api.deployment import Deployment
 else:
     Deployment = TypeVar("Deployment")
 
@@ -108,30 +106,32 @@
     feature_list_namespace will not change.
     """
 
     # class variable
     _route = "/feature_list_namespace"
     _update_schema_class = FeatureListNamespaceUpdate
 
-    _list_schema = FeatureListNamespaceModel
-    _get_schema = FeatureListNamespaceModel
+    _list_schema = FeatureListNamespaceModelResponse
+    _get_schema = FeatureListNamespaceModelResponse
     _list_fields = [
         "name",
         "num_feature",
         "status",
         "deployed",
         "readiness_frac",
         "online_frac",
         "tables",
         "entities",
+        "primary_entities",
         "created_at",
     ]
     _list_foreign_keys = [
         ForeignKeyMapping("entity_ids", Entity, "entities"),
         ForeignKeyMapping("table_ids", TableApiObject, "tables"),
+        ForeignKeyMapping("primary_entity_ids", Entity, "primary_entities"),
     ]
 
     @property
     def feature_list_ids(self) -> List[PydanticObjectId]:
         """
         List of feature list IDs from the same feature list namespace
 
@@ -189,14 +189,20 @@
     def status(self) -> FeatureListStatus:
         """
         Feature list status
 
         Returns
         -------
         FeatureListStatus
+
+        Examples
+        --------
+        >>> feature_list = catalog.get_feature_list("invoice_feature_list")
+        >>> feature_list.status
+        'TEMPLATE'
         """
         return self.cached_model.status
 
     @classmethod
     def _post_process_list(cls, item_list: pd.DataFrame) -> pd.DataFrame:
         feature_lists = super()._post_process_list(item_list)
 
@@ -220,50 +226,59 @@
         )
         return feature_lists
 
     @classmethod
     def list(
         cls,
         include_id: Optional[bool] = False,
+        primary_entity: Optional[Union[str, List[str]]] = None,
         entity: Optional[str] = None,
         table: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         List saved feature lists
 
         Parameters
         ----------
         include_id: Optional[bool]
             Whether to include id in the list
+        primary_entity: Optional[Union[str, List[str]]]
+            Name of entity used to filter results. If multiple entities are provided, the filtered results will
+            contain feature lists that are associated with all the entities.
         entity: Optional[str]
             Name of entity used to filter results
         table: Optional[str]
             Name of table used to filter results
 
         Returns
         -------
         pd.DataFrame
             Table of feature lists
         """
         feature_lists = super().list(include_id=include_id)
+        target_entities = convert_to_list_of_strings(primary_entity)
+        if target_entities:
+            feature_lists = feature_lists[
+                feature_lists.primary_entities.apply(
+                    lambda primary_entities: set(target_entities).issubset(primary_entities)
+                )
+            ]
         if entity:
             feature_lists = feature_lists[
                 feature_lists.entities.apply(lambda entities: entity in entities)
             ]
         if table:
             feature_lists = feature_lists[
                 feature_lists.tables.apply(lambda table_list: table in table_list)
             ]
         return feature_lists
 
 
 # pylint: disable=too-many-public-methods
-class FeatureList(
-    BaseFeatureGroup, FrozenFeatureListModel, DeletableApiObject, SavableApiObject, FeatureJobMixin
-):
+class FeatureList(BaseFeatureGroup, DeletableApiObject, SavableApiObject, FeatureJobMixin):
     """
     The FeatureList class is used as a constructor to create a FeatureList Object.
 
     A FeatureList object is added to the catalog only when explicitly saved.
 
     A Feature List is a collection of Feature Objects specifically designed to address a particular Use Case. The
     Feature List is initially used to gather historical feature values for EDA, training, or testing data for a Use
@@ -276,62 +291,153 @@
     based on the relationships between the entities, with the lowest-level entity chosen as the primary entity. If
     there are no relationships between entities, the primary entity may become a tuple comprising those entities.
 
     For example, imagine a feature list that includes features related to a card, customer, and customer city. In
     this scenario, the primary entity is the card entity because it is a child of both the customer and customer
     city entities. However, if the feature list also contains features for a merchant and merchant city, the primary
     entity becomes a tuple of card and merchant.
+
+    Examples
+    --------
+    Create a feature list with two features.
+
+    >>> features = fb.FeatureList([
+    ...   catalog.get_feature("InvoiceCount_60days"),
+    ...   catalog.get_feature("InvoiceAmountAvg_60days"),
+    ... ], name="My new feature list")
     """
 
     # documentation metadata
     __fbautodoc__ = FBAutoDoc(
         proxy_class="featurebyte.FeatureList",
         hide_keyword_only_params_in_class_docs=True,
     )
 
-    # override FeatureListModel attributes
-    feature_ids: List[PydanticObjectId] = Field(
-        default_factory=list,
-        allow_mutation=False,
-        description="Returns the unique identifier (ID) of the Feature objects associated with the FeatureList object.",
-    )
-    version: VersionIdentifier = Field(
-        allow_mutation=False,
-        default=None,
-        description="Returns the version identifier of a FeatureList object.",
-    )
-
     # class variables
     _route = "/feature_list"
     _update_schema_class = FeatureListUpdate
     _list_schema = FeatureListModel
     _get_schema = FeatureListModel
     _list_fields = [
         "name",
         "version",
-        "feature_list_namespace_id",
         "num_feature",
         "online_frac",
         "deployed",
         "created_at",
     ]
 
+    # pydantic instance variable (internal use)
+    internal_catalog_id: PydanticObjectId = Field(
+        default_factory=get_active_catalog_id, alias="catalog_id"
+    )
+    internal_feature_ids: List[PydanticObjectId] = Field(alias="feature_ids", default_factory=list)
+
+    @root_validator(pre=True)
+    @classmethod
+    def _initialize_feature_objects_and_items(cls, values: dict[str, Any]) -> dict[str, Any]:
+        if "feature_ids" in values:
+            # FeatureList object constructed in SDK will not have feature_ids attribute,
+            # only the record retrieved from the persistent contains this attribute.
+            # Use this check to decide whether to make API call to retrieve features.
+            items = []
+            feature_objects = collections.OrderedDict()
+            id_value = values["_id"]
+            feature_store_map: Dict[ObjectId, FeatureStore] = {}
+            with alive_bar(
+                total=len(values["feature_ids"]),
+                title="Loading Feature(s)",
+                **get_alive_bar_additional_params(),
+            ) as progress_bar:
+                for feature_dict in cls.iterate_api_object_using_paginated_routes(
+                    route="/feature",
+                    params={"feature_list_id": id_value, "page_size": PAGINATED_CALL_PAGE_SIZE},
+                ):
+                    # store the feature store retrieve result to reuse it if same feature store are called again
+                    feature_store_id = TabularSource(
+                        **feature_dict["tabular_source"]
+                    ).feature_store_id
+                    if feature_store_id not in feature_store_map:
+                        feature_store_map[feature_store_id] = FeatureStore.get_by_id(
+                            feature_store_id
+                        )
+                    feature_dict["feature_store"] = feature_store_map[feature_store_id]
+
+                    # deserialize feature record into feature object
+                    feature = Feature.from_persistent_object_dict(object_dict=feature_dict)
+                    items.append(feature)
+                    feature_objects[feature.name] = feature
+                    progress_bar.text = feature.name
+                    progress_bar()  # pylint: disable=not-callable
+
+            values["items"] = items
+            values["feature_objects"] = feature_objects
+        return values
+
+    @root_validator
+    @classmethod
+    def _initialize_feature_list_parameters(cls, values: dict[str, Any]) -> dict[str, Any]:
+        # set the following values if it is empty (used mainly by the SDK constructed feature list)
+        # for the feature list constructed during serialization, following codes should be skipped
+        features = list(values["feature_objects"].values())
+        values["internal_feature_ids"] = [feature.id for feature in features]
+        return values
+
+    @typechecked
+    def __init__(self, items: Sequence[Union[Feature, BaseFeatureGroup]], name: str, **kwargs: Any):
+        super().__init__(items=items, name=name, **kwargs)
+
+    @property
+    def version(self) -> str:
+        """
+        Returns the version identifier of a FeatureList object.
+
+        Returns
+        -------
+        str
+
+        Examples
+        --------
+        >>> feature_list = catalog.get_feature_list("invoice_feature_list")
+        >>> feature_list.version  # doctest: +SKIP
+        'V230330'
+        """
+        return cast(FeatureListModel, self.cached_model).version.to_str()
+
+    @property
+    def catalog_id(self) -> ObjectId:
+        """
+        Returns the catalog ID that is associated with the FeatureList object.
+
+        Returns
+        -------
+        ObjectId
+            Catalog ID of the feature list.
+        See Also
+        --------
+        - [Catalog](/reference/featurebyte.api.catalog.Catalog)
+        """
+        try:
+            return cast(FeatureListModel, self.cached_model).catalog_id
+        except RecordRetrievalException:
+            return self.internal_catalog_id
+
     def _get_init_params_from_object(self) -> dict[str, Any]:
         return {"items": self.items}
 
     def _get_feature_tiles_specs(self) -> List[Tuple[str, List[TileSpec]]]:
         feature_tile_specs = []
         for feature in self.feature_objects.values():
             tile_specs = ExtendedFeatureModel(**feature.dict()).tile_specs
             if tile_specs:
                 feature_tile_specs.append((str(feature.name), tile_specs))
         return feature_tile_specs
 
     @typechecked
-    def get_feature_jobs_status(  # pylint: disable=useless-parent-delegation
+    def get_feature_jobs_status(
         self,
         job_history_window: int = 1,
         job_duration_tolerance: int = 60,
     ) -> FeatureJobStatusResult:
         """
         Returns a report on the recent activity of scheduled feature jobs associated with a FeatureList object.
 
@@ -349,22 +455,25 @@
             History window in hours.
         job_duration_tolerance: int
             Maximum duration before job is considered later, in seconds.
 
         Returns
         -------
         FeatureJobStatusResult
+
+        Examples
+        --------
+        >>> feature_list = catalog.get_feature_list("invoice_feature_list")
+        >>> feature_list.get_feature_jobs_status()  # doctest: +SKIP
         """
         return super().get_feature_jobs_status(
             job_history_window=job_history_window, job_duration_tolerance=job_duration_tolerance
         )
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         Returns a dictionary that summarizes the essential information of an FeatureList object. The dictionary
         contains the following keys:
 
         - `name`: The name of the FeatureList object.
         - `created_at`: The timestamp indicating when the FeatureList object was created.
         - `updated_at`: The timestamp indicating when the FeatureList object was last updated.
@@ -381,26 +490,89 @@
         - `serving_endpoint`: The URL for a deployed FeatureList for online serving of features.
 
         Some information is provided for both the FeatureList object and the default version with the same feature
         list namespace:
 
         - `version`: The version name.
         - `production_ready_fraction`: The percentage of features that are production-ready.
+        - `default_feature_fraction`: The percentage of features that are default features.
 
         This method is only available for FeatureList objects that are saved in the catalog.
 
         Parameters
         ----------
         verbose: bool
             Control verbose level of the summary.
 
         Returns
         -------
         Dict[str, Any]
             Key-value mapping of properties of the object.
+
+        Examples
+        --------
+        >>> feature_list = catalog.get_feature_list("invoice_feature_list")
+        >>> info = feature_list.info()
+        >>> del info["created_at"]
+        >>> del info["updated_at"]
+        >>> info  # doctest: +ELLIPSIS
+        {
+          'name': 'invoice_feature_list',
+          'entities': [
+            {
+              'name': 'grocerycustomer',
+              'serving_names': [
+                'GROCERYCUSTOMERGUID'
+              ],
+              'catalog_name': 'grocery'
+            }
+          ],
+          'primary_entity': [
+            {
+              'name': 'grocerycustomer',
+              'serving_names': [
+                'GROCERYCUSTOMERGUID'
+              ],
+              'catalog_name': 'grocery'
+            }
+          ],
+          'tables': [
+            {
+              'name': 'GROCERYINVOICE',
+              'status': 'PUBLIC_DRAFT',
+              'catalog_name': 'grocery'
+            }
+          ],
+          'default_version_mode': 'AUTO',
+          'version_count': 3,
+          'catalog_name': 'grocery',
+          'dtype_distribution': [
+            {
+              'dtype': 'FLOAT',
+              'count': 1
+            }
+          ],
+          'default_feature_list_id': ...,
+          'status': 'DRAFT',
+          'feature_count': 1,
+          'version': {
+            'this': ...,
+            'default': ...
+          },
+          'production_ready_fraction': {
+            'this': 1.0,
+            'default': 1.0
+          },
+          'default_feature_fraction': {
+            'this': 1.0,
+            'default': 1.0
+          },
+          'versions_info': None,
+          'deployed': False
+        }
         """
         return super().info(verbose)
 
     @property
     def feature_names(self) -> list[str]:
         """
         Returns a report on the recent activity of scheduled feature jobs associated with a FeatureList object.
@@ -426,14 +598,28 @@
 
         See Also
         --------
         - [FeatureGroup.feature_names](/reference/featurebyte.api.feature_group.FeatureGroup.feature_names/)
         """
         return super().feature_names
 
+    @property
+    def feature_ids(self) -> Sequence[ObjectId]:
+        """
+        Returns the unique identifier (ID) of the Feature objects associated with the FeatureList object.
+
+        Returns
+        -------
+        Sequence[ObjectId]
+        """
+        try:
+            return cast(FeatureListModel, self.cached_model).feature_ids
+        except RecordRetrievalException:
+            return self.internal_feature_ids
+
     @classmethod
     def _get_init_params(cls) -> dict[str, Any]:
         return {"items": []}
 
     @classmethod
     def get(cls, name: str, version: Optional[str] = None) -> FeatureList:
         """
@@ -484,88 +670,108 @@
                     self.feature_objects[feat_name].save(conflict_resolution=conflict_resolution)
                     text = f'Feature "{feat_name}" is saved.'
 
                 # update progress bar
                 progress_bar.text = text
                 progress_bar()  # pylint: disable=not-callable
 
-    def save(self, conflict_resolution: ConflictResolution = "raise") -> None:
+    def save(
+        self, conflict_resolution: ConflictResolution = "raise", _id: Optional[ObjectId] = None
+    ) -> None:
         """
         Adds a FeatureList object to the catalog.
 
         A conflict could be triggered when the object being saved has violated a uniqueness check at the catalog.
         If uniqueness is violated, you can either raise an error or retrieve the object with the same name, depending
         on the conflict resolution parameter passed in. The default behavior is to raise an error.
 
         Parameters
         ----------
         conflict_resolution: ConflictResolution
             "raise" raises error when we encounter a conflict error (default).
             "retrieve" handle conflict error by retrieving the object with the same name.
+        _id: Optional[ObjectId]
+            The object ID to be used when saving the object. If not provided, a new object ID will be generated.
 
         Raises
         ------
         DuplicatedRecordException
             When a record with the same key exists at the persistent data store.
+
+        Examples
+        --------
+        >>> feature_list = fb.FeatureList([
+        ...     catalog.get_feature("InvoiceCount_60days"),
+        ...     catalog.get_feature("InvoiceAmountAvg_60days"),
+        ... ], name="feature_lists_invoice_features")
+        >>> feature_list.save()  # doctest: +SKIP
         """
         try:
             super().save(conflict_resolution=conflict_resolution)
         except DuplicatedRecordException as exc:
             if conflict_resolution == "raise":
                 raise DuplicatedRecordException(
                     exc.response,
                     resolution=' Or try `feature_list.save(conflict_resolution = "retrieve")` to resolve conflict.',
                 ) from exc
             raise exc
 
     def delete(self) -> None:
         """
-        Delete a FeatureList object from the persistent data store. A feature list can only be deleted if
-        * the feature list status is DRAFT
-        * the feature list is not a default feature list with manual version mode
+        Deletes a FeatureList object from the persistent data store. A feature list can only be deleted from the
+        persistent data store if:
+
+        - the feature list status is DRAFT
+        - the feature list is not a default feature list with manual version mode
 
         Examples
         --------
-        Delete a FeatureList.
-
         >>> feature_list = catalog.get_feature_list("invoice_feature_list")
         >>> feature_list.delete()  # doctest: +SKIP
         """
         self._delete()
 
     @typechecked
-    def drop(self, items: List[str]) -> FeatureGroup:  # pylint: disable=useless-parent-delegation
+    def drop(self, items: List[str]) -> FeatureGroup:
         """
         Drops feature(s) from the original FeatureList and returns a new FeatureGroup object.
 
         Parameters
         ----------
         items: List[str]
             List of feature names to be dropped
 
         Returns
         -------
         FeatureGroup
             FeatureGroup object containing remaining feature(s)
+
+        Examples
+        --------
+        >>> feature_list = fb.FeatureList([
+        ...     catalog.get_feature("InvoiceCount_60days"),
+        ...     catalog.get_feature("InvoiceAmountAvg_60days"),
+        ... ], name="feature_lists_invoice_features")
+        >>> amount_only_feature_list = feature_list.drop(["InvoiceCount_60days"])
         """
         return super().drop(items=items)
 
     @property
-    def saved(self) -> bool:  # pylint: disable=useless-parent-delegation
+    def saved(self) -> bool:
         """
         Returns whether the FeatureList object is saved and added to the catalog.
 
         Returns
         -------
         bool
         """
         return super().saved
 
     @typechecked
-    def preview(  # pylint: disable=useless-parent-delegation
+    def preview(
         self,
         observation_set: pd.DataFrame,
     ) -> Optional[pd.DataFrame]:
         """
         Materializes a FeatureList using a small observation set of up to 50 rows. Unlike compute_historical_features,
         this method does not store partial aggregations (tiles) to speed up future computation. Instead, it computes
         the features on the fly, and should be used only for small observation sets for debugging or prototyping
@@ -585,84 +791,58 @@
         Returns
         -------
         pd.DataFrame
             Materialized feature values.
             The returned DataFrame will have the same number of rows, and include all columns from the observation set.
 
             **Note**: `POINT_IN_TIME` values will be converted to UTC time.
-        """
-        return super().preview(observation_set=observation_set)
 
-    @root_validator(pre=True)
-    @classmethod
-    def _initialize_feature_objects_and_items(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if "feature_ids" in values:
-            # FeatureList object constructed in SDK will not have feature_ids attribute,
-            # only the record retrieved from the persistent contains this attribute.
-            # Use this check to decide whether to make API call to retrieve features.
-            items = []
-            feature_objects = collections.OrderedDict()
-            id_value = values["_id"]
-            feature_store_map: Dict[ObjectId, FeatureStore] = {}
-            with alive_bar(
-                total=len(values["feature_ids"]),
-                title="Loading Feature(s)",
-                **get_alive_bar_additional_params(),
-            ) as progress_bar:
-                for feature_dict in cls.iterate_api_object_using_paginated_routes(
-                    route="/feature",
-                    params={"feature_list_id": id_value, "page_size": PAGINATED_CALL_PAGE_SIZE},
-                ):
-                    # store the feature store retrieve result to reuse it if same feature store are called again
-                    feature_store_id = TabularSource(
-                        **feature_dict["tabular_source"]
-                    ).feature_store_id
-                    if feature_store_id not in feature_store_map:
-                        feature_store_map[feature_store_id] = FeatureStore.get_by_id(
-                            feature_store_id
-                        )
-                    feature_dict["feature_store"] = feature_store_map[feature_store_id]
+        Examples
+        --------
+        Create a feature list with two features.
 
-                    # deserialize feature record into feature object
-                    feature = Feature.from_persistent_object_dict(object_dict=feature_dict)
-                    items.append(feature)
-                    feature_objects[feature.name] = feature
-                    progress_bar.text = feature.name
-                    progress_bar()  # pylint: disable=not-callable
+        >>> features = fb.FeatureList([
+        ...    catalog.get_feature("InvoiceCount_60days"),
+        ...    catalog.get_feature("InvoiceAmountAvg_60days"),
+        ... ], name="My new feature list")
 
-            values["items"] = items
-            values["feature_objects"] = feature_objects
-        return values
 
-    @root_validator
-    @classmethod
-    def _initialize_feature_list_parameters(cls, values: dict[str, Any]) -> dict[str, Any]:
-        # set the following values if it is empty (used mainly by the SDK constructed feature list)
-        # for the feature list constructed during serialization, following codes should be skipped
-        features = list(values["feature_objects"].values())
-        if not values.get("feature_ids"):
-            values["feature_ids"] = [feature.id for feature in features]
-        if not values.get("version"):
-            values["version"] = get_version()
-        return values
+        Prepare observation set with POINT_IN_TIME and serving names columns.
+
+        >>> observation_set = pd.DataFrame({
+        ...    "POINT_IN_TIME": ["2022-06-01 00:00:00", "2022-06-02 00:00:00"],
+        ...    "GROCERYCUSTOMERGUID": [
+        ...      "a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3",
+        ...      "ac479f28-e0ff-41a4-8e60-8678e670e80b",
+        ...    ],
+        ... })
 
-    @typechecked
-    def __init__(self, items: Sequence[Union[Feature, BaseFeatureGroup]], name: str, **kwargs: Any):
-        super().__init__(items=items, name=name, **kwargs)
+
+        Preview the feature list with a small observation set.
+
+        >>> features.preview(observation_set)
+            POINT_IN_TIME  GROCERYCUSTOMERGUID                   InvoiceCount_60days  InvoiceAmountAvg_60days
+        0   2022-06-01     a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3  10.0                 7.938
+        1   2022-06-02     ac479f28-e0ff-41a4-8e60-8678e670e80b  6.0                  9.870
+        """
+        return super().preview(observation_set=observation_set)
 
     @property
     def feature_list_namespace(self) -> FeatureListNamespace:
         """
         FeatureListNamespace object of current feature list
 
         Returns
         -------
         FeatureListNamespace
         """
-        return FeatureListNamespace.get_by_id(id=self.feature_list_namespace_id)
+        feature_list_namespace_id = cast(
+            FeatureListModel, self.cached_model
+        ).feature_list_namespace_id
+        return FeatureListNamespace.get_by_id(id=feature_list_namespace_id)
 
     @property
     def online_enabled_feature_ids(self) -> List[PydanticObjectId]:
         """
         List of online enabled feature IDs of this feature list
 
         Returns
@@ -684,28 +864,57 @@
         Returns
         -------
         FeatureReadinessDistribution
         """
         try:
             return self.cached_model.readiness_distribution
         except RecordRetrievalException:
-            return self.derive_readiness_distribution(list(self.feature_objects.values()))  # type: ignore
+            return FeatureListModel.derive_readiness_distribution(
+                list(self.feature_objects.values())  # type: ignore
+            )
 
     @property
     def production_ready_fraction(self) -> float:
         """
         Retrieve fraction of production ready features in the feature list
 
         Returns
         -------
         Fraction of production ready feature
+
+        See Also
+        --------
+        - [FeatureList.info](/reference/featurebyte.api.feature_list.FeatureList.info/)
         """
         return self.readiness_distribution.derive_production_ready_fraction()
 
     @property
+    def default_feature_fraction(self) -> float:
+        """
+        Retrieve fraction of default features in the feature list
+
+        Returns
+        -------
+        Fraction of default feature
+
+        See Also
+        --------
+        - [Feature.info](/reference/featurebyte.api.feature.Feature.info/)
+        - [Feature.is_default](/reference/featurebyte.api.feature.Feature.is_default/)
+        - [FeatureList.info](/reference/featurebyte.api.feature_list.FeatureList.info/)
+        """
+        namespace_info = self.feature_list_namespace.info()
+        default_feat_ids = set(namespace_info["default_feature_ids"])
+        default_feat_count = 0
+        for feat_id in self.feature_ids:
+            if str(feat_id) in default_feat_ids:
+                default_feat_count += 1
+        return default_feat_count / len(self.feature_ids)
+
+    @property
     def deployed(self) -> bool:
         """
         Whether this feature list is deployed or not
 
         Returns
         -------
         bool
@@ -779,23 +988,23 @@
             Table of feature lists
 
         Examples
         --------
         List saved FeatureList versions (calling from FeatureList class):
 
         >>> FeatureList.list_versions()  # doctest: +SKIP
-                           name feature_list_namespace_id  num_feature  online_frac  deployed              created_at
-        0  invoice_feature_list  641d2f94f8d79eb6fee0a335            1          0.0     False 2023-03-24 05:05:24.875
+                           name  num_feature  online_frac  deployed              created_at
+        0  invoice_feature_list            1          0.0     False 2023-03-24 05:05:24.875
 
         List FeatureList versions with the same name (calling from FeatureList object):
 
         >>> feature_list = catalog.get_feature_list("invoice_feature_list") # doctest: +SKIP
         >>> feature_list.list_versions()  # doctest: +SKIP
-                           name feature_list_namespace_id  num_feature  online_frac  deployed              created_at
-        0  invoice_feature_list  641d02af94ede33779acc6c8            1          0.0     False 2023-03-24 01:53:51.515
+                           name  num_feature  online_frac  deployed              created_at
+        0  invoice_feature_list            1          0.0     False 2023-03-24 01:53:51.515
 
         See Also
         --------
         - [FeatureList.list_features](/reference/featurebyte.api.feature_list.FeatureList.list_features/)
         """
         return super().list(include_id=include_id)
 
@@ -813,44 +1022,56 @@
         pd.DataFrame
             Table of features with the same name
 
         Examples
         --------
         >>> feature_list = catalog.get_feature_list("invoice_feature_list")
         >>> feature_list.list_versions()  # doctest: +SKIP
-                           name feature_list_namespace_id  num_feature  online_frac  deployed              created_at
-        0  invoice_feature_list  641d02af94ede33779acc6c8            1          0.0     False 2023-03-24 01:53:51.515
+                           name  online_frac  deployed              created_at  is_default
+        0  invoice_feature_list          0.0     False 2023-03-24 01:53:51.515        True
         """
-        return self._list(include_id=include_id, params={"name": self.name})
+        output = self._list(include_id=True, params={"name": self.name})
+        default_feature_list_id = self.feature_list_namespace.default_feature_list_id
+        output["is_default"] = output["id"] == default_feature_list_id
+        exclude_cols = {"num_feature"}
+        if not include_id:
+            exclude_cols.add("id")
+        return output[[col for col in output.columns if col not in exclude_cols]]
 
     @classmethod
     def list(
         cls,
         include_id: Optional[bool] = False,
+        primary_entity: Optional[Union[str, List[str]]] = None,
         entity: Optional[str] = None,
         table: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         List saved feature lists
 
         Parameters
         ----------
         include_id: Optional[bool]
             Whether to include id in the list
+        primary_entity: Optional[Union[str, List[str]]] = None,
+            Name of entity used to filter results. If multiple entities are provided, the filtered results will
+            contain feature lists that are associated with all the entities.
         entity: Optional[str]
             Name of entity used to filter results
         table: Optional[str]
             Name of table used to filter results
 
         Returns
         -------
         pd.DataFrame
             Table of feature lists
         """
-        return FeatureListNamespace.list(include_id=include_id, entity=entity, table=table)
+        return FeatureListNamespace.list(
+            include_id=include_id, primary_entity=primary_entity, entity=entity, table=table
+        )
 
     def list_features(self) -> pd.DataFrame:
         """
         Returns a DataFrame that contains various attributes of the features in a Feature List object, such as their
         names, versions, types, corresponding tables, related entities, creation dates, states of readiness and
         online availability.
 
@@ -924,16 +1145,15 @@
 
     @enforce_observation_set_row_order
     @typechecked
     def compute_historical_features(
         self,
         observation_set: pd.DataFrame,
         serving_names_mapping: Optional[Dict[str, str]] = None,
-        max_batch_size: int = 5000,
-    ) -> Optional[pd.DataFrame]:
+    ) -> pd.DataFrame:
         """
         Returns a DataFrame with feature values for analysis, model training, or evaluation. The historical features
         request data consists of an observation set that combines historical points-in-time and key values of the
         primary entity from the feature list.
 
         Associated serving entities can also be utilized.
 
@@ -958,29 +1178,22 @@
             Observation set DataFrame or ObservationTable object, which combines historical points-in-time and values
             of the feature primary entity or its descendant (serving entities). The column containing the point-in-time
             values should be named `POINT_IN_TIME`, while the columns representing entity values should be named using
             accepted serving names for the entity.
         serving_names_mapping : Optional[Dict[str, str]]
             Optional serving names mapping if the training events table has different serving name columns than those
             defined in Entities, mapping from original serving name to new name.
-        max_batch_size: int
-            Maximum number of rows per batch.
 
         Returns
         -------
         pd.DataFrame
             Materialized historical features.
 
             **Note**: `POINT_IN_TIME` values will be converted to UTC time.
 
-        Raises
-        ------
-        RecordRetrievalException
-            Get historical features request failed.
-
         Examples
         --------
         Create a feature list with two features.
         >>> feature_list = fb.FeatureList([
         ...     catalog.get_feature("InvoiceCount_60days"),
         ...     catalog.get_feature("InvoiceAmountAvg_60days"),
         ... ], name="InvoiceFeatures")
@@ -999,55 +1212,38 @@
         2    2022-04-19  a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3                  9.0                10.223333
         3    2022-04-21  a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3                 10.0                 9.799000
         4    2022-04-23  a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3                 10.0                 9.799000
         5    2022-04-25  a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3                  9.0                 9.034444
         6    2022-04-27  a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3                 10.0                 9.715000
         7    2022-04-29  a2828c3b-036c-4e2e-9bd6-30c9ee9a20e3                 10.0                 9.715000
 
+
+        Retrieve materialized historical features with serving names mapping.
+        >>> historical_features = feature_list.compute_historical_features(  # doctest: +SKIP
+        ...   observation_set=observation_set,
+        ...   serving_names_mapping={"GROCERYCUSTOMERGUID": "CUSTOMERGUID"}
+        ... )
+
         See Also
         --------
         - [FeatureGroup.preview](/reference/featurebyte.api.feature_group.FeatureGroup.preview/):
           Preview feature group.
         - [Feature.preview](/reference/featurebyte.api.feature.Feature.preview/):
           Preview feature group.
         """
-        payload = FeatureListGetHistoricalFeatures(
-            feature_list_id=self.id,
-            feature_clusters=self._get_feature_clusters(),
+        temp_historical_feature_table_name = f"__TEMPORARY_HISTORICAL_FEATURE_TABLE_{ObjectId()}"
+        temp_historical_feature_table = self.compute_historical_feature_table(
+            observation_table=observation_set,
+            historical_feature_table_name=temp_historical_feature_table_name,
             serving_names_mapping=serving_names_mapping,
         )
-
-        client = Configurations().get_client()
-        output = []
-        with alive_bar(
-            total=int(np.ceil(len(observation_set) / max_batch_size)),
-            title="Retrieving Historical Feature(s)",
-            **get_alive_bar_additional_params(),
-        ) as progress_bar:
-            for _, batch in observation_set.groupby(
-                np.arange(len(observation_set)) // max_batch_size
-            ):
-                response = client.post(
-                    "/feature_list/historical_features",
-                    data={"payload": payload.json()},
-                    files={"observation_set": dataframe_to_arrow_bytes(batch)},
-                )
-                if response.status_code != HTTPStatus.OK:
-                    raise RecordRetrievalException(
-                        response,
-                        resolution=(
-                            f"\nIf the error is related to connection broken, "
-                            f"try to use a smaller `max_batch_size` parameter (current value: {max_batch_size})."
-                        ),
-                    )
-
-                output.append(dataframe_from_arrow_stream(response.content))
-                progress_bar()  # pylint: disable=not-callable
-
-        return pd.concat(output, ignore_index=True)
+        try:
+            return temp_historical_feature_table.to_pandas()
+        finally:
+            temp_historical_feature_table.delete()
 
     @typechecked
     def compute_historical_feature_table(
         self,
         observation_table: Union[ObservationTable, pd.DataFrame],
         historical_feature_table_name: str,
         serving_names_mapping: Optional[Dict[str, str]] = None,
@@ -1065,14 +1261,32 @@
             Name of the historical feature table to be created
         serving_names_mapping : Optional[Dict[str, str]]
             Optional serving names mapping if the training events table has different serving name
 
         Returns
         -------
         HistoricalFeatureTable
+
+        Examples
+        --------
+        >>> # Get the desired observation table
+        >>> observation_table = catalog.get_observation_table(<observation_table_name>)  # doctest: +SKIP
+        >>> # Get the desired feature list
+        >>> my_feature_list = catalog.get_feature_list(<feature_list_name>)  # doctest: +SKIP
+        >>> # Decide the name of the historical feature table
+        >>> training_table_name = (  # doctest: +SKIP
+        ...   '2y Features for Customer Purchase next 2w '
+        ...   'up to end 22 with Improved Feature List'
+        ... )
+        >>> # Compute the historical feature table
+        >>> training_table = my_feature_list.compute_historical_feature_table(  # doctest: +SKIP
+        ...   observation_table=observation_table,
+        ...   historical_feature_table_name=training_table_name
+        ...   serving_names_mapping={"GROCERYCUSTOMERGUID": "CUSTOMERGUID"}
+        ... )
         """
         featurelist_get_historical_features = FeatureListGetHistoricalFeatures(
             feature_list_id=self.id,
             feature_clusters=self._get_feature_clusters(),
             serving_names_mapping=serving_names_mapping,
         )
         feature_store_id = featurelist_get_historical_features.feature_clusters[0].feature_store_id
@@ -1225,15 +1439,15 @@
         ----------
         status: Literal[tuple(FeatureListStatus)]
             Desired feature list status.
 
         Examples
         --------
         >>> feature_list = catalog.get_feature_list("invoice_feature_list")
-        >>> feature_list.update_status(FeatureListStatus.TEMPLATE)
+        >>> feature_list.update_status(fb.FeatureListStatus.TEMPLATE)
         """
         self.feature_list_namespace.update(
             update_payload={"status": str(status)}, allow_update_local=False
         )
 
     @typechecked
     def update_default_version_mode(
@@ -1252,16 +1466,16 @@
         Parameters
         ----------
         default_version_mode: Literal[tuple(DefaultVersionMode)]
             Feature list default version mode
 
         Examples
         --------
-        >>> feature_list = catalog.get_feature_list("invoice_feature_list")
-        >>> feature_list.update_default_version_mode(DefaultVersionMode.MANUAL)
+        >>> feature_list = catalog.get_feature_list_by_id(<FeatureList_Object_ID>)  # doctest: +SKIP
+        >>> feature_list.update_default_version_mode(DefaultVersionMode.MANUAL)  # doctest: +SKIP
 
         See Also
         --------
         - [FeatureList.create_new_version](/reference/featurebyte.api.feature_list.FeatureList.create_new_version/)
         - [FeatureList.as_default_version](/reference/featurebyte.api.feature_list.FeatureList.as_default_version/)
         """
         self.feature_list_namespace.update(
@@ -1280,17 +1494,17 @@
         The default version streamlines feature list reuse by supplying the most suitable version when none is
         explicitly indicated. By default, the feature list's default version mode is automatic, selecting the version
         with the highest percentage of production ready features. If several versions share the same readiness level,
         the most recent one becomes the default."
 
         Examples
         --------
-        >>> feature_list = catalog.get_feature_list("invoice_feature_list")
-        >>> feature_list.update_default_version_mode(DefaultVersionMode.MANUAL)
-        >>> feature_list.as_default_version()
+        >>> feature_list = catalog.get_feature_list_by_id(<FeatureList_Object_ID>)  # doctest: +SKIP
+        >>> feature_list.update_default_version_mode(DefaultVersionMode.MANUAL)  # doctest: +SKIP
+        >>> feature_list.as_default_version()  # doctest: +SKIP
 
         See Also
         --------
         - [FeatureList.create_new_version](/reference/featurebyte.api.feature_list.FeatureList.create_new_version/)
         - [FeatureList.update_default_version_mode](/reference/featurebyte.api.feature_list.FeatureList.update_default_version_mode/)
         """
         self.feature_list_namespace.update(
@@ -1329,15 +1543,18 @@
         -------
         Deployment
             Deployment object of the feature list. The created deployment is disabled by default.
 
         Examples
         --------
         >>> feature_list = catalog.get_feature_list("invoice_feature_list")
-        >>> deployment = feature_list.deploy(make_production_ready=True)  # doctest: +SKIP
+        >>> deployment = feature_list.deploy(  # doctest: +SKIP
+        ...   deployment_name="new deploy",
+        ...   make_production_ready=True,
+        ... )
 
         See Also
         --------
         - [Deployment.get_online_serving_code](/reference/featurebyte.api.deployment.Deployment.get_online_serving_code/)
         """
         self.update(
             update_payload={
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_namespace.py` & `featurebyte-0.3.0/featurebyte/api/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_store.py` & `featurebyte-0.3.0/featurebyte/api/feature_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Optional
 
 from bson import ObjectId
 from pandas import DataFrame
 
-from featurebyte.api.api_object import SavableApiObject
 from featurebyte.api.data_source import DataSource
+from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.enum import SourceType
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.models.credential import DatabaseCredential, StorageCredential
 from featurebyte.models.feature_store import FeatureStoreModel
 from featurebyte.query_graph.node.schema import DatabaseDetails
 from featurebyte.schema.feature_store import FeatureStoreCreate
@@ -41,36 +41,39 @@
     database_credential: Optional[DatabaseCredential] = None
     storage_credential: Optional[StorageCredential] = None
 
     def _get_create_payload(self) -> dict[str, Any]:
         data = FeatureStoreCreate(**self.json_dict())
         return data.json_dict()
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         Returns a dictionary that summarizes the essential information of the feature store represented by the
         FeatureStore object. The dictionary contains the following keys:
 
         - `name`: The name of the feature store.
         - `created_at`: The timestamp indicating when the feature store owas created.
         - `updated_at`: The timestamp indicating when the FeatureStore object was last updated.
         - `source`: The type of the feature store (Spark, Snowflake, DataBricks,...).
-        - `database_details`: details of the database used by the feature store."
+        - `database_details`: details of the database used by the feature store.
 
         Parameters
         ----------
         verbose: bool
             The parameter "verbose" in the current state of the code does not have any impact on the output.
 
         Returns
         -------
         Dict[str, Any]
             Key-value mapping of properties of the object.
+
+        Examples
+        --------
+        >>> feature_store = fb.FeatureStore.get(<feature_store_name>)  # doctest: +SKIP
+        >>> feature_store.info()  # doctest: +SKIP
         """
         return super().info(verbose)
 
     @classmethod
     def create(
         cls,
         name: str,
@@ -100,14 +103,31 @@
             Credential details to use when connecting to the database.
         storage_credential: Optional[StorageCredential]
             Credential details to use when connecting to the storage.
 
         Returns
         -------
         FeatureStore
+
+        Examples
+        --------
+        >>> feature_store = fb.FeatureStore.create(  # doctest: +SKIP
+        ...     name="playground",
+        ...     source_type=SourceType.SPARK,
+        ...     details=fb.SparkDetails(
+        ...         host="spark-thrift",
+        ...         http_path="cliservice",
+        ...         port=10000,
+        ...         storage_type="file",
+        ...         storage_url="/data/staging/featurebyte",
+        ...         storage_spark_url="file:///opt/spark/data/staging/featurebyte",
+        ...         featurebyte_catalog="spark_catalog",
+        ...         featurebyte_schema="playground",
+        ...     )
+        ... )
         """
         # Construct object, and save to persistent layer.
         feature_store = FeatureStore(
             name=name,
             type=source_type,
             details=details,
             database_credential=database_credential,
@@ -183,15 +203,15 @@
                 source_type=source_type,
                 details=details,
                 database_credential=database_credential,
                 storage_credential=storage_credential,
             )
 
     @classmethod
-    def get(cls, name: str) -> FeatureStore:  # pylint: disable=useless-parent-delegation
+    def get(cls, name: str) -> FeatureStore:
         """
         Gets a FeatureStore object by its name.
 
         Parameters
         ----------
         name: str
             Name of the feature store to retrieve.
@@ -206,15 +226,15 @@
         Get a FeatureStore object that is already saved.
 
         >>> feature_store = fb.FeatureStore.get("feature_store_name")  # doctest: +SKIP
         """
         return super().get(name)
 
     @classmethod
-    def get_by_id(  # pylint: disable=useless-parent-delegation
+    def get_by_id(
         cls, id: ObjectId  # pylint: disable=redefined-builtin,invalid-name
     ) -> FeatureStore:
         """
         Returns a FeatureStore object by its unique identifier (ID).
 
         Parameters
         ----------
@@ -224,24 +244,22 @@
         Returns
         -------
         FeatureStore
             FeatureStore object.
 
         Examples
         --------
-        Get a FeatureStore object that is already saved.
+        Get a FeatureStore object by its Object ID.
 
         >>> fb.FeatureStore.get_by_id(<catalog_id>)  # doctest: +SKIP
         """
         return cls._get_by_id(id=id)
 
     @classmethod
-    def list(  # pylint: disable=useless-parent-delegation
-        cls, include_id: Optional[bool] = True
-    ) -> DataFrame:
+    def list(cls, include_id: Optional[bool] = True) -> DataFrame:
         """
         Returns a DataFrame that lists the feature stores by their names, types and creation dates.
 
         Parameters
         ----------
         include_id: Optional[bool]
             Whether to include id in the list.
@@ -264,12 +282,18 @@
         Gets the data source associated with the feature store.
 
         Returns
         -------
         DataSource
             DataSource object
 
+        Examples
+        --------
+        Get a data source from a feature store.
+
+        >>> data_source = fb.FeatureStore.get("playground").get_data_source()
+
         See Also
         --------
         - [DataSource](/reference/featurebyte.api.data_source.DataSource/): DataSource class
         """
         return DataSource(feature_store_model=self)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_util.py` & `featurebyte-0.3.0/featurebyte/api/feature_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/feature_validation_util.py` & `featurebyte-0.3.0/featurebyte/api/feature_validation_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/groupby.py` & `featurebyte-0.3.0/featurebyte/api/groupby.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,14 +31,49 @@
 
     The grouping keys determine the primary entity for the declared features in the aggregation function.
 
     Moreover, the groupby method's category parameter allows you to define a categorical column, which can be used to
     generate Cross Aggregate Features. These features involve aggregating data across categories of the categorical
     column, enabling the extraction of patterns in an entity across these categories. For instance, you can calculate
     the amount spent by a customer on each product category during a specific time period using this approach.
+
+    Examples
+    --------
+    Groupby for Aggregate features.
+
+    >>> items_view = catalog.get_view("INVOICEITEMS")
+    >>> # Group items by the column GroceryCustomerGuid that references the customer entity
+    >>> items_by_customer = items_view.groupby("GroceryCustomerGuid")
+    >>> # Declare features that measure the discount received by customer
+    >>> customer_discounts = items_by_customer.aggregate_over(  # doctest: +SKIP
+    ...   "Discount",
+    ...   method=fb.AggFunc.SUM,
+    ...   feature_names=["CustomerDiscounts_7d", "CustomerDiscounts_28d"],
+    ...   fill_value=0,
+    ...   windows=['7d', '28d']
+    ... )
+
+
+    Groupby for Cross Aggregate features
+
+    >>> # Join product view to items view
+    >>> product_view = catalog.get_view("GROCERYPRODUCT")
+    >>> items_view = items_view.join(product_view)
+    >>> # Group items by the column GroceryCustomerGuid that references the customer entity
+    >>> # And use ProductGroup as the column to perform operations across
+    >>> items_by_customer_across_product_group = items_view.groupby(
+    ...   by_keys = "GroceryCustomerGuid", category="ProductGroup"
+    ... )
+    >>> # Cross Aggregate feature of the customer purchases across product group over the past 4 weeks
+    >>> customer_inventory_28d = items_by_customer_across_product_group.aggregate_over(
+    ...   "TotalCost",
+    ...   method=fb.AggFunc.SUM,
+    ...   feature_names=["CustomerInventory_28d"],
+    ...   windows=['28d']
+    ... )
     """
 
     # documentation metadata
     __fbautodoc__ = FBAutoDoc()
 
     @typechecked
     def __init__(
@@ -154,23 +189,46 @@
 
         Returns
         -------
         FeatureGroup
 
         Examples
         --------
-        >>> import featurebyte as fb
-        >>> features = cc_transactions.groupby("AccountID").aggregate_over(  # doctest: +SKIP
-        ...    "Amount",
-        ...    method=fb.AggFunc.SUM,
-        ...    windows=["7d", "30d"],
-        ...    feature_names=["Total spend 7d", "Total spend 30d"],
+        Sum of discounts by grocerycustomer entity over the past 7 and 28 days.
+
+        >>> items_view = catalog.get_view("INVOICEITEMS")
+        >>> # Group items by the column GroceryCustomerGuid that references the customer entity
+        >>> items_by_customer = items_view.groupby("GroceryCustomerGuid")
+        >>> # Declare features that measure the discount received by customer
+        >>> customer_discounts = items_by_customer.aggregate_over(
+        ...   "Discount",
+        ...   method=fb.AggFunc.SUM,
+        ...   feature_names=["CustomerDiscounts_7d", "CustomerDiscounts_28d"],
+        ...   fill_value=0,
+        ...   windows=['7d', '28d']
+        ... )
+
+
+        Sum spent by grocerycustomer entity across product group over the past 28 days.
+
+        >>> # Join product view to items view
+        >>> product_view = catalog.get_view("GROCERYPRODUCT")
+        >>> items_view = items_view.join(product_view)
+        >>> # Group items by the column GroceryCustomerGuid that references the customer entity
+        >>> # And use ProductGroup as the column to perform operations across
+        >>> items_by_customer_across_product_group = items_view.groupby(
+        ...   by_keys="GroceryCustomerGuid", category="ProductGroup"
+        ... )
+        >>> # Cross Aggregate feature of the customer purchases across product group over the past 4 weeks
+        >>> customer_inventory_28d = items_by_customer_across_product_group.aggregate_over(
+        ...   "TotalCost",
+        ...   method=fb.AggFunc.SUM,
+        ...   feature_names=["CustomerInventory_28d"],
+        ...   windows=['28d']
         ... )
-        >>> features.feature_names  # doctest: +SKIP
-        ['Total spend 7d', 'Total spend 30d']
 
         See Also
         --------
         - [FeatureGroup](/reference/featurebyte.api.feature_group.FeatureGroup/): FeatureGroup object
         - [Feature](/reference/featurebyte.api.feature.Feature/): Feature object
         """
         return WindowAggregator(
@@ -255,21 +313,35 @@
 
         Returns
         -------
         Feature
 
         Examples
         --------
-        >>> import featurebyte as fb
-        >>> feature = credit_card_accounts.groupby("CustomerID").aggregate_asat(  # doctest: +SKIP
-        ...    method=fb.AggFunc.COUNT,
-        ...    feature_name="Number of Credit Cards",
+        Count number of active cards per customer at a point-in-time.
+
+        >>> # Filter active cards
+        >>> cond = credit_card_accounts['status'] == "active"  # doctest: +SKIP
+        >>> # Group by customer
+        >>> active_credit_card_by_cust = credit_card_accounts[cond].groupby(  # doctest: +SKIP
+        ...   "CustomerID"
+        ... )
+        >>> feature = active_credit_card_by_cust.aggregate_asat(  # doctest: +SKIP
+        ...   method=fb.AggFunc.COUNT,
+        ...   feature_name="Number of Active Credit Cards",
+        ... )
+
+
+        Count number of active cards per customer 12 weeks prior to a point-in-time
+
+        >>> feature_12w_before = active_credit_card_by_cust.aggregate_asat(  # doctest: +SKIP
+        ...   method=fb.AggFunc.COUNT,
+        ...   feature_name="Number of Active Credit Cards 12 w before",
+        ...   offset="12w"
         ... )
-        >>> feature  # doctest: +SKIP
-        Feature(name=Number of Credit Cards, node_name=alias_1)
         """
         return AsAtAggregator(
             self.view_obj, self.category, self.entity_ids, self.keys, self.serving_names
         ).aggregate_asat(
             value_column=value_column,
             method=method,
             feature_name=feature_name,
@@ -320,14 +392,26 @@
             Value to fill if the value in the column is empty
         skip_fill_na: bool
             Whether to skip filling NaN values
 
         Returns
         -------
         Feature
+
+        Examples
+        --------
+        >>> items_view = catalog.get_view("INVOICEITEMS")
+        >>> # Group items by the column GroceryInvoiceGuid that references the customer entity
+        >>> items_by_invoice = items_view.groupby("GroceryInvoiceGuid")
+        >>> # Get the number of items in each invoice
+        >>> invoice_item_count = items_by_invoice.aggregate(  # doctest: +SKIP
+        ...   None,
+        ...   method=fb.AggFunc.COUNT,
+        ...   feature_name="InvoiceItemCount",
+        ... )
         """
         return SimpleAggregator(
             self.view_obj, self.category, self.entity_ids, self.keys, self.serving_names
         ).aggregate(
             value_column=value_column,
             method=method,
             feature_name=feature_name,
```

### Comparing `featurebyte-0.2.2/featurebyte/api/historical_feature_table.py` & `featurebyte-0.3.0/featurebyte/service/historical_feature_table.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,84 @@
 """
-HistoricalFeatureTable class
+HistoricalFeatureTableService class
 """
 from __future__ import annotations
 
+from typing import Optional
+
+from pathlib import Path
+
 import pandas as pd
+from bson import ObjectId
 
-from featurebyte.api.api_object import ApiObject, ForeignKeyMapping
-from featurebyte.api.feature_store import FeatureStore
-from featurebyte.api.materialized_table import MaterializedTableMixin
-from featurebyte.api.observation_table import ObservationTable
-from featurebyte.common.doc_util import FBAutoDoc
+from featurebyte.models.base import FeatureByteBaseDocumentModel
 from featurebyte.models.historical_feature_table import HistoricalFeatureTableModel
-from featurebyte.schema.historical_feature_table import HistoricalFeatureTableListRecord
+from featurebyte.schema.historical_feature_table import HistoricalFeatureTableCreate
+from featurebyte.schema.worker.task.historical_feature_table import (
+    HistoricalFeatureTableTaskPayload,
+)
+from featurebyte.service.materialized_table import BaseMaterializedTableService
+from featurebyte.storage import Storage
 
 
-class HistoricalFeatureTable(HistoricalFeatureTableModel, ApiObject, MaterializedTableMixin):
+class HistoricalFeatureTableService(
+    BaseMaterializedTableService[HistoricalFeatureTableModel, HistoricalFeatureTableModel]
+):
     """
-    HistoricalFeatureTable class
+    HistoricalFeatureTableService class
     """
 
-    __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.HistoricalFeatureTable")
-
-    _route = "/historical_feature_table"
-    _list_schema = HistoricalFeatureTableListRecord
-    _get_schema = HistoricalFeatureTableModel
-    _list_fields = [
-        "name",
-        "feature_store_name",
-        "observation_table_name",
-        "shape",
-        "created_at",
-    ]
-    _list_foreign_keys = [
-        ForeignKeyMapping("feature_store_id", FeatureStore, "feature_store_name"),
-        ForeignKeyMapping("observation_table_id", ObservationTable, "observation_table_name"),
-    ]
-
-    def preview(self, limit: int = 10) -> pd.DataFrame:
-        """
-        Returns a DataFrame that contains a selection of rows of the historical feature table.
-
-        Parameters
-        ----------
-        limit: int
-            Maximum number of return rows.
-
-        Returns
-        -------
-        pd.DataFrame
-            Preview rows of the table.
-        """
-        return super().preview(limit=limit)
+    document_class = HistoricalFeatureTableModel
+    materialized_table_name_prefix = "HISTORICAL_FEATURE_TABLE"
 
-    def sample(self, size: int = 10, seed: int = 1234) -> pd.DataFrame:
+    @property
+    def class_name(self) -> str:
+        return "HistoricalFeatureTable"
+
+    async def get_historical_feature_table_task_payload(
+        self,
+        data: HistoricalFeatureTableCreate,
+        storage: Storage,
+        observation_set_dataframe: Optional[pd.DataFrame],
+    ) -> HistoricalFeatureTableTaskPayload:
         """
-        Returns a DataFrame that contains a random selection of rows of the historical feature table based on a
-        specified size and seed for sampling control.
+        Validate and convert a HistoricalFeatureTableCreate schema to a HistoricalFeatureTableTaskPayload schema
+        which will be used to initiate the HistoricalFeatureTable creation task.
 
         Parameters
         ----------
-        size: int
-            Maximum number of rows to sample.
-        seed: int
-            Seed to use for random sampling.
+        data: HistoricalFeatureTableCreate
+            HistoricalFeatureTable creation payload
+        storage: Storage
+            Storage instance
+        observation_set_dataframe: Optional[pd.DataFrame]
+            Optional observation set DataFrame. If provided, the DataFrame will be stored in the
+            temp storage to be used by the HistoricalFeatureTable creation task.
 
         Returns
         -------
-        pd.DataFrame
-            Sampled rows from the table.
+        HistoricalFeatureTableTaskPayload
         """
-        return super().sample(size=size, seed=seed)
-
-    def describe(self, size: int = 0, seed: int = 1234) -> pd.DataFrame:
-        """
-        Returns descriptive statistics of the historical feature table.
-
-        Parameters
-        ----------
-        size: int
-            Maximum number of rows to sample. If 0, all rows will be used.
-        seed: int
-            Seed to use for random sampling.
 
-        Returns
-        -------
-        pd.DataFrame
-            Summary of the table.
-        """
-        return super().describe(size=size, seed=seed)
+        # Check any conflict with existing documents
+        output_document_id = data.id or ObjectId()
+        await self._check_document_unique_constraints(
+            document=FeatureByteBaseDocumentModel(_id=output_document_id, name=data.name),
+        )
+
+        if observation_set_dataframe is not None:
+            observation_set_storage_path = (
+                f"historical_feature_table/observation_set/{output_document_id}.parquet"
+            )
+            await storage.put_dataframe(
+                observation_set_dataframe, Path(observation_set_storage_path)
+            )
+        else:
+            observation_set_storage_path = None
+
+        return HistoricalFeatureTableTaskPayload(
+            **data.dict(),
+            user_id=self.user.id,
+            catalog_id=self.catalog_id,
+            output_document_id=output_document_id,
+            observation_set_storage_path=observation_set_storage_path,
+        )
```

### Comparing `featurebyte-0.2.2/featurebyte/api/item_table.py` & `featurebyte-0.3.0/featurebyte/api/item_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 ItemTable class
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, ClassVar, List, Literal, Optional, Type, cast
 
+from bson import ObjectId
 from pydantic import Field, StrictStr, root_validator
 
 from featurebyte.api.base_table import TableApiObject
 from featurebyte.api.event_table import EventTable
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.join_utils import append_rsuffix_to_columns
 from featurebyte.common.validator import construct_data_model_root_validator
@@ -159,18 +160,46 @@
         Returns
         -------
         ItemView
             ItemView object constructed from the source table.
 
         Examples
         --------
-        Get an ItemView.
+        Get an ItemView in automated mode.
 
-        >>> item_table = fb.Table.get("INVOICEITEMS")
+        >>> item_table = catalog.get_table("INVOICEITEMS")
         >>> item_view = item_table.get_view()
+
+
+        Get an ItemView in manual mode.
+
+        >>> item_table = catalog.get_table("INVOICEITEMS")
+        >>> item_view = item_table.get_view(
+        ...   event_suffix=None,
+        ...   view_mode="manual",
+        ...   drop_column_names=[],
+        ...   column_cleaning_operations=[
+        ...     fb.ColumnCleaningOperation(
+        ...       column_name="Discount",
+        ...       cleaning_operations=[
+        ...         fb.MissingValueImputation(imputed_value=0),
+        ...         fb.ValueBeyondEndpointImputation(
+        ...           type="less_than", end_point=0, imputed_value=None
+        ...         ),
+        ...       ],
+        ...     )
+        ...   ],
+        ...   event_drop_column_names=["record_available_at"],
+        ...   event_column_cleaning_operations=[],
+        ...   event_join_column_names=[
+        ...     "Timestamp",
+        ...     "GroceryInvoiceGuid",
+        ...     "GroceryCustomerGuid",
+        ...   ],
+        ... )
         """
         from featurebyte.api.item_view import ItemView  # pylint: disable=import-outside-toplevel
 
         self._validate_view_mode_params(
             view_mode=view_mode,
             drop_column_names=drop_column_names,
             column_cleaning_operations=column_cleaning_operations,
@@ -313,7 +342,30 @@
             return self.cached_model.item_id_column
         except RecordRetrievalException:
             return self.internal_item_id_column
 
     @property
     def timestamp_column(self) -> Optional[str]:
         return None
+
+    @classmethod
+    def get_by_id(cls, id: ObjectId) -> ItemTable:  # pylint: disable=redefined-builtin,invalid-name
+        """
+        Returns an ItemTable object by its unique identifier (ID).
+
+        Parameters
+        ----------
+        id: ObjectId
+            ItemTable unique identifier ID.
+
+        Returns
+        -------
+        ItemTable
+            ItemTable object.
+
+        Examples
+        --------
+        Get an ItemTable object that is already saved.
+
+        >>> fb.ItemTable.get_by_id(<item_table_id>)  # doctest: +SKIP
+        """
+        return cls._get_by_id(id=id)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/item_view.py` & `featurebyte-0.3.0/featurebyte/api/item_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/lag.py` & `featurebyte-0.3.0/featurebyte/api/lag.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,16 +43,25 @@
         Raises
         ------
         ValueError
             If a lag operation has already been applied to the column.
 
         Examples
         --------
-        >>> event_view = fb.Table.get("GROCERYINVOICE").get_view()
+        Create a new column that indicates the prior event timestamp for a Customer.
+
+        >>> event_view = catalog.get_view("GROCERYINVOICE")
         >>> lagged_column = event_view["Timestamp"].lag("GroceryCustomerGuid")
+
+
+        Create a new column that indicates the 2nd prior event timestamp for a Customer.
+
+        >>> lagged_2_column = event_view["Timestamp"].lag(
+        ...   "GroceryCustomerGuid", offset=2
+        ... )
         """
         if not isinstance(entity_columns, list):
             entity_columns = [entity_columns]
         if NodeType.LAG in self.node_types_lineage:
             raise ValueError("lag can only be applied once per column")
         assert self._parent is not None
```

### Comparing `featurebyte-0.2.2/featurebyte/api/materialized_table.py` & `featurebyte-0.3.0/featurebyte/api/materialized_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,31 @@
     """
 
     _route: ClassVar[str] = ""
     _poll_async_task: Callable[..., Any]
 
     def download(self, output_path: Optional[Union[str, Path]] = None) -> Path:
         """
-        Downloads the table from the database
+        Downloads the table from the database.
 
         Parameters
         ----------
         output_path: Optional[Union[str, Path]]
-            Location to save downloaded parquet file
+            Location to save downloaded parquet file.
 
         Returns
         -------
         Path
 
         Raises
         ------
         FileExistsError
-            File already exists at output path
+            File already exists at output path.
         RecordRetrievalException
-            Error retrieving record from API
+            Error retrieving record from API.
         """
         file_name = f"{self.location.table_details.table_name}.parquet"
         output_path = output_path or Path(f"./{file_name}")
         output_path = Path(output_path)
         if output_path.exists():
             raise FileExistsError(f"{output_path} already exists.")
 
@@ -60,28 +60,28 @@
         parquet_from_arrow_stream(
             response=response, output_path=output_path, num_rows=self.num_rows
         )
         return output_path
 
     def to_pandas(self) -> pd.DataFrame:
         """
-        Converts the table to pandas dataframe
+        Converts the table to pandas dataframe.
 
         Returns
         -------
         pd.DataFrame
         """
         with tempfile.TemporaryDirectory() as temp_dir:
             output_path = os.path.join(temp_dir, "temp.parquet")
             self.download(output_path=output_path)
             return pd.read_parquet(output_path)
 
     def delete(self) -> None:
         """
-        Deletes the materialized table
+        Deletes the materialized table.
 
         Raises
         ------
         RecordDeletionException
             When the record cannot be deleted properly
         """
         client = Configurations().get_client()
```

### Comparing `featurebyte-0.2.2/featurebyte/api/observation_table.py` & `featurebyte-0.3.0/featurebyte/sql/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,111 @@
 """
-ObservationTable class
+Common utilities for Spark SQL
 """
-# pylint: disable=duplicate-code
 from __future__ import annotations
 
+from typing import Optional
+
+import asyncio
+from random import randint
+
 import pandas as pd
 
-from featurebyte.api.api_object import ApiObject, ForeignKeyMapping
-from featurebyte.api.feature_store import FeatureStore
-from featurebyte.api.materialized_table import MaterializedTableMixin
-from featurebyte.common.doc_util import FBAutoDoc
-from featurebyte.models.observation_table import ObservationTableModel
-from featurebyte.schema.observation_table import ObservationTableListRecord
+from featurebyte.logging import get_logger
+from featurebyte.session.base import BaseSession
+from featurebyte.session.snowflake import SnowflakeSession
+
+TABLE_PROPERTIES = "TBLPROPERTIES('delta.columnMapping.mode' = 'name', 'delta.minReaderVersion' = '2', 'delta.minWriterVersion' = '5')"
+
+
+logger = get_logger(__name__)
 
 
-class ObservationTable(ObservationTableModel, ApiObject, MaterializedTableMixin):
+def construct_create_table_query(
+    table_name: str,
+    table_query: str,
+    partition_keys: Optional[str] = None,
+    session: Optional[BaseSession] = None,
+) -> str:
     """
-    ObservationTable class
+    Construct a query to create a delta table in Spark based table_query
+
+    Parameters
+    ----------
+    table_name: str
+        Table name
+    table_query: str
+        SQL query for the contents of the table
+    partition_keys: str
+        Partition keys
+    session: BaseSession
+        Spark or Snowflake session
+
+    Returns
+    -------
+    str
+        Query to create a delta table in Spark
+    """
+    partition_clause = ""
+    if partition_keys:
+        partition_clause = f"PARTITIONED BY ({partition_keys})"
+
+    sql = f"""
+            CREATE TABLE {table_name} USING DELTA
+                {partition_clause}
+                {TABLE_PROPERTIES}
+            AS
+                {table_query}
+            """
+    if session is not None and isinstance(session, SnowflakeSession):
+        sql = f"CREATE TABLE {table_name} AS (SELECT * FROM ({table_query}))"
+
+    return sql
+
+
+async def retry_sql(
+    session: BaseSession,
+    sql: str,
+    retry_num: int = 10,
+    sleep_interval: int = 5,
+) -> pd.DataFrame | None:
     """
+    Retry sql operation
+
+    Parameters
+    ----------
+    session: BaseSession
+        Spark session
+    sql: str
+        SQL query
+    retry_num: int
+        Number of retries
+    sleep_interval: int
+        Sleep interval between retries
+
+    Returns
+    -------
+    pd.DataFrame
+        Result of the sql operation
+
+    Raises
+    ------
+    Exception
+        if the sql operation fails after retry_num retries
+    """
+
+    for i in range(retry_num):
+        try:
+            return await session.execute_query_long_running(sql)
+        except Exception as exc:  # pylint: disable=broad-exception-caught
+            logger.warning(
+                "SQL query failed",
+                extra={"attempt": i, "query": sql.strip()[:50].replace("\n", " ")},
+            )
+            if i == retry_num - 1:
+                logger.error("SQL query failed", extra={"attempts": retry_num, "exception": exc})
+                raise
 
-    __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.ObservationTable")
+        random_interval = randint(1, sleep_interval)
+        await asyncio.sleep(random_interval)
 
-    _route = "/observation_table"
-    _list_schema = ObservationTableListRecord
-    _get_schema = ObservationTableModel
-    _list_fields = [
-        "name",
-        "type",
-        "shape",
-        "feature_store_name",
-        "created_at",
-    ]
-    _list_foreign_keys = [
-        ForeignKeyMapping("feature_store_id", FeatureStore, "feature_store_name"),
-    ]
-
-    def to_pandas(self) -> pd.DataFrame:
-        """
-        Converts the observation table to a pandas dataframe.
-
-        Returns
-        -------
-        pd.DataFrame
-
-        Examples
-        --------
-        >>> observation_table = catalog.get_observation_table("observation_table_name")  # doctest: +SKIP
-        >>> observation_table.to_pandas()  # doctest: +SKIP
-        """
-        return super().to_pandas()
-
-    def preview(self, limit: int = 10) -> pd.DataFrame:
-        """
-        Returns a DataFrame that contains a selection of rows of the observation table.
-
-        Parameters
-        ----------
-        limit: int
-            Maximum number of return rows.
-
-        Returns
-        -------
-        pd.DataFrame
-            Preview rows of the table.
-        """
-        return super().preview(limit=limit)
-
-    def sample(self, size: int = 10, seed: int = 1234) -> pd.DataFrame:
-        """
-        Returns a DataFrame that contains a random selection of rows of the observation table based on a
-        specified size and seed for sampling control.
-
-        Parameters
-        ----------
-        size: int
-            Maximum number of rows to sample.
-        seed: int
-            Seed to use for random sampling.
-
-        Returns
-        -------
-        pd.DataFrame
-            Sampled rows from the table.
-        """
-        return super().sample(size=size, seed=seed)
-
-    def describe(self, size: int = 0, seed: int = 1234) -> pd.DataFrame:
-        """
-        Returns descriptive statistics of the observation table.
-
-        Parameters
-        ----------
-        size: int
-            Maximum number of rows to sample. If 0, all rows will be used.
-        seed: int
-            Seed to use for random sampling.
-
-        Returns
-        -------
-        pd.DataFrame
-            Summary of the table.
-        """
-        return super().describe(size=size, seed=seed)
+    return None
```

### Comparing `featurebyte-0.2.2/featurebyte/api/periodic_task.py` & `featurebyte-0.3.0/featurebyte/api/periodic_task.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 PeriodicTask class
 """
 from __future__ import annotations
 
-from featurebyte.api.api_object import SavableApiObject
+from featurebyte.api.savable_api_object import SavableApiObject
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.models.periodic_task import PeriodicTask as PeriodicTaskModel
 
 
 class PeriodicTask(PeriodicTaskModel, SavableApiObject):
     """
     PeriodicTask class
```

### Comparing `featurebyte-0.2.2/featurebyte/api/relationship.py` & `featurebyte-0.3.0/featurebyte/api/relationship.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Relationships API object
 """
-from typing import Literal, Optional
+from typing import Any, Dict, Literal, Optional
 
 import pandas as pd
 from pydantic import Field
 from typeguard import typechecked
 
 from featurebyte.api.api_object import ApiObject, ForeignKeyMapping
 from featurebyte.api.base_table import TableApiObject
 from featurebyte.api.entity import Entity
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.exception import RecordRetrievalException
 from featurebyte.models.base import PydanticObjectId
-from featurebyte.models.relationship import RelationshipInfo, RelationshipType
+from featurebyte.models.relationship import RelationshipInfoModel, RelationshipType
 from featurebyte.schema.relationship_info import RelationshipInfoUpdate
 
 
 class Relationship(ApiObject):
     """
     The relationships class allows users to see explore what types of relationships exist between the various
     entities they have.
@@ -38,16 +38,16 @@
     __fbautodoc__ = FBAutoDoc(
         proxy_class="featurebyte.Relationship",
     )
 
     # class variables
     _route = "/relationship_info"
     _update_schema_class = RelationshipInfoUpdate
-    _get_schema = RelationshipInfo
-    _list_schema = RelationshipInfo
+    _get_schema = RelationshipInfoModel
+    _list_schema = RelationshipInfoModel
     _list_fields = [
         "relationship_type",
         "entity",
         "related_entity",
         "relation_table",
         "relation_table_type",
         "enabled",
@@ -59,15 +59,15 @@
         ForeignKeyMapping("related_entity_id", Entity, "related_entity"),
         ForeignKeyMapping("relation_table_id", TableApiObject, "relation_table"),
         ForeignKeyMapping("relation_table_id", TableApiObject, "relation_table_type", "type"),
     ]
 
     # pydantic instance variable (internal use)
     internal_enabled: bool = Field(alias="enabled")
-    internal_updated_by: PydanticObjectId = Field(alias="updated_by")
+    internal_updated_by: Optional[PydanticObjectId] = Field(alias="updated_by")
 
     @property
     def enabled(self) -> bool:
         """
         Whether the relationship has been enabled
 
         Returns
@@ -77,28 +77,44 @@
         """
         try:
             return self.cached_model.enabled
         except RecordRetrievalException:
             return self.internal_enabled
 
     @property
-    def updated_by(self) -> PydanticObjectId:
+    def updated_by(self) -> Optional[PydanticObjectId]:
         """
         Who the relationship was updated by
 
         Returns
         -------
         PydanticObjectId
             User ID of the user who updated the relationship
         """
         try:
             return self.cached_model.updated_by
         except RecordRetrievalException:
             return self.internal_updated_by
 
+    @property
+    def catalog_id(self) -> PydanticObjectId:
+        """
+        Returns the unique identifier (ID) of the Catalog that is associated with the Relationship object.
+
+        Returns
+        -------
+        PydanticObjectId
+            Catalog ID of the relationship.
+
+        See Also
+        --------
+        - [Catalog](/reference/featurebyte.api.catalog.Catalog)
+        """
+        return self.cached_model.catalog_id  # pylint: disable=no-member
+
     @classmethod
     @typechecked
     def list(
         cls, include_id: Optional[bool] = True, relationship_type: Optional[Literal[tuple(RelationshipType)]] = None  # type: ignore[misc]
     ) -> pd.DataFrame:
         """
         List all relationships that exist in your FeatureByte instance, or filtered by relationship type.
@@ -189,7 +205,36 @@
         Disable a relationship
 
         >>> import featurebyte as fb  # doctest: +SKIP
         >>> relationship = fb.Relationship.get_by_id(<relationship_id>)  # doctest: +SKIP
         >>> relationship.disable()  # doctest: +SKIP
         """
         self.update({"enabled": False}, allow_update_local=True, add_internal_prefix=True)
+
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
+        """
+        Returns a dictionary that summarizes the essential information of the relationship represented by the
+        Relationship object. The dictionary contains the following keys:
+
+        - `relationship_type`: The relationship type
+        - `entity_id`: The main entity of the relationship
+        - `related_entity_id`: The entity that the relationship is related to
+        - `relation_table_id`: The table that maps the relationship
+        - `enabled`: Whether the relationship is enabled
+        - `updated_by`: Who the relationship was updated by
+
+        Parameters
+        ----------
+        verbose: bool
+            The parameter "verbose" in the current state of the code does not have any impact on the output.
+
+        Returns
+        -------
+        Dict[str, Any]
+            Key-value mapping of properties of the object.
+
+        Examples
+        --------
+        >>> relationship = fb.Relationship.get(<relationship_name>)  # doctest: +SKIP
+        >>> relationship.info()  # doctest: +SKIP
+        """
+        return super().info(verbose)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/request_column.py` & `featurebyte-0.3.0/featurebyte/api/request_column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/scd_table.py` & `featurebyte-0.3.0/featurebyte/api/scd_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 SCDTable class
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, ClassVar, List, Literal, Optional, Tuple, Type, cast
 
+from bson import ObjectId
 from pydantic import Field, StrictStr, root_validator
 
 from featurebyte.api.base_table import TableApiObject
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.validator import construct_data_model_root_validator
 from featurebyte.enum import DBVarType, TableDataType, ViewMode
 from featurebyte.exception import RecordRetrievalException
@@ -139,18 +140,35 @@
         Returns
         -------
         SCDView
             SCDView object constructed from the source table.
 
         Examples
         --------
-        Get a SCDView.
+        Get a SCDView in automated mode.
 
-        >>> scd_table = fb.Table.get("GROCERYCUSTOMER")
+        >>> scd_table = catalog.get_table("GROCERYCUSTOMER")
         >>> scd_view = scd_table.get_view()
+
+
+        Get a SCDView in manual mode.
+
+        >>> scd_table = catalog.get_table("GROCERYCUSTOMER")
+        >>> scd_view = scd_table.get_view(
+        ...   view_mode="manual",
+        ...   drop_column_names=["record_available_at", "CurrentRecord"],
+        ...   column_cleaning_operations=[
+        ...     fb.ColumnCleaningOperation(
+        ...       column_name="Gender",
+        ...       cleaning_operations=[
+        ...         fb.MissingValueImputation(imputed_value="Unknown"),
+        ...       ],
+        ...     )
+        ...   ],
+        ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.scd_view import SCDView
 
         self._validate_view_mode_params(
             view_mode=view_mode,
             drop_column_names=drop_column_names,
@@ -260,20 +278,20 @@
         Returns
         -------
         ChangeView
             ChangeView object constructed from the SCD source table.
 
         Examples
         --------
-        Get a ChangeView.
+        Get a ChangeView to track changes in Customer's State.
 
-        >>> scd_table = fb.Table.get("GROCERYCUSTOMER")
+        >>> scd_table = catalog.get_table("GROCERYCUSTOMER")
         >>> change_view = scd_table.get_change_view(
-        ...     track_changes_column="CurrentRecord",
-        ...     prefixes=("previous_", "next_"),
+        ...   track_changes_column="State",
+        ...   prefixes=("previous_", "next_"),
         ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.change_view import ChangeView
 
         # Validate input
         ChangeView.validate_inputs(self, track_changes_column, prefixes)
@@ -426,7 +444,30 @@
         Timestamp column name of the SCDTable
 
         Returns
         -------
         Optional[str]
         """
         return self.effective_timestamp_column
+
+    @classmethod
+    def get_by_id(cls, id: ObjectId) -> SCDTable:  # pylint: disable=redefined-builtin,invalid-name
+        """
+        Returns a SCDTable object by its unique identifier (ID).
+
+        Parameters
+        ----------
+        id: ObjectId
+            SCDTable unique identifier ID.
+
+        Returns
+        -------
+        SCDTable
+            SCDTable object.
+
+        Examples
+        --------
+        Get a SCDTable object that is already saved.
+
+        >>> fb.SCDTable.get_by_id(<scd_table_id>)  # doctest: +SKIP
+        """
+        return cls._get_by_id(id=id)
```

### Comparing `featurebyte-0.2.2/featurebyte/api/scd_view.py` & `featurebyte-0.3.0/featurebyte/api/scd_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/simple_aggregator.py` & `featurebyte-0.3.0/featurebyte/api/simple_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/source_table.py` & `featurebyte-0.3.0/featurebyte/api/source_table.py`

 * *Files 13% similar despite different names*

```diff
@@ -332,14 +332,30 @@
         Sample 3 rows from the table.
         >>> catalog.get_table("GROCERYPRODUCT").sample(3)
                              GroceryProductGuid ProductGroup
         0  e890c5cb-689b-4caf-8e49-6b97bb9420c0       Épices
         1  5720e4df-2996-4443-a1bc-3d896bf98140         Chat
         2  96fc4d80-8cb0-4f1b-af01-e71ad7e7104a        Pains
 
+
+        Sample 3 rows from the table with timestamps.
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(  # doctest: +SKIP
+        ...   cleaning_operations=[
+        ...     fb.MissingValueImputation(imputed_value=0),
+        ...   ]
+        ... )
+        >>> event_table.sample(  # doctest: +SKIP
+        ...   size=3,
+        ...   seed=111,
+        ...   from_timestamp=datetime(2019, 1, 1),
+        ...   to_timestamp=datetime(2023, 12, 31),
+        ...   after_cleaning=True,
+        ... )
+
         See Also
         --------
         - [Table.preview](/reference/featurebyte.api.base_table.TableApiObject.preview/):
           Retrieve a preview of a table.
         - [Table.describe](/reference/featurebyte.api.base_table.TableApiObject.describe/):
           Retrieve a summary of a table.
         """
@@ -356,14 +372,15 @@
         self,
         size: int = 0,
         seed: int = 1234,
         from_timestamp: Optional[Union[datetime, str]] = None,
         to_timestamp: Optional[Union[datetime, str]] = None,
         after_cleaning: bool = False,
     ) -> pd.DataFrame:
+        # pylint: disable=line-too-long
         """
         Returns descriptive statistics of the table columns.
 
         Parameters
         ----------
         size: int
             Maximum number of rows to sample. If 0, all rows will be used.
@@ -380,23 +397,34 @@
         -------
         pd.DataFrame
             Summary of the table.
 
         Examples
         --------
         Get a summary of a view.
-        >>> catalog.get_table("GROCERYPRODUCT").describe()
-                                    GroceryProductGuid        ProductGroup
-        dtype                                  VARCHAR             VARCHAR
-        unique                                   29099                  87
-        %missing                                   0.0                 0.0
-        %empty                                       0                   0
-        entropy                               6.214608             4.13031
-        top       017fe5ed-80a2-4e70-ae48-78aabfdee856  Chips et Tortillas
-        freq                                       1.0              1319.0
+
+        >>> catalog.get_table("GROCERYINVOICE").describe(
+        ...   from_timestamp=datetime(2022, 1, 1),
+        ...   to_timestamp=datetime(2022, 12, 31),
+        ... )
+                                    GroceryInvoiceGuid                   GroceryCustomerGuid                      Timestamp            record_available_at     Amount
+        dtype                                  VARCHAR                               VARCHAR                      TIMESTAMP                      TIMESTAMP      FLOAT
+        unique                                   25422                                   471                          25399                           5908       6734
+        %missing                                   0.0                                   0.0                            0.0                            0.0        0.0
+        %empty                                       0                                     0                            NaN                            NaN        NaN
+        entropy                               6.214608                              5.784261                            NaN                            NaN        NaN
+        top       018f0163-249b-4cbc-ab4d-e933ce3786c1  c5820998-e779-4d62-ab8b-79ef0dfd841b            2022-01-09 10:47:17            2022-02-02 17:01:00        1.0
+        freq                                       1.0                                 692.0                            2.0                           18.0      406.0
+        mean                                       NaN                                   NaN                            NaN                            NaN  19.966062
+        std                                        NaN                                   NaN                            NaN                            NaN  25.027878
+        min                                        NaN                                   NaN  2022-01-01T00:24:14.000000000  2022-01-01T01:01:00.000000000        0.0
+        25%                                        NaN                                   NaN                            NaN                            NaN     4.5325
+        50%                                        NaN                                   NaN                            NaN                            NaN     10.725
+        75%                                        NaN                                   NaN                            NaN                            NaN      24.99
+        max                                        NaN                                   NaN  2022-12-30T22:37:57.000000000  2022-12-30T23:01:00.000000000     360.84
 
         See Also
         --------
         - [Table.preview](/reference/featurebyte.api.base_table.TableApiObject.preview/):
           Retrieve a preview of a table.
         - [Table.sample](/reference/featurebyte.api.base_table.TableApiObject.sample/):
           Retrieve a sample of a table.
@@ -503,19 +531,25 @@
         EventTable
             EventTable created from the source table.
 
         Examples
         --------
         Create an event table from a source table.
 
-        >>> grocery_invoice_table = event_source_table.create_event_table(  # doctest: +SKIP
+        >>> # Register GroceryInvoice as an event data
+        >>> source_table = ds.get_table(  # doctest: +SKIP
+        ...   database_name="spark_catalog",
+        ...   schema_name="GROCERY",
+        ...   table_name="GROCERYINVOICE"
+        ... )
+        >>> invoice_table = source_table.create_event_table(  # doctest: +SKIP
         ...   name="GROCERYINVOICE",
         ...   event_id_column="GroceryInvoiceGuid",
         ...   event_timestamp_column="Timestamp",
-        ...   record_creation_timestamp_column="record_available_at",
+        ...   record_creation_timestamp_column="record_available_at"
         ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.event_table import EventTable
 
         return EventTable.create(
             source_table=self,
@@ -574,19 +608,25 @@
         ItemTable
             ItemTable created from the source table.
 
         Examples
         --------
         Create an item table from a source table.
 
-        >>> grocery_items_table = item_source_table.create_item_table(  # doctest: +SKIP
+        >>> # Register invoice items as an item table
+        >>> source_table = ds.get_table(  # doctest: +SKIP
+        ...   database_name="spark_catalog",
+        ...   schema_name="GROCERY",
+        ...   table_name="INVOICEITEMS"
+        ... )
+        >>> items_table.create_item_table(  # doctest: +SKIP
         ...   name="INVOICEITEMS",
         ...   event_id_column="GroceryInvoiceGuid",
         ...   item_id_column="GroceryInvoiceItemGuid",
-        ...   event_table_name="GROCERYINVOICE",
+        ...   event_table_name="GROCERYINVOICE"
         ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.event_table import EventTable
         from featurebyte.api.item_table import ItemTable
 
         event_table = EventTable.get(event_table_name)
@@ -643,17 +683,23 @@
         DimensionTable
             DimensionTable created from the source table.
 
         Examples
         --------
         Create a dimension table from a source table.
 
-        >>> grocery_product_table = dimension_source_table.create_dimension_table(  # doctest: +SKIP
-        ...   name="GROCERYPRODUCT",  # doctest: +SKIP
-        ...   dimension_id_column="GroceryProductGuid",
+        >>> # Register GroceryProduct as a dimension table
+        >>> source_table = ds.get_table(  # doctest: +SKIP
+        ...   database_name="spark_catalog",
+        ...   schema_name="GROCERY",
+        ...   table_name="GROCERYPRODUCT"
+        ... )
+        >>> product_table = source_table.create_dimension_table(  # doctest: +SKIP
+        ...   name="GROCERYPRODUCT",
+        ...   dimension_id_column="GroceryProductGuid"
         ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.dimension_table import DimensionTable
 
         return DimensionTable.create(
             source_table=self,
@@ -726,21 +772,27 @@
         SCDTable
             SCDTable created from the source table.
 
         Examples
         --------
         Create a SCD table from a source table.
 
-        >>> grocery_customer_table = scd_source_table.create_scd_table(  # doctest: +SKIP
-        ...   name="GROCERYCUSTOMER",
-        ...   surrogate_key_column="RowID",
-        ...   natural_key_column="GroceryCustomerGuid",
-        ...   effective_timestamp_column="ValidFrom",
-        ...   current_flag_column="CurrentRecord",
-        ...   record_creation_timestamp_column="record_available_at",
+        >>> # Declare the grocery customer table
+        >>> source_table = ds.get_table(  # doctest: +SKIP
+        ...   database_name="spark_catalog",
+        ...   schema_name="GROCERY",
+        ...   table_name="GROCERYCUSTOMER"
+        ... )
+        >>> customer_table = source_table.create_scd_table(  # doctest: +SKIP
+        ...    name="GROCERYCUSTOMER",
+        ...    surrogate_key_column='RowID',
+        ...    natural_key_column="GroceryCustomerGuid",
+        ...    effective_timestamp_column="ValidFrom",
+        ...    current_flag_column ="CurrentRecord",
+        ...    record_creation_timestamp_column="record_available_at"
         ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.scd_table import SCDTable
 
         return SCDTable.create(
             source_table=self,
@@ -949,15 +1001,20 @@
         self,
         name: str,
         sample_rows: Optional[int] = None,
         columns: Optional[list[str]] = None,
         columns_rename_mapping: Optional[dict[str, str]] = None,
     ) -> ObservationTable:
         """
-        Create an observation table from this source table.
+        Creates an ObservationTable from the SourceTable.
+
+        When you specify the columns and the columns_rename_mapping parameters, make sure that the table has:
+
+        - column(s) containing entity values with an accepted serving name.
+        - a column containing historical points-in-time in UTC. The column name must be "POINT_IN_TIME".
 
         Parameters
         ----------
         name: str
             Observation table name.
         sample_rows: Optional[int]
             Optionally sample the source table to this number of rows before creating the
@@ -978,17 +1035,21 @@
         >>> ds = fb.FeatureStore.get(<feature_store_name>).get_data_source()  # doctest: +SKIP
         >>> source_table = ds.get_source_table(  # doctest: +SKIP
         ...   database_name="<data_base_name>",
         ...   schema_name="<schema_name>",
         ...   table_name=<table_name>
         ... )
         >>> observation_table = source_table.create_observation_table(  # doctest: +SKIP
-        ...   "<observation_table_name>",
-        ...   sample_rows=10000,
-        ...   columns_rename_mapping={"timestamp": "POINT_IN_TIME"},
+        ...   name="<observation_table_name>",
+        ...   sample_rows=desired_sample_size,
+        ...   columns=[<timestamp_column_name>, <entity_column_name>],
+        ...   columns_rename_mapping={
+        ...     timestamp_column_name: "POINT_IN_TIME",
+        ...     entity_column_name: <entity_serving_name>,
+        ...   },
         ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.observation_table import ObservationTable
 
         payload = ObservationTableCreate(
             name=name,
@@ -1008,15 +1069,18 @@
     def create_batch_request_table(
         self,
         name: str,
         columns: Optional[list[str]] = None,
         columns_rename_mapping: Optional[dict[str, str]] = None,
     ) -> BatchRequestTable:
         """
-        Create a batch request table from this source table.
+        Creates an BatchRequestTable from the SourceTable.
+
+        When you specify the columns and the columns_rename_mapping parameters, make sure that the table has a column
+        containing entity values with an accepted serving name.
 
         Parameters
         ----------
         name: str
             Batch request table name.
         columns: Optional[list[str]]
             Include only these columns when creating the batch request table. If None, all columns
@@ -1024,14 +1088,28 @@
         columns_rename_mapping: Optional[dict[str, str]]
             Rename columns in the source table using this mapping from old column names to new
             column names when creating the batch request table. If None, no columns are renamed.
 
         Returns
         -------
         BatchRequestTable
+
+        Examples
+        --------
+        >>> data_source = fb.FeatureStore.get(<feature_store_name>).get_data_source()  # doctest: +SKIP
+        >>> source_table = data_source.get_source_table(  # doctest: +SKIP
+        ...   database_name="<data_base_name>",
+        ...   schema_name="<schema_name>",
+        ...   table_name=<table_name>
+        ... )
+        >>> batch_request_table = source_table.create_batch_request_table(  # doctest: +SKIP
+        ...   name="<batch_request_table_name>",
+        ...   columns=[<entity_column_name>],
+        ...   columns_rename_mapping={ <entity_column_name>: <entity_serving_name>, }
+        ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.batch_request_table import BatchRequestTable
 
         payload = BatchRequestTableCreate(
             name=name,
             feature_store_id=self.feature_store.id,
```

### Comparing `featurebyte-0.2.2/featurebyte/api/table.py` & `featurebyte-0.3.0/featurebyte/api/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,15 @@
         Any
             Retrieved table source
         """
         data = cls._get_by_id(id)
         data_class = cls._data_type_to_cls_mapping[data.cached_model.type]
         return data_class.get_by_id(id)
 
-    def info(  # pylint: disable=useless-parent-delegation
-        self, verbose: bool = False
-    ) -> Dict[str, Any]:
+    def info(self, verbose: bool = False) -> Dict[str, Any]:
         """
         Returns a dictionary that summarizes the essential information of a Table object, depending on its type.
         The dictionary contains the following common keys:
 
         - `name`: The name of the Table object.
         - `created_at`: The timestamp indicating when the Table object was created.
         - `updated_at`: The timestamp indicating when the Table object was last updated.
```

### Comparing `featurebyte-0.2.2/featurebyte/api/templates/online_serving/python.tpl` & `featurebyte-0.3.0/featurebyte/api/templates/online_serving/python.tpl`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/view.py` & `featurebyte-0.3.0/featurebyte/api/view.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,18 @@
 from featurebyte.logging import get_logger
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.batch_request_table import ViewBatchRequestInput
 from featurebyte.models.observation_table import ViewObservationInput
 from featurebyte.query_graph.enum import GraphNodeType, NodeOutputType, NodeType
 from featurebyte.query_graph.model.column_info import ColumnInfo
 from featurebyte.query_graph.node import Node
+from featurebyte.query_graph.node.cleaning_operation import (
+    CleaningOperation,
+    ColumnCleaningOperation,
+)
 from featurebyte.query_graph.node.generic import JoinMetadata, ProjectNode
 from featurebyte.query_graph.node.input import InputNode
 from featurebyte.query_graph.node.nested import BaseGraphNode
 from featurebyte.schema.batch_request_table import BatchRequestTableCreate
 from featurebyte.schema.observation_table import ObservationTableCreate
 
 if TYPE_CHECKING:
@@ -88,15 +92,54 @@
 
     @property
     def timestamp_column(self) -> Optional[str]:
         if not self._parent:
             return None
         return self._parent.timestamp_column
 
-    def sample(  # pylint: disable=useless-parent-delegation
+    @property
+    def cleaning_operations(self) -> Optional[List[CleaningOperation]]:
+        """
+        List of cleaning operations that were applied to this column during the view's creation.
+
+        Returns
+        -------
+        Optional[List[CleaningOperation]]
+            Returns None if the view column does not have parent. Otherwise, returns the list of cleaning operations.
+
+        Examples
+        --------
+        Show the list of cleaning operations of the event view amount column after updating the critical
+        data info of the event table.
+
+        >>> event_table = catalog.get_table("GROCERYINVOICE")
+        >>> event_table["Amount"].update_critical_data_info(
+        ...    cleaning_operations=[
+        ...        fb.MissingValueImputation(imputed_value=0),
+        ...    ]
+        ... )
+        >>> view = catalog.get_view("GROCERYINVOICE")
+        >>> view["Amount"].cleaning_operations
+        [MissingValueImputation(imputed_value=0, type=missing)]
+
+        Empty list of column cleaning operations of the event table amount column.
+
+        >>> event_table["Amount"].update_critical_data_info(cleaning_operations=[])
+        >>> event_table["Amount"].cleaning_operations
+        []
+        """
+        if not self.parent:
+            return None
+
+        for column_cleaning_operations in self.parent.column_cleaning_operations:
+            if column_cleaning_operations.column_name == self.name:
+                return cast(List[CleaningOperation], column_cleaning_operations.cleaning_operations)
+        return []
+
+    def sample(
         self,
         size: int = 10,
         seed: int = 1234,
         from_timestamp: Optional[Union[datetime, str]] = None,
         to_timestamp: Optional[Union[datetime, str]] = None,
         **kwargs: Any,
     ) -> pd.DataFrame:
@@ -128,27 +171,34 @@
         Sample 3 rows of a column.
         >>> catalog.get_view("GROCERYPRODUCT")["ProductGroup"].sample(3)
           ProductGroup
         0       Épices
         1         Chat
         2        Pains
 
+
+        Sample 3 rows of a column with timestamp.
+        >>> catalog.get_view("GROCERYINVOICE")["Amount"].sample(  # doctest: +SKIP
+        ...   size=3,
+        ...   seed=123,
+        ...   from_timestamp="2020-01-01",
+        ...   to_timestamp="2023-01-31"
+        ... )
+
         See Also
         --------
         - [ViewColumn.preview](/reference/featurebyte.api.view.ViewColumn.preview/):
           Retrieve a preview of a ViewColumn.
         - [ViewColumn.sample](/reference/featurebyte.api.view.ViewColumn.sample/):
           Retrieve a sample of a ViewColumn.
         """
         return super().sample(size, seed, from_timestamp, to_timestamp, **kwargs)
 
     @typechecked
-    def preview(  # pylint: disable=useless-parent-delegation
-        self, limit: int = 10, **kwargs: Any
-    ) -> pd.DataFrame:
+    def preview(self, limit: int = 10, **kwargs: Any) -> pd.DataFrame:
         """
         Returns a DataFrame that contains a selection of rows of the view column. The materialization process occurs
         after any cleaning operations that were defined either at the table level or during the view's creation.
 
         Parameters
         ----------
         limit: int
@@ -169,15 +219,15 @@
         0  10355516-5582-4358-b5f9-6e1ea7d5dc9f
         1  116c9284-2c41-446e-8eee-33901e0acdef
         2  3a45a5e8-1b71-42e8-b84e-43ddaf692375
         """
         return super().preview(limit=limit, **kwargs)
 
     @typechecked
-    def describe(  # pylint: disable=useless-parent-delegation
+    def describe(
         self,
         size: int = 0,
         seed: int = 1234,
         from_timestamp: Optional[Union[datetime, str]] = None,
         to_timestamp: Optional[Union[datetime, str]] = None,
         **kwargs: Any,
     ) -> pd.DataFrame:
@@ -211,14 +261,21 @@
         dtype                VARCHAR
         unique                    87
         %missing                 0.0
         %empty                     0
         entropy              4.13031
         top       Chips et Tortillas
         freq                  1319.0
+
+
+        Get summary of a column with timestamp.
+        >>> catalog.get_view("GROCERYINVOICE")["Amount"].describe(  # doctest: +SKIP
+        ...   from_timestamp="2020-01-01",
+        ...   to_timestamp="2023-01-31"
+        ... )
         """
         return super().describe(size, seed, from_timestamp, to_timestamp, **kwargs)
 
     @typechecked
     def as_feature(self, feature_name: str, offset: Optional[str] = None) -> Feature:
         """
         Creates a lookup feature directly from the column in the View.
@@ -239,14 +296,31 @@
         -------
         Feature
 
         Raises
         ------
         ValueError
             If the column is a temporary column not associated with any View
+
+        Examples
+        --------
+        >>> customer_view = catalog.get_view("GROCERYCUSTOMER")
+        >>> # Extract operating system from BrowserUserAgent column
+        >>> customer_view["OperatingSystemIsWindows"] = customer_view.BrowserUserAgent.str.contains("Windows")
+        >>> # Create a feature from the OperatingSystemIsWindows column
+        >>> uses_windows = customer_view.OperatingSystemIsWindows.as_feature("UsesWindows")
+
+
+        If the view is a Slowly Changing Dimension View, you may also consider to create a feature that retrieves the
+        entity's attribute at a point-in-time prior to the point-in-time specified in the feature request by specifying
+        an offset.
+
+        >>> uses_windows_12w_ago = customer_view.OperatingSystemIsWindows.as_feature(
+        ...   "UsesWindows_12w_ago", offset="12w"
+        ... )
         """
         view = self._parent
         if view is None:
             raise ValueError(
                 "as_feature is only supported for named columns in the View object. Consider"
                 " assigning the Feature to the View before calling as_feature()."
             )
@@ -256,15 +330,15 @@
             [input_column_name],
             [feature_name],
             offset=offset,
         )[feature_name]
         return cast(Feature, feature)
 
     @property
-    def is_datetime(self) -> bool:  # pylint: disable=useless-parent-delegation
+    def is_datetime(self) -> bool:
         """
         Returns whether the view column has a datetime data type.
 
         Returns
         -------
         bool
 
@@ -276,15 +350,15 @@
         True
         >>> print(view["Amount"].is_datetime)
         False
         """
         return super().is_datetime
 
     @property
-    def is_numeric(self) -> bool:  # pylint: disable=useless-parent-delegation
+    def is_numeric(self) -> bool:
         """
         Returns whether the view column has a numeric data type.
 
         Returns
         -------
         bool
 
@@ -296,17 +370,15 @@
         True
         >>> print(view["Timestamp"].is_numeric)
         False
         """
         return super().is_numeric
 
     @typechecked
-    def preview_sql(  # pylint: disable=useless-parent-delegation
-        self, limit: int = 10, **kwargs: Any
-    ) -> str:
+    def preview_sql(self, limit: int = 10, **kwargs: Any) -> str:
         """
         Returns an SQL query for previewing the column data after applying the set of cleaning operations defined
         at the column level.
 
         Parameters
         ----------
         limit: int
@@ -317,15 +389,15 @@
         Returns
         -------
         str
         """
         return super().preview_sql(limit=limit, **kwargs)
 
     @typechecked
-    def astype(  # pylint: disable=useless-parent-delegation
+    def astype(
         self: FrozenSeriesT,
         new_type: Union[Type[int], Type[float], Type[str], Literal["int", "float", "str"]],
     ) -> FrozenSeriesT:
         """
         Converts the data type of a column. It is useful when you need to convert column values between numerical and
         string formats, or the other way around.
 
@@ -339,24 +411,22 @@
         FrozenSeriesT
             A new Series with converted variable type.
 
         Examples
         --------
         Convert a numerical series to a string series, and back to an int series.
 
-        >>> event_view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> event_view = catalog.get_view("GROCERYINVOICE")
         >>> event_view["Amount"] = event_view["Amount"].astype(str)
         >>> event_view["Amount"] = event_view["Amount"].astype(int)
         """
         return super().astype(new_type=new_type)  # type: ignore[no-any-return,misc]
 
     @typechecked
-    def isin(  # pylint: disable=useless-parent-delegation
-        self: FrozenSeriesT, other: Union[FrozenSeries, ScalarSequence]
-    ) -> FrozenSeriesT:
+    def isin(self: FrozenSeriesT, other: Union[FrozenSeries, ScalarSequence]) -> FrozenSeriesT:
         """
         Identifies if each element is contained in a sequence of values represented by the `other` parameter.
 
         Parameters
         ----------
         other: Union[FrozenSeries, ScalarSequence]
             The sequence of values to check for membership. `other` can be a predefined list of values.
@@ -427,18 +497,46 @@
         - [GroupBy.aggregate](/reference/featurebyte.api.groupby.GroupBy.aggregate/):
         Create feature from grouped aggregates
         - [GroupBy.aggregate_over](/reference/featurebyte.api.groupby.GroupBy.aggregate_over/):
         Create features from grouped aggregates over different time windows
 
         Examples
         --------
-        Create GroupBy object from an event view
-        >>> transactions_view = transactions_data.get_view()  # doctest: +SKIP
-        >>> transactions_view.groupby("AccountID")  # doctest: +SKIP
-        GroupBy(EventView(node.name=input_1), keys=['AccountID'])
+        Groupby for Aggregate features.
+
+        >>> items_view = catalog.get_view("INVOICEITEMS")
+        >>> # Group items by the column GroceryCustomerGuid that references the customer entity
+        >>> items_by_customer = items_view.groupby("GroceryCustomerGuid")  # doctest: +SKIP
+        >>> # Declare features that measure the discount received by customer
+        >>> customer_discounts = items_by_customer.aggregate_over(  # doctest: +SKIP
+        ...   "Discount",
+        ...   method=fb.AggFunc.SUM,
+        ...   feature_names=["CustomerDiscounts_7d", "CustomerDiscounts_28d"],
+        ...   fill_value=0,
+        ...   windows=['7d', '28d']
+        ... )
+
+
+        Groupby for Cross Aggregate features.
+
+        >>> # Join product view to items view
+        >>> product_view = catalog.get_view("GROCERYPRODUCT")
+        >>> items_view = items_view.join(product_view)  # doctest: +SKIP
+        >>> # Group items by the column GroceryCustomerGuid that references the customer entity
+        >>> # And use ProductGroup as the column to perform operations across
+        >>> items_by_customer_across_product_group = items_view.groupby(  # doctest: +SKIP
+        ...   by_keys="GroceryCustomerGuid", category="ProductGroup"
+        ... )
+        >>> # Cross Aggregate feature of the customer purchases across product group over the past 4 weeks
+        >>> customer_inventory_28d = items_by_customer_across_product_group.aggregate_over(  # doctest: +SKIP
+        ...   "TotalCost",
+        ...   method=fb.AggFunc.SUM,
+        ...   feature_names=["CustomerInventory_28d"],
+        ...   windows=['28d']
+        ... )
         """
         # pylint: disable=import-outside-toplevel
         from featurebyte.api.groupby import GroupBy
 
         return GroupBy(obj=self, keys=by_keys, category=category)  # type: ignore
 
     def validate_aggregate_over_parameters(
@@ -478,15 +576,20 @@
     __fbautodoc__ = FBAutoDoc()
 
     _view_graph_node_type: ClassVar[GraphNodeType]
 
     @property
     def raw(self) -> FrozenFrame:
         """
-        Return the raw input table view (without any cleaning operations applied)
+        Return the raw input table view (without any cleaning operations applied).
+
+        Examples
+        --------
+        >>> items_view = catalog.get_view("INVOICEITEMS")
+        >>> items_view['Discount_missing'] = items_view.raw['Discount'].isnull()
 
         Returns
         -------
         FrozenFrame
         """
         view_input_node_names = []
         for graph_node in self.graph.iterate_nodes(target_node=self.node, node_type=NodeType.GRAPH):
@@ -544,28 +647,49 @@
     def __repr__(self) -> str:
         return f"{type(self).__name__}(node.name={self.node.name})"
 
     def __str__(self) -> str:
         return repr(self)
 
     @property
-    def columns(self) -> list[str]:  # pylint: disable=useless-parent-delegation
+    def columns(self) -> list[str]:
         """
         List the names of the columns in the view.
 
         Returns
         -------
         list[str]
         """
         return super().columns
 
+    @property
+    def column_cleaning_operations(self) -> List[ColumnCleaningOperation]:
+        """
+        List the cleaning operations associated with each column in the view during view creation.
+
+        Returns
+        -------
+        List[ColumnCleaningOperation]
+            List of column cleaning operations
+
+        See Also
+        --------
+        - [Table.columns_info](/reference/featurebyte.api.base_table.TableApiObject.columns_info)
+        - [TableColumn.update_critical_data_info](/reference/featurebyte.api.base_table.TableColumn.update_critical_data_info)
+        """
+        return [
+            ColumnCleaningOperation(
+                column_name=col.name, cleaning_operations=col.critical_data_info.cleaning_operations
+            )
+            for col in self.columns_info
+            if col.critical_data_info is not None and col.critical_data_info.cleaning_operations
+        ]
+
     @typechecked
-    def preview_sql(  # pylint: disable=useless-parent-delegation
-        self, limit: int = 10, **kwargs: Any
-    ) -> str:
+    def preview_sql(self, limit: int = 10, **kwargs: Any) -> str:
         """
         Returns an SQL query for previewing the view raw data after applying the set of cleaning operations defined
         at the column level.
 
         Parameters
         ----------
         limit: int
@@ -576,15 +700,15 @@
         Returns
         -------
         str
         """
         return super().preview_sql(limit=limit, **kwargs)
 
     @typechecked
-    def describe(  # pylint: disable=useless-parent-delegation
+    def describe(
         self,
         size: int = 0,
         seed: int = 1234,
         from_timestamp: Optional[Union[datetime, str]] = None,
         to_timestamp: Optional[Union[datetime, str]] = None,
         **kwargs: Any,
     ) -> pd.DataFrame:
@@ -618,21 +742,26 @@
         dtype                                  VARCHAR             VARCHAR
         unique                                   29099                  87
         %missing                                   0.0                 0.0
         %empty                                       0                   0
         entropy                               6.214608             4.13031
         top       017fe5ed-80a2-4e70-ae48-78aabfdee856  Chips et Tortillas
         freq                                       1.0              1319.0
+
+
+        Get summary of a view with timestamp.
+        >>> catalog.get_view("GROCERYINVOICE").describe(  # doctest: +SKIP
+        ...   from_timestamp=datetime(2019, 1, 1),
+        ...   to_timestamp=datetime(2019, 1, 31),
+        ... )
         """
         return super().describe(size, seed, from_timestamp, to_timestamp, **kwargs)
 
     @typechecked
-    def preview(  # pylint: disable=useless-parent-delegation
-        self, limit: int = 10, **kwargs: Any
-    ) -> pd.DataFrame:
+    def preview(self, limit: int = 10, **kwargs: Any) -> pd.DataFrame:
         """
         Returns a DataFrame that contains a selection of rows of the view. The materialization process occurs after
         any cleaning operations that were defined either at the table level or during the view's creation.
 
         Parameters
         ----------
         limit: int
@@ -652,15 +781,15 @@
                              GroceryProductGuid ProductGroup
         0  10355516-5582-4358-b5f9-6e1ea7d5dc9f      Glaçons
         1  116c9284-2c41-446e-8eee-33901e0acdef      Glaçons
         2  3a45a5e8-1b71-42e8-b84e-43ddaf692375      Glaçons
         """
         return super().preview(limit=limit, **kwargs)
 
-    def sample(  # pylint: disable=useless-parent-delegation
+    def sample(
         self,
         size: int = 10,
         seed: int = 1234,
         from_timestamp: Optional[Union[datetime, str]] = None,
         to_timestamp: Optional[Union[datetime, str]] = None,
         **kwargs: Any,
     ) -> pd.DataFrame:
@@ -686,20 +815,28 @@
         -------
         pd.DataFrame
             Sampled rows of the data.
 
         Examples
         --------
         Sample rows of a view.
-        >>> catalog.get_view("GROCERYPRODUCT").sample(3)
+        >>> catalog.get_view("GROCERYPRODUCT").sample(size=3)
                              GroceryProductGuid ProductGroup
         0  e890c5cb-689b-4caf-8e49-6b97bb9420c0       Épices
         1  5720e4df-2996-4443-a1bc-3d896bf98140         Chat
         2  96fc4d80-8cb0-4f1b-af01-e71ad7e7104a        Pains
 
+
+        Sample rows of a view with timestamp.
+        >>> catalog.get_view("GROCERYINVOICE").sample(  # doctest: +SKIP
+        ...   size=3,
+        ...   from_timestamp=datetime(2019, 1, 1),
+        ...   to_timestamp=datetime(2019, 1, 31),
+        ... )
+
         See Also
         --------
         - [View.preview](/reference/featurebyte.api.view.View.preview/):
           Retrieve a preview of a view.
         - [View.sample](/reference/featurebyte.api.view.View.sample/):
           Retrieve a sample of a view.
         """
@@ -1145,15 +1282,15 @@
             "left_on": left_on,
             "right_on": right_on,
             "left_input_columns": left_input_columns,
             "left_output_columns": left_output_columns,
             "right_input_columns": right_input_columns,
             "right_output_columns": right_output_columns,
             "join_type": how,
-            "metadata": JoinMetadata(on=on, rsuffix=rsuffix),
+            "metadata": JoinMetadata(rsuffix=rsuffix),
         }
         node_params.update(
             other_view._get_join_parameters(self)  # pylint: disable=protected-access
         )
 
         node = self.graph.add_operation(
             node_type=NodeType.JOIN,
@@ -1312,15 +1449,14 @@
 
         Returns
         -------
         FeatureGroup
 
         Examples
         --------
-        >>> import featurebyte as fb
         >>> features = dimension_view.as_features(  # doctest: +SKIP
         ...    column_names=["column_a", "column_b"],
         ...    feature_names=["Feature A", "Feature B"],
         ... )
         >>> features.feature_names  # doctest: +SKIP
         ['Feature A', 'Feature B']
         """
@@ -1376,15 +1512,20 @@
         self,
         name: str,
         sample_rows: Optional[int] = None,
         columns: Optional[list[str]] = None,
         columns_rename_mapping: Optional[dict[str, str]] = None,
     ) -> ObservationTable:
         """
-        Create an ObservationTable from the View.
+        Creates an ObservationTable from the View.
+
+        When you specify the columns and the columns_rename_mapping parameters, make sure that the table has:
+
+        - a column containing entity values with an accepted serving name.
+        - a column containing historical points-in-time in UTC. The column name must be "POINT-IN-TIME".
 
         Parameters
         ----------
         name: str
             Name of the ObservationTable.
         sample_rows: Optional[int]
             Optionally sample the source table to this number of rows before creating the
@@ -1430,15 +1571,18 @@
     def create_batch_request_table(
         self,
         name: str,
         columns: Optional[list[str]] = None,
         columns_rename_mapping: Optional[dict[str, str]] = None,
     ) -> BatchRequestTable:
         """
-        Create a BatchRequestTable from the View.
+        Creates an BatchRequestTable from the View.
+
+        When you specify the columns and the columns_rename_mapping parameters, make sure that the table has a
+        column containing entity values with an accepted serving name.
 
         Parameters
         ----------
         name: str
             Name of the BatchRequestTable.
         columns: Optional[list[str]]
             Include only these columns in the view when creating the batch request table. If None,
@@ -1447,14 +1591,24 @@
             Rename columns in the view using this mapping from old column names to new column names
             when creating the batch request table. If None, no columns are renamed.
 
         Returns
         -------
         BatchRequestTable
             BatchRequestTable object.
+
+        Examples
+        --------
+        >>> batch_request_table = view.create_batch_request_table(  # doctest: +SKIP
+        ...   name="<batch_request_table_name>",
+        ...   columns=[<entity_column_name>],
+        ...   columns_rename_mapping={
+        ...     <entity_column_name>: <entity_serving_name>,
+        ...   }
+        ... )
         """
         pruned_graph, mapped_node = self.extract_pruned_graph_and_node()
         payload = BatchRequestTableCreate(
             name=name,
             feature_store_id=self.feature_store.id,
             request_input=ViewBatchRequestInput(
                 graph=pruned_graph,
```

### Comparing `featurebyte-0.2.2/featurebyte/api/window_aggregator.py` & `featurebyte-0.3.0/featurebyte/api/window_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/api/window_validator.py` & `featurebyte-0.3.0/featurebyte/api/window_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/app.py` & `featurebyte-0.3.0/featurebyte/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/date_util.py` & `featurebyte-0.3.0/featurebyte/common/date_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/descriptor.py` & `featurebyte-0.3.0/featurebyte/common/descriptor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/dict_util.py` & `featurebyte-0.3.0/featurebyte/common/dict_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/doc_util.py` & `featurebyte-0.3.0/featurebyte/common/doc_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/allowed_classes.py` & `featurebyte-0.3.0/featurebyte/common/documentation/allowed_classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 Allowed classes module.
 
 A temporary hack to allow parameter descriptions to be parsed correctly.
 """
 
 nested_description_allowed_classes = {
     "accesstokencredential",
+    "azureblobstoragecredential",
     "columncleaningoperation",
     "databricksdetails",
     "disguisedvalueimputation",
     "featuregroup",
     "featurejobsetting",
     "featureversioninfo",
+    "gcsstoragecredential",
     "missingvalueimputation",
     "snowflakedetails",
     "sparkdetails",
     "stringvalueimputation",
     "s3storagecredential",
     "tablecleaningoperation",
     "tablefeaturejobsetting",
```

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/autodoc_processor.py` & `featurebyte-0.3.0/featurebyte/common/documentation/autodoc_processor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/constants.py` & `featurebyte-0.3.0/featurebyte/common/documentation/constants.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/custom_nav.py` & `featurebyte-0.3.0/featurebyte/common/documentation/custom_nav.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/doc_types.py` & `featurebyte-0.3.0/featurebyte/common/documentation/doc_types.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/documentation_layout.py` & `featurebyte-0.3.0/featurebyte/common/documentation/documentation_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
     # we want to point users to a hand-written overview document. If this is true, you should also provide a
     # core_doc_path_override. It is likely that doc_path_override will be unused if `is_core_object` is set to true.
     is_core_object: Optional[bool] = False
     # The path to the core object documentation. This should be a path to a markdown file found in the `core` folder in
     # the documentation repo.
     core_doc_path_override: Optional[str] = None
 
+    # Used to flag pure methods that aren't part of a class.
+    is_pure_method: Optional[bool] = False
+
     def get_api_path_override(self) -> str:
         if not self.menu_header:
             return ""
         return "featurebyte." + self.menu_header[-1]
 
     def get_doc_path_override(self) -> Optional[str]:
         if self.doc_path_override is None:
@@ -102,14 +105,18 @@
     Returns
     -------
     List[DocLayoutItem]
         The layout for the data module.
     """
     return [
         DocLayoutItem([TABLE]),
+        DocLayoutItem([TABLE, CLASS_METHODS, "EventTable.get_by_id"]),
+        DocLayoutItem([TABLE, CLASS_METHODS, "DimensionTable.get_by_id"]),
+        DocLayoutItem([TABLE, CLASS_METHODS, "SCDTable.get_by_id"]),
+        DocLayoutItem([TABLE, CLASS_METHODS, "ItemTable.get_by_id"]),
         DocLayoutItem(
             [TABLE, SET_FEATURE_JOB, "EventTable.create_new_feature_job_setting_analysis"]
         ),
         DocLayoutItem(
             [TABLE, SET_FEATURE_JOB, "EventTable.initialize_default_feature_job_setting"]
         ),
         DocLayoutItem([TABLE, SET_FEATURE_JOB, "EventTable.list_feature_job_setting_analysis"]),
@@ -214,14 +221,15 @@
         DocLayoutItem([TABLE_COLUMN]),
         DocLayoutItem([TABLE_COLUMN, ADD_METADATA, "TableColumn.as_entity"]),
         DocLayoutItem([TABLE_COLUMN, ADD_METADATA, "TableColumn.update_critical_data_info"]),
         DocLayoutItem([TABLE_COLUMN, EXPLORE, "TableColumn.describe"]),
         DocLayoutItem([TABLE_COLUMN, EXPLORE, "TableColumn.preview"]),
         DocLayoutItem([TABLE_COLUMN, EXPLORE, "TableColumn.sample"]),
         DocLayoutItem([TABLE_COLUMN, INFO, "TableColumn.name"]),
+        DocLayoutItem([TABLE_COLUMN, INFO, "TableColumn.cleaning_operations"]),
         DocLayoutItem([TABLE_COLUMN, LINEAGE, "TableColumn.preview_sql"]),
     ]
 
 
 def _get_entity_layout() -> List[DocLayoutItem]:
     """
     Returns the layout for the entity documentation
@@ -237,14 +245,15 @@
         DocLayoutItem([ENTITY, INFO, "Entity.info"]),
         DocLayoutItem([ENTITY, INFO, "Entity.name"]),
         DocLayoutItem([ENTITY, INFO, "Entity.name_history"]),
         DocLayoutItem([ENTITY, INFO, "Entity.parents"]),
         DocLayoutItem([ENTITY, INFO, "Entity.serving_names"]),
         DocLayoutItem([ENTITY, INFO, "Entity.updated_at"]),
         DocLayoutItem([ENTITY, LINEAGE, "Entity.id"]),
+        DocLayoutItem([ENTITY, LINEAGE, "Entity.catalog_id"]),
         DocLayoutItem([ENTITY, MANAGE, "Entity.update_name"]),
     ]
 
 
 def _get_feature_layout() -> List[DocLayoutItem]:
     """
     Returns the layout for the feature documentation
@@ -268,21 +277,20 @@
         DocLayoutItem([FEATURE, INFO, "Feature.is_datetime"]),
         DocLayoutItem([FEATURE, INFO, "Feature.is_numeric"]),
         DocLayoutItem([FEATURE, INFO, "Feature.is_default"]),
         DocLayoutItem([FEATURE, INFO, "Feature.version"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.entity_ids"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.primary_entity"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.feature_list_ids"]),
-        DocLayoutItem([FEATURE, LINEAGE, "Feature.feature_namespace_id"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.feature_store"]),
-        DocLayoutItem([FEATURE, LINEAGE, "Feature.graph"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.id"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.definition"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.sql"]),
         DocLayoutItem([FEATURE, LINEAGE, "Feature.catalog_id"]),
+        DocLayoutItem([FEATURE, MANAGE, "Feature.delete"]),
         DocLayoutItem([FEATURE, MANAGE, "Feature.get_feature_jobs_status"]),
         DocLayoutItem([FEATURE, MANAGE, "Feature.as_default_version"]),
         DocLayoutItem([FEATURE, MANAGE, "Feature.create_new_version"]),
         DocLayoutItem([FEATURE, MANAGE, "Feature.list_versions"]),
         DocLayoutItem([FEATURE, MANAGE, "Feature.update_default_version_mode"]),
         DocLayoutItem([FEATURE, MANAGE, "Feature.update_readiness"]),
         DocLayoutItem([FEATURE, TRANSFORM, "Feature.abs"]),
@@ -351,40 +359,42 @@
         The layout for the FeatureList class.
     """
     return [
         DocLayoutItem([FEATURE_LIST]),
         DocLayoutItem([FEATURE_LIST, CONSTRUCTOR, "FeatureList"]),
         DocLayoutItem([FEATURE_LIST, CREATE_FEATURE_GROUP, "FeatureList.drop"]),
         DocLayoutItem([FEATURE_LIST, DEPLOY, "FeatureList.deploy"]),
-        DocLayoutItem([FEATURE_LIST, DEPLOY, "FeatureList.compute_historical_feature_table"]),
         DocLayoutItem([FEATURE_LIST, SAVE, "FeatureList.save"]),
         DocLayoutItem([FEATURE_LIST, EXPLORE, "FeatureList.preview"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.created_at"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.feature_names"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.info"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.list_features"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.name"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.saved"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.status"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.updated_at"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.is_default"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.production_ready_fraction"]),
+        DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.default_feature_fraction"]),
         DocLayoutItem([FEATURE_LIST, INFO, "FeatureList.version"]),
         DocLayoutItem([FEATURE_LIST, LINEAGE, "FeatureList.catalog_id"]),
         DocLayoutItem([FEATURE_LIST, LINEAGE, "FeatureList.feature_ids"]),
         DocLayoutItem([FEATURE_LIST, LINEAGE, "FeatureList.id"]),
         DocLayoutItem([FEATURE_LIST, LINEAGE, "FeatureList.sql"]),
         DocLayoutItem([FEATURE_LIST, LINEAGE, "FeatureList.primary_entity"]),
         DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.get_feature_jobs_status"]),
+        DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.delete"]),
         DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.as_default_version"]),
         DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.create_new_version"]),
         DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.list_versions"]),
         DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.update_default_version_mode"]),
         DocLayoutItem([FEATURE_LIST, MANAGE, "FeatureList.update_status"]),
         DocLayoutItem([FEATURE_LIST, SERVE, "FeatureList.compute_historical_features"]),
+        DocLayoutItem([FEATURE_LIST, SERVE, "FeatureList.compute_historical_feature_table"]),
     ]
 
 
 def _get_feature_store_layout() -> List[DocLayoutItem]:
     """
     The layout for the FeatureStore class.
 
@@ -441,14 +451,15 @@
     return [
         DocLayoutItem([RELATIONSHIP]),
         DocLayoutItem([RELATIONSHIP, INFO, "Relationship.created_at"]),
         DocLayoutItem([RELATIONSHIP, INFO, "Relationship.info"]),
         DocLayoutItem([RELATIONSHIP, INFO, "Relationship.name"]),
         DocLayoutItem([RELATIONSHIP, INFO, "Relationship.updated_at"]),
         DocLayoutItem([RELATIONSHIP, LINEAGE, "Relationship.id"]),
+        DocLayoutItem([RELATIONSHIP, LINEAGE, "Relationship.catalog_id"]),
         DocLayoutItem([RELATIONSHIP, MANAGE, "Relationship.enable"]),
         DocLayoutItem([RELATIONSHIP, MANAGE, "Relationship.disable"]),
     ]
 
 
 def _get_view_layout() -> List[DocLayoutItem]:
     """
@@ -487,14 +498,15 @@
         DocLayoutItem([VIEW, INFO, "SCDView.current_flag_column"]),
         DocLayoutItem([VIEW, INFO, "SCDView.effective_timestamp_column"]),
         DocLayoutItem([VIEW, INFO, "SCDView.end_timestamp_column"]),
         DocLayoutItem([VIEW, INFO, "SCDView.natural_key_column"]),
         DocLayoutItem([VIEW, INFO, "SCDView.surrogate_key_column"]),
         DocLayoutItem([VIEW, INFO, "View.columns"]),
         DocLayoutItem([VIEW, INFO, "View.columns_info"]),
+        DocLayoutItem([VIEW, INFO, "View.column_cleaning_operations"]),
         DocLayoutItem([VIEW, INFO, "View.dtypes"]),
         DocLayoutItem([VIEW, INFO, "View.entity_columns"]),
         DocLayoutItem([VIEW, INFO, "View.timestamp_column"]),
         DocLayoutItem([VIEW, INFO, "View.get_join_column"]),
         DocLayoutItem([VIEW, LINEAGE, "View.feature_store"]),
         DocLayoutItem([VIEW, LINEAGE, "View.preview_sql"]),
         DocLayoutItem([VIEW, TYPE, "ChangeView"]),
@@ -553,14 +565,15 @@
         DocLayoutItem([VIEW_COLUMN, EXPLORE, "ViewColumn.describe"]),
         DocLayoutItem([VIEW_COLUMN, EXPLORE, "ViewColumn.preview"]),
         DocLayoutItem([VIEW_COLUMN, EXPLORE, "ViewColumn.sample"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.dtype"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.is_datetime"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.is_numeric"]),
         DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.name"]),
+        DocLayoutItem([VIEW_COLUMN, INFO, "ViewColumn.cleaning_operations"]),
         DocLayoutItem([VIEW_COLUMN, LAGS, "ChangeViewColumn.lag"]),
         DocLayoutItem([VIEW_COLUMN, LAGS, "EventViewColumn.lag"]),
         DocLayoutItem([VIEW_COLUMN, LINEAGE, "ViewColumn.feature_store"]),
         DocLayoutItem([VIEW_COLUMN, LINEAGE, "ViewColumn.preview_sql"]),
         DocLayoutItem([VIEW_COLUMN, TRANSFORM, "ViewColumn.astype"]),
         DocLayoutItem([VIEW_COLUMN, TRANSFORM, "ViewColumn.abs"]),
         DocLayoutItem([VIEW_COLUMN, TRANSFORM, "ViewColumn.ceil"]),
@@ -656,14 +669,20 @@
     List[DocLayoutItem]
         The layout for the utility methods used in featurebyte.
     """
     return [
         DocLayoutItem(
             [UTILITY_METHODS, TRANSFORM, "to_timedelta"],
             doc_path_override="core.timedelta.to_timedelta.md",
+            is_pure_method=True,
+        ),
+        DocLayoutItem(
+            [UTILITY_METHODS, LIST, "list_unsaved_features"],
+            doc_path_override="feature_utility.list_unsaved_features.md",
+            is_pure_method=True,
         ),
     ]
 
 
 def _get_utility_classes_layout() -> List[DocLayoutItem]:
     """
     The layout for the utility classes used in featurebyte.
@@ -704,14 +723,16 @@
         ),
         DocLayoutItem([UTILITY_CLASSES, FEATURE, "FeatureVersionInfo"]),
         DocLayoutItem([UTILITY_CLASSES, WAREHOUSE, "DatabricksDetails"]),
         DocLayoutItem([UTILITY_CLASSES, WAREHOUSE, "SnowflakeDetails"]),
         DocLayoutItem([UTILITY_CLASSES, WAREHOUSE, "SparkDetails"]),
         DocLayoutItem([UTILITY_CLASSES, CREDENTIAL]),
         DocLayoutItem([UTILITY_CLASSES, CREDENTIAL, "AccessTokenCredential"]),
+        DocLayoutItem([UTILITY_CLASSES, CREDENTIAL, "AzureBlobStorageCredential"]),
+        DocLayoutItem([UTILITY_CLASSES, CREDENTIAL, "GCSStorageCredential"]),
         DocLayoutItem([UTILITY_CLASSES, CREDENTIAL, "S3StorageCredential"]),
         DocLayoutItem([UTILITY_CLASSES, CREDENTIAL, "UsernamePasswordCredential"]),
         DocLayoutItem([UTILITY_CLASSES, REQUEST_COLUMN, "RequestColumn.point_in_time"]),
     ]
 
 
 def _get_source_table_layout() -> List[DocLayoutItem]:
@@ -812,14 +833,16 @@
         # DocLayoutItem([BATCH_FEATURE_TABLE, INFO, "BatchFeatureTable.batch_request_table_name"]),
         DocLayoutItem([BATCH_FEATURE_TABLE, INFO, "BatchFeatureTable.name"]),
         DocLayoutItem([BATCH_FEATURE_TABLE, INFO, "BatchFeatureTable.created_at"]),
         DocLayoutItem([BATCH_FEATURE_TABLE, INFO, "BatchFeatureTable.updated_at"]),
         DocLayoutItem([BATCH_FEATURE_TABLE, LINEAGE, "BatchFeatureTable.batch_request_table_id"]),
         DocLayoutItem([BATCH_FEATURE_TABLE, LINEAGE, "BatchFeatureTable.deployment_id"]),
         DocLayoutItem([BATCH_FEATURE_TABLE, LINEAGE, "BatchFeatureTable.id"]),
+        DocLayoutItem([BATCH_FEATURE_TABLE, MANAGE, "BatchFeatureTable.download"]),
+        DocLayoutItem([BATCH_FEATURE_TABLE, MANAGE, "BatchFeatureTable.delete"]),
     ]
 
 
 def _get_observation_table_layout() -> List[DocLayoutItem]:
     """
     The layout for the ObservationTable module.
 
@@ -836,14 +859,17 @@
         DocLayoutItem([OBSERVATION_TABLE, INFO, "ObservationTable.name"]),
         DocLayoutItem([OBSERVATION_TABLE, INFO, "ObservationTable.context_id"]),
         # DocLayoutItem([OBSERVATION_TABLE, INFO, "ObservationTable.type"]),
         # DocLayoutItem([OBSERVATION_TABLE, INFO, "ObservationTable.feature_store_name"]),
         DocLayoutItem([OBSERVATION_TABLE, INFO, "ObservationTable.created_at"]),
         DocLayoutItem([OBSERVATION_TABLE, INFO, "ObservationTable.updated_at"]),
         DocLayoutItem([OBSERVATION_TABLE, LINEAGE, "ObservationTable.id"]),
+        DocLayoutItem([OBSERVATION_TABLE, MANAGE, "ObservationTable.download"]),
+        DocLayoutItem([OBSERVATION_TABLE, MANAGE, "ObservationTable.delete"]),
+        DocLayoutItem([OBSERVATION_TABLE, MANAGE, "ObservationTable.to_pandas"]),
     ]
 
 
 def _get_batch_request_table_layout() -> List[DocLayoutItem]:
     """
     The layout for the BatchRequestTable module.
 
@@ -860,14 +886,17 @@
         DocLayoutItem([BATCH_REQUEST_TABLE, INFO, "BatchRequestTable.context_id"]),
         # DocLayoutItem([BATCH_REQUEST_TABLE, INFO, "BatchRequestTable.type"]),
         # DocLayoutItem([BATCH_REQUEST_TABLE, INFO, "BatchRequestTable.feature_store_name"]),
         DocLayoutItem([BATCH_REQUEST_TABLE, INFO, "BatchRequestTable.name"]),
         DocLayoutItem([BATCH_REQUEST_TABLE, INFO, "BatchRequestTable.created_at"]),
         DocLayoutItem([BATCH_REQUEST_TABLE, INFO, "BatchRequestTable.updated_at"]),
         DocLayoutItem([BATCH_REQUEST_TABLE, LINEAGE, "BatchRequestTable.id"]),
+        DocLayoutItem([BATCH_REQUEST_TABLE, MANAGE, "BatchRequestTable.download"]),
+        DocLayoutItem([BATCH_REQUEST_TABLE, MANAGE, "BatchRequestTable.delete"]),
+        DocLayoutItem([BATCH_REQUEST_TABLE, MANAGE, "BatchRequestTable.to_pandas"]),
     ]
 
 
 def _get_historical_feature_table_layout() -> List[DocLayoutItem]:
     """
     The layout for the HistoricalFeatureTable module.
 
@@ -882,14 +911,16 @@
         DocLayoutItem([HISTORICAL_FEATURE_TABLE, EXPLORE, "HistoricalFeatureTable.preview"]),
         DocLayoutItem([HISTORICAL_FEATURE_TABLE, EXPLORE, "HistoricalFeatureTable.sample"]),
         DocLayoutItem([HISTORICAL_FEATURE_TABLE, INFO, "HistoricalFeatureTable.name"]),
         # DocLayoutItem([HISTORICAL_FEATURE_TABLE, INFO, "HistoricalFeatureTable.feature_store_name"]),
         # DocLayoutItem([HISTORICAL_FEATURE_TABLE, INFO, "HistoricalFeatureTable.observation_table_name"]),
         DocLayoutItem([HISTORICAL_FEATURE_TABLE, INFO, "HistoricalFeatureTable.created_at"]),
         DocLayoutItem([HISTORICAL_FEATURE_TABLE, INFO, "HistoricalFeatureTable.updated_at"]),
+        DocLayoutItem([HISTORICAL_FEATURE_TABLE, MANAGE, "HistoricalFeatureTable.download"]),
+        DocLayoutItem([HISTORICAL_FEATURE_TABLE, MANAGE, "HistoricalFeatureTable.delete"]),
         DocLayoutItem(
             [HISTORICAL_FEATURE_TABLE, LINEAGE, "HistoricalFeatureTable.feature_list_id"]
         ),
         DocLayoutItem([HISTORICAL_FEATURE_TABLE, LINEAGE, "HistoricalFeatureTable.id"]),
         DocLayoutItem(
             [HISTORICAL_FEATURE_TABLE, LINEAGE, "HistoricalFeatureTable.observation_table_id"]
         ),
```

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/extract_csv.py` & `featurebyte-0.3.0/featurebyte/common/documentation/extract_csv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Extract documentation into a CSV file.
 """
-from typing import Dict, List
+from typing import Dict, List, Literal
 
 import csv
 from dataclasses import dataclass
 
 from featurebyte.common.documentation.doc_types import DocItems
 from featurebyte.common.documentation.documentation_layout import get_overall_layout
 from featurebyte.common.documentation.gen_ref_pages_docs_builder import (
@@ -26,51 +26,57 @@
     """
     DocItemToRender is a dataclass to capture what we're going to be writing to the CSV.
 
     Each field is a column in the CSV.
     """
 
     menu_item: str
+    # eg. class, method, property
+    item_type: Literal["class", "property", "method", "missing"]
     # eg. FeatureStore, FeatureStore.list
     class_method_or_attribute: str
-    # ilnk to docs, eg: http://127.0.0.1:8000/reference/featurebyte.api.feature_store.FeatureStore/
+    # link to docs, eg: http://127.0.0.1:8000/reference/featurebyte.api.feature_store.FeatureStore/
     link: str
     # the current docstring
     docstring_description: str
 
     parameters: str
     returns: str
     raises: str
     examples: str
     see_also: str
 
 
-def get_resource_details_for_path(path: str) -> ResourceDetails:
+def get_resource_details_for_path(path: str, is_pure_method: bool) -> ResourceDetails:
     """
     Get the resource details for a given path.
 
     This is typically only used for documentation items that have an explicit file override.
 
     Parameters
     ----------
     path: str
         The path to get the resource details for
+    is_pure_method: bool
+        Whether the path is a pure method or not
 
     Returns
     -------
     ResourceDetails
         The resource details for the given path
     """
     split_path = path.split(".")
     # this is for instances where the override is a class
     # eg. "api.groupby.GroupBy"
     if split_path[-1][0].isupper():
         return get_resource_details(path)
 
     class_description = ".".join(split_path[:-1])
+    if is_pure_method:
+        return get_resource_details(f"{class_description}!!{split_path[-1]}")
     return get_resource_details(f"{class_description}::{split_path[-1]}")
 
 
 def extract_details_for_rendering(resource_details: ResourceDetails) -> Dict[str, str]:
     """
     Extract the details for rendering.
 
@@ -155,40 +161,45 @@
     logger.info("Building items to generate")
     all_doc_items_to_generate: List[DocItemToRender] = []
     for layout_item in get_overall_layout():
         doc_path_override = layout_item.get_doc_path_override()
         if doc_path_override is not None:
             # handle those with explicit overrides
             link_without_md = doc_path_override.replace(".md", "")
-            resource_details = get_resource_details_for_path(link_without_md)
+            resource_details = get_resource_details_for_path(
+                link_without_md, bool(layout_item.is_pure_method)
+            )
             all_doc_items_to_generate.append(
                 DocItemToRender(
                     menu_item=" > ".join(layout_item.menu_header),
+                    item_type=resource_details.type,
                     class_method_or_attribute=link_without_md,
                     link=f"http://127.0.0.1:8000/reference/{link_without_md}",
                     **extract_details_for_rendering(resource_details),
                 )
             )
             continue
         doc_item = doc_items.get(layout_item.get_api_path_override())
         if doc_item is not None:
             all_doc_items_to_generate.append(
                 DocItemToRender(
                     menu_item=" > ".join(layout_item.menu_header),
+                    item_type=doc_item.resource_details.type,
                     class_method_or_attribute=doc_item.class_method_or_attribute,
                     link=doc_item.link,
                     **extract_details_for_rendering(doc_item.resource_details),
                 )
             )
             continue
 
         # If we don't find a doc item, add a placeholder.
         all_doc_items_to_generate.append(
             DocItemToRender(
                 menu_item=" > ".join(layout_item.menu_header),
+                item_type="missing",
                 class_method_or_attribute="missing",
                 link="missing",
                 docstring_description="missing",
                 parameters="missing",
                 returns="missing",
                 raises="missing",
                 examples="missing",
```

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/formatters.py` & `featurebyte-0.3.0/featurebyte/common/documentation/formatters.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/gen_ref_pages_docs_builder.py` & `featurebyte-0.3.0/featurebyte/common/documentation/gen_ref_pages_docs_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,34 +346,46 @@
 
     Returns
     -------
     Dict[str, Any]
         Dict mapping an accessor to its metadata.
     """
     return {
-        "StringAccessor": AccessorMetadata(
+        # Must include `string` prefix to avoid conflict with the `FeatureStringAccessor`.
+        "string.StringAccessor": AccessorMetadata(
             classes_using_accessor=[
-                "featurebyte.Feature",
                 "featurebyte.ViewColumn",
             ],
             property_name="str",
         ),
+        "FeatureStringAccessor": AccessorMetadata(
+            classes_using_accessor=[
+                "featurebyte.Feature",
+            ],
+            property_name="str",
+        ),
         "CountDictAccessor": AccessorMetadata(
             classes_using_accessor=[
                 "featurebyte.Feature",
             ],
             property_name="cd",
         ),
-        "DatetimeAccessor": AccessorMetadata(
+        # Must include `datetime` prefix to avoid conflict with the `FeatureDatetimeAccessor`.
+        "datetime.DatetimeAccessor": AccessorMetadata(
             classes_using_accessor=[
-                "featurebyte.Feature",
                 "featurebyte.ViewColumn",
             ],
             property_name="dt",
         ),
+        "FeatureDatetimeAccessor": AccessorMetadata(
+            classes_using_accessor=[
+                "featurebyte.Feature",
+            ],
+            property_name="dt",
+        ),
     }
 
 
 def build_markdown_format_str(obj_path: str, obj_type: str, api_to_use: str) -> str:
     """
     Build the markdown format string for the given object path.
 
@@ -521,24 +533,30 @@
         The doc groups.
 
     Returns
     -------
     Dict[DocGroupKey, DocGroupValue]
         The doc groups.
     """
-    doc_groups[
-        DocGroupKey(
-            module_path="featurebyte.core.timedelta",
-            attribute_name="to_timedelta",
+    methods = [
+        ("featurebyte.core.timedelta", "to_timedelta"),
+        ("featurebyte.feature_utility", "list_unsaved_features"),
+    ]
+    for method in methods:
+        doc_groups[
+            DocGroupKey(
+                module_path=method[0],
+                attribute_name=method[1],
+            )
+        ] = DocGroupValue(
+            doc_group=[],
+            obj_type="method",
+            proxy_path="",
         )
-    ] = DocGroupValue(
-        doc_group=[],
-        obj_type="method",
-        proxy_path="",
-    )
+
     return doc_groups
 
 
 def get_doc_groups() -> Dict[DocGroupKey, DocGroupValue]:
     """
     This returns a dictionary of doc groups.
 
@@ -766,15 +784,19 @@
             The local path.
         output: str
             The output to write.
         """
         with self.gen_files_open(filepath, "w") as fd:
             fd.writelines(output)
         if DEBUG_MODE:
-            with open(f"debug/{local_path}_local.txt", "w") as local_file:
+            debug_folder = "debug"
+            file_exists = os.path.exists(debug_folder)
+            if not file_exists:
+                os.makedirs(debug_folder)
+            with open(f"{debug_folder}/{local_path}_local.txt", "w") as local_file:
                 local_file.writelines(output)
 
     def _build_and_write_to_file(
         self,
         metadata: MarkdownFileMetadata,
     ) -> None:
         """
```

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/markdown_extension/extension.py` & `featurebyte-0.3.0/featurebyte/common/documentation/markdown_extension/extension.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/pydantic_field_docs.py` & `featurebyte-0.3.0/featurebyte/common/documentation/pydantic_field_docs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/resource_extractor.py` & `featurebyte-0.3.0/featurebyte/common/documentation/resource_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -250,14 +250,45 @@
                 default=format_literal(raw_parameter_detail.param_default),
                 description=parameters_desc.get(param_name),
             )
         )
     return details
 
 
+def _get_docstring_for_resource(resource: Any) -> Docstring:
+    """
+    Get docstring for resource.
+
+    Filters out comment lines in block docstrings that start with `# noqa` which is typically used to skip some
+    lint checks.
+
+    Parameters
+    ----------
+    resource: Any
+        Resource
+
+    Returns
+    -------
+    Docstring
+    """
+    docstring = getattr(resource, "__doc__", "")
+    if not docstring:
+        docs = ""
+    else:
+        split_string = docstring.split("\n")
+        filtered_string = []
+        for string in split_string:
+            stripped_string = string.strip()
+            if stripped_string.startswith("# noqa"):
+                continue
+            filtered_string.append(string)
+        docs = trim_docstring("\n".join(filtered_string))
+    return Docstring(parse(docs))
+
+
 def _get_resource_detail_for_pure_fn(resource_descriptor: str) -> ResourceDetails:
     """
     Extract a resource detail for a pure function.
 
     Parameters
     ----------
     resource_descriptor: str
@@ -270,24 +301,22 @@
 
     Returns
     -------
     ResourceDetails
     """
     if "!!" not in resource_descriptor:
         raise ValueError(f"Invalid resource descriptor: {resource_descriptor}")
-
     parts = resource_descriptor.split("!!")
     module_path = parts[0]
     method_name = parts[1]
 
     resource = import_from_string(module_path)
     method_resource = getattr(resource, method_name)
 
-    docs = trim_docstring(getattr(method_resource, "__doc__", ""))
-    docstring = Docstring(parse(docs))
+    docstring = _get_docstring_for_resource(method_resource)
 
     # process signature
     parameters, return_type = get_params_from_signature(method_resource)
     parameters_desc = (
         {param.arg_name: param.description for param in docstring.params if param.description}
         if docstring.params
         else {}
@@ -383,16 +412,15 @@
     if autodoc_config.proxy_class:
         proxy_path = autodoc_config.proxy_class
 
     # process signature
     parameters, return_type = get_params_from_signature(resource)
 
     # process docstring
-    docs = trim_docstring(getattr(resource, "__doc__", ""))
-    docstring = Docstring(parse(docs))
+    docstring = _get_docstring_for_resource(resource)
 
     # get parameter description from docstring
     short_description = docstring.short_description
     if getattr(resource, "field_info", None):
         short_description = resource.field_info.description
         if resource_class.__name__ in pydantic_field_doc_overrides:
             override = pydantic_field_doc_overrides[resource_class.__name__]
```

### Comparing `featurebyte-0.2.2/featurebyte/common/documentation/resource_util.py` & `featurebyte-0.3.0/featurebyte/common/documentation/resource_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/env_util.py` & `featurebyte-0.3.0/featurebyte/common/env_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/join_utils.py` & `featurebyte-0.3.0/featurebyte/common/join_utils.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/model_util.py` & `featurebyte-0.3.0/featurebyte/common/model_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/path_util.py` & `featurebyte-0.3.0/featurebyte/common/path_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/tile_util.py` & `featurebyte-0.3.0/featurebyte/common/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/typing.py` & `featurebyte-0.3.0/featurebyte/common/typing.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/common/utils.py` & `featurebyte-0.3.0/featurebyte/common/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 from io import BytesIO
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
-import pygments
 from alive_progress import alive_bar
 from dateutil import parser
-from pygments.formatters.html import HtmlFormatter
 from requests import Response
 
 from featurebyte.common.env_util import get_alive_bar_additional_params
 from featurebyte.enum import DBVarType, InternalName
 
 
 class ResponseStream:
@@ -398,25 +396,7 @@
     """
     output = []
     if isinstance(value, str):
         output = [value]
     if isinstance(value, list):
         output = value
     return output
-
-
-class CodeStr(str):
-    """
-    Code string content that can be displayed in markdown format
-    """
-
-    def _repr_html_(self) -> str:
-        lexer = pygments.lexers.get_lexer_by_name("python")
-        highlighted_code = pygments.highlight(
-            str(self).strip(),
-            lexer=lexer,
-            formatter=HtmlFormatter(noclasses=True, nobackground=True),
-        )
-        return (
-            '<div style="margin:30px; padding: 20px; border:1px solid #aaa">'
-            f"{highlighted_code}</div>"
-        )
```

### Comparing `featurebyte-0.2.2/featurebyte/common/validator.py` & `featurebyte-0.3.0/featurebyte/common/validator.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,31 +25,44 @@
     Returns
     -------
     Any
     """
     # Note: When `root_validator(pre=True)` is used to decorate this validator, alias key should be used.
     # When `root_validator(pre=False)` is used to decorate, non-alias key should be used.
 
+    def _sanitize_field_name(field_name: str) -> str:
+        if field_name.startswith("internal_"):
+            return field_name[len("internal_") :]
+        return field_name
+
     def _root_validator(cls: Any, values: dict[str, Any]) -> dict[str, Any]:
         _ = cls
         columns_info = values[columns_info_key]
         col_info_map = {}
         for col_info in columns_info:
             col_dict = dict(col_info)
             col_info_map[col_dict["name"]] = col_dict
 
+        col_name_to_field_name_map: dict[str, str] = {}
         for field_name, expected_db_types in expected_column_field_name_type_pairs:
             col_name = values.get(field_name)
             if col_name:
                 if col_name not in col_info_map:
                     raise ValueError(f'Column "{col_name}" not found in the table!')
                 col_dtype = col_info_map[col_name].get("dtype")
                 if expected_db_types and col_dtype not in expected_db_types:
                     dtypes = sorted(str(dtype) for dtype in expected_db_types)
                     raise ValueError(f'Column "{col_name}" is expected to have type(s): {dtypes}')
+                if col_name in col_name_to_field_name_map:
+                    duplicate_field_name = col_name_to_field_name_map[col_name]
+                    raise ValueError(
+                        f"{_sanitize_field_name(field_name)} and {_sanitize_field_name(duplicate_field_name)} "
+                        f'have to be different columns in the table but "{col_name}" is specified for both.'
+                    )
+                col_name_to_field_name_map[col_name] = field_name
         return values
 
     return _root_validator
 
 
 def construct_sort_validator(field: Optional[str] = None) -> Any:
     """
```

### Comparing `featurebyte-0.2.2/featurebyte/config.py` & `featurebyte-0.3.0/featurebyte/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         """
         try:
             headers = kwargs.get("headers", {})
             headers["active-catalog-id"] = headers.get(
                 "active-catalog-id", str(get_active_catalog_id())
             )
             kwargs["headers"] = headers
+            kwargs["allow_redirects"] = False
             return super().request(
                 method,
                 self.base_url + str(url),
                 *args,
                 **kwargs,
             )
         except requests.exceptions.ConnectionError:
```

### Comparing `featurebyte-0.2.2/featurebyte/conftest.py` & `featurebyte-0.3.0/featurebyte/conftest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/core/accessor/count_dict.py` & `featurebyte-0.3.0/featurebyte/core/accessor/count_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             A new Feature object.
 
         Examples
         --------
 
         Create a new feature by calculating the entropy of the dictionary feature:
 
-        >>> counts = fb.Feature.get("CustomerProductGroupCounts_7d")
+        >>> counts = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = counts.cd.entropy()
         >>> new_feature.name = "CustomerProductGroupCountsEntropy_7d"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([counts, new_feature])
@@ -145,15 +145,15 @@
             A new Feature object.
 
         Examples
         --------
 
         Create a new feature by retrieving the most frequent key of the dictionary feature:
 
-        >>> counts = fb.Feature.get("CustomerProductGroupCounts_7d")
+        >>> counts = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = counts.cd.most_frequent()
         >>> new_feature.name = "CustomerProductGroupCountsMostFrequent_7d"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([counts, new_feature])
@@ -189,15 +189,15 @@
             A new Feature object.
 
         Examples
         --------
 
         Create a new feature by counting the number of keys in the dictionary feature:
 
-        >>> counts = fb.Feature.get("CustomerProductGroupCounts_7d")
+        >>> counts = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = counts.cd.unique_count()
         >>> new_feature.name = "CustomerProductGroupCountsUniqueCount_7d"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([counts, new_feature])
@@ -235,16 +235,16 @@
         Feature
             Another Cross Aggregate feature.
 
         Examples
         --------
         Create a similarity feature between two dictionary features:
 
-        >>> feature_1 = fb.Feature.get("CustomerProductGroupCounts_7d")
-        >>> feature_2 = fb.Feature.get("CustomerProductGroupCounts_90d")
+        >>> feature_1 = catalog.get_feature("CustomerProductGroupCounts_7d")
+        >>> feature_2 = catalog.get_feature("CustomerProductGroupCounts_90d")
         >>> similarity = feature_1.cd.cosine_similarity(feature_2)
         >>> similarity.name = "CustomerProductGroupCounts_7d_90d_similarity"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([feature_1, feature_2, similarity])
@@ -289,15 +289,15 @@
         Feature
             A new Feature object
 
         Examples
         --------
         Create a new feature by getting the value for a particular key:
 
-        >>> counts = fb.Feature.get("CustomerProductGroupCounts_7d")
+        >>> counts = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = counts.cd.get_value("Chips et Tortillas")
         >>> new_feature.name = "Chips et Tortillas Value"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([counts, new_feature])
@@ -350,15 +350,15 @@
         Feature
             A new Feature object.
 
         Examples
         --------
         Create a new feature by computing the rank for a particular key:
 
-        >>> counts = fb.Feature.get("CustomerProductGroupCounts_7d")
+        >>> counts = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = counts.cd.get_rank("Chips et Tortillas")
         >>> new_feature.name = "Chips et Tortillas Rank"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([counts, new_feature])
@@ -408,15 +408,15 @@
             A new Feature object.
 
         Examples
         --------
 
         Create a new feature by computing the relative frequency for a particular key:
 
-        >>> counts = fb.Feature.get("CustomerProductGroupCounts_7d")
+        >>> counts = catalog.get_feature("CustomerProductGroupCounts_7d")
         >>> new_feature = counts.cd.get_relative_frequency("Chips et Tortillas")
         >>> new_feature.name = "Chips et Tortillas Relative Frequency"
 
 
         Preview the features:
 
         >>> features = fb.FeatureGroup([counts, new_feature])
```

### Comparing `featurebyte-0.2.2/featurebyte/core/accessor/datetime.py` & `featurebyte-0.3.0/featurebyte/core/accessor/datetime.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,14 +153,19 @@
             The timezone offset to apply. If a string is provided, it must be a valid timezone
             offset in the format "(+|-)HH:mm". If the timezone offset can also be a column in the
             table, in which case a Column object should be provided.
 
         Returns
         -------
         DatetimeAccessor
+
+        Examples
+        --------
+        >>> view = catalog.get_view("GROCERYINVOICE")
+        >>> view["TimestampYearWithOffset"] = view["Timestamp"].dt.tz_offset("+08:00").year
         """
         return DatetimeAccessor(self._obj, timezone_offset)
 
     @property
     def year(self) -> FrozenSeries:
         """
         Returns the year component of each element.
@@ -170,15 +175,15 @@
         FrozenSeries
             Column or Feature containing the year component values
 
         Examples
         --------
         Compute the year component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampYear"] = view["Timestamp"].dt.year
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampYear
         0 2022-01-03 12:28:58           2022
         1 2022-01-03 16:32:15           2022
         2 2022-01-07 16:20:04           2022
         3 2022-01-10 16:18:32           2022
@@ -196,15 +201,15 @@
         FrozenSeries
             Column or Feature containing the quarter component values
 
         Examples
         --------
         Compute the quarter component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampQuarter"] = view["Timestamp"].dt.quarter
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampQuarter
         0 2022-01-03 12:28:58                 1
         1 2022-01-03 16:32:15                 1
         2 2022-01-07 16:20:04                 1
         3 2022-01-10 16:18:32                 1
@@ -222,15 +227,15 @@
         FrozenSeries
             Column or Feature containing the month component values
 
         Examples
         --------
         Compute the month component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampMonth"] = view["Timestamp"].dt.month
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampMonth
         0 2022-01-03 12:28:58               1
         1 2022-01-03 16:32:15               1
         2 2022-01-07 16:20:04               1
         3 2022-01-10 16:18:32               1
@@ -248,15 +253,15 @@
         FrozenSeries
             Column or Feature containing the week component values
 
         Examples
         --------
         Compute the week component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampWeek"] = view["Timestamp"].dt.week
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampWeek
         0 2022-01-03 12:28:58              1
         1 2022-01-03 16:32:15              1
         2 2022-01-07 16:20:04              1
         3 2022-01-10 16:18:32              2
@@ -277,28 +282,28 @@
         FrozenSeries
             Column or Feature containing the day of week component values
 
         Examples
         --------
         Compute the day component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampDay"] = view["Timestamp"].dt.day
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampDay
         0 2022-01-03 12:28:58             3
         1 2022-01-03 16:32:15             3
         2 2022-01-07 16:20:04             7
         3 2022-01-10 16:18:32            10
         4 2022-01-12 17:36:23            12
 
 
         Compute the interval since the previous event in terms of days:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["PreviousTimestamp"] = view["Timestamp"].lag("GroceryCustomerGuid")
         >>> view["DaysSincePreviousTimestamp"] = (view["Timestamp"] - view["PreviousTimestamp"]).dt.day
         >>> view.preview(5).filter(regex="Timestamp|Customer")
                             GroceryCustomerGuid           Timestamp   PreviousTimestamp  DaysSincePreviousTimestamp
         0  007a07da-1525-49be-94d1-fc7251f46a66 2022-01-07 12:02:17                 NaT                         NaN
         1  007a07da-1525-49be-94d1-fc7251f46a66 2022-01-11 19:46:41 2022-01-07 12:02:17                    4.322500
         2  007a07da-1525-49be-94d1-fc7251f46a66 2022-02-04 13:06:35 2022-01-11 19:46:41                   23.722153
@@ -317,15 +322,15 @@
         Returns
         -------
         FrozenSeries
             Column or Feature containing the day of week component values
 
         Examples
         --------
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampDayOfWeek"] = view["Timestamp"].dt.day_of_week
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampDayOfWeek
         0 2022-01-03 12:28:58                   0
         1 2022-01-03 16:32:15                   0
         2 2022-01-07 16:20:04                   4
         3 2022-01-10 16:18:32                   0
@@ -346,15 +351,15 @@
         FrozenSeries
             Column or Feature containing the hour component values
 
         Examples
         --------
         Compute the hour component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampHour"] = view["Timestamp"].dt.hour
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampHour
         0 2022-01-03 12:28:58             12
         1 2022-01-03 16:32:15             16
         2 2022-01-07 16:20:04             16
         3 2022-01-10 16:18:32             16
@@ -375,15 +380,15 @@
         FrozenSeries
             Column or Feature containing the minute component values
 
         Examples
         --------
         Compute the minute component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampMinute"] = view["Timestamp"].dt.minute
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampMinute
         0 2022-01-03 12:28:58               28
         1 2022-01-03 16:32:15               32
         2 2022-01-07 16:20:04               20
         3 2022-01-10 16:18:32               18
@@ -405,15 +410,15 @@
             Column or Feature containing the second component values
 
         Examples
         --------
 
         Compute the second component of a timestamp column:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["TimestampSecond"] = view["Timestamp"].dt.second
         >>> view.preview(5).filter(regex="Timestamp")
                     Timestamp  TimestampSecond
         0 2022-01-03 12:28:58             58.0
         1 2022-01-03 16:32:15             15.0
         2 2022-01-07 16:20:04              4.0
         3 2022-01-10 16:18:32             32.0
```

### Comparing `featurebyte-0.2.2/featurebyte/core/accessor/string.py` & `featurebyte-0.3.0/featurebyte/core/accessor/string.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Compute the length of each string element in the BrowserUserAgent column:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["BrowserUserAgentLength"] = view["BrowserUserAgent"].str.len()
         >>> view.preview(5).filter(regex="BrowserUserAgent")
                                             BrowserUserAgent  BrowserUserAgentLength
         0  Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.3...                     102
         1  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:6...                      78
         2  Mozilla/5.0 (Windows NT 10.0; Win64; x64) Appl...                     115
         3  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...                     117
@@ -100,15 +100,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Convert the BrowserUserAgent column to lower case:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["BrowserUserAgentLower"] = view["BrowserUserAgent"].str.lower()
         >>> view.preview(5).filter(regex="BrowserUserAgent")
                                             BrowserUserAgent                              BrowserUserAgentLower
         0  Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.3...  mozilla/5.0 (windows nt 6.1) applewebkit/537.3...
         1  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:6...  mozilla/5.0 (windows nt 10.0; win64; x64; rv:6...
         2  Mozilla/5.0 (Windows NT 10.0; Win64; x64) Appl...  mozilla/5.0 (windows nt 10.0; win64; x64) appl...
         3  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...  mozilla/5.0 (macintosh; intel mac os x 10_14_4...
@@ -132,15 +132,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Convert the BrowserUserAgent column to upper case:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["BrowserUserAgentUpper"] = view["BrowserUserAgent"].str.upper()
         >>> view.preview(5).filter(regex="BrowserUserAgent")
                                             BrowserUserAgent                              BrowserUserAgentUpper
         0  Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.3...  MOZILLA/5.0 (WINDOWS NT 6.1) APPLEWEBKIT/537.3...
         1  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:6...  MOZILLA/5.0 (WINDOWS NT 10.0; WIN64; X64; RV:6...
         2  Mozilla/5.0 (Windows NT 10.0; Win64; x64) Appl...  MOZILLA/5.0 (WINDOWS NT 10.0; WIN64; X64) APPL...
         3  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...  MOZILLA/5.0 (MACINTOSH; INTEL MAC OS X 10_14_4...
@@ -170,15 +170,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Remove leading and trailing "M" characters from the Title column:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["TitleStrip"] = view["Title"].str.strip("M")
         >>> view.preview(5).filter(regex="Title")
           Title TitleStrip
         0   Ms.         s.
         1   Ms.         s.
         2   Mr.         r.
         3  Mrs.        rs.
@@ -208,15 +208,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Remove leading "M" characters from the Title column:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["TitleStrip"] = view["Title"].str.lstrip("M")
         >>> view.preview(5).filter(regex="Title")
           Title TitleStrip
         0   Ms.         s.
         1   Ms.         s.
         2   Mr.         r.
         3  Mrs.        rs.
@@ -229,32 +229,31 @@
             node_params={"character": to_strip, "side": "left"},
             **self._obj.unary_op_series_params(),
         )
 
     @typechecked
     def rstrip(self, to_strip: Optional[str] = None) -> FrozenSeries:
         """
-        Removes leading characters (whitespaces by default) from each string element.
+        Removes trailing characters (whitespaces by default) from each string element.
 
         Parameters
         ----------
         to_strip: Optional[str]
             Characters to remove, whitespace is used by default.
 
         Returns
         -------
         FrozenSeries
             A new Column or Feature object.
 
         Examples
         --------
+        Remove trailing "M" characters from the Title column:
 
-        Remove leading "M" characters from the Title column:
-
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["TitleStrip"] = view["Title"].str.rstrip(".")
         >>> view.preview(5).filter(regex="Title")
           Title TitleStrip
         0   Ms.         Ms
         1   Ms.         Ms
         2   Mr.         Mr
         3  Mrs.        Mrs
@@ -286,15 +285,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Replace "Windows" with "Win" in the BrowserUserAgent column:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["BrowserUserAgentNew"] = view["BrowserUserAgent"].str.replace("Windows", "Win")
         >>> view.preview(5).filter(regex="BrowserUserAgent")
                                             BrowserUserAgent                                BrowserUserAgentNew
         0  Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.3...  Mozilla/5.0 (Win NT 6.1) AppleWebKit/537.36 (K...
         1  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:6...  Mozilla/5.0 (Win NT 10.0; Win64; x64; rv:66.0)...
         2  Mozilla/5.0 (Windows NT 10.0; Win64; x64) Appl...  Mozilla/5.0 (Win NT 10.0; Win64; x64) AppleWeb...
         3  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...
@@ -328,15 +327,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Pad the Title column to 10 characters:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["PostalCodePadded"] = view["PostalCode"].str.pad(10, fillchar="0")
         >>> view.preview(5).filter(regex="PostalCode")
           PostalCode PostalCodePadded
         0      52000       0000052000
         1      68200       0000068200
         2      12100       0000012100
         3      97232       0000097232
@@ -368,15 +367,15 @@
             A new Column or Feature object.
 
         Examples
         --------
 
         Check whether the BrowserUserAgent column contains "x64":
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["BrowserUserAgent_x64"] = view["BrowserUserAgent"].str.contains("x64")
         >>> view.preview(5).filter(regex="BrowserUserAgent")
                                             BrowserUserAgent  BrowserUserAgent_x64
         0  Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.3...                 False
         1  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:6...                  True
         2  Mozilla/5.0 (Windows NT 10.0; Win64; x64) Appl...                  True
         3  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...                 False
@@ -417,15 +416,15 @@
             When the step size is neither None nor 1.
 
         Examples
         --------
 
         Slice the first 10 characters from the BrowserUserAgent column:
 
-        >>> view = catalog.get_table("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["BrowserUserAgentSlice"] = view["BrowserUserAgent"].str.slice(0, 10)
         >>> view.preview(5).filter(regex="BrowserUserAgent")
                                             BrowserUserAgent BrowserUserAgentSlice
         0  Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.3...            Mozilla/5.
         1  Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:6...            Mozilla/5.
         2  Mozilla/5.0 (Windows NT 10.0; Win64; x64) Appl...            Mozilla/5.
         3  Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_4...            Mozilla/5.
```

### Comparing `featurebyte-0.2.2/featurebyte/core/frame.py` & `featurebyte-0.3.0/featurebyte/core/frame.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/core/generic.py` & `featurebyte-0.3.0/featurebyte/core/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/core/mixin.py` & `featurebyte-0.3.0/featurebyte/core/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/core/series.py` & `featurebyte-0.3.0/featurebyte/core/series.py`

 * *Files 4% similar despite different names*

```diff
@@ -558,15 +558,15 @@
 
         Returns
         -------
         bool
 
         Examples
         --------
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
 
         >>> print(view["Timestamp"].is_datetime)
         True
         >>> print(view["Amount"].is_datetime)
         False
         """
         return self.dtype in (DBVarType.TIMESTAMP, DBVarType.TIMESTAMP_TZ, DBVarType.DATE)
@@ -578,15 +578,15 @@
 
         Returns
         -------
         bool
 
         Examples
         --------
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
 
         >>> print(view["Amount"].is_numeric)
         True
         >>> print(view["Timestamp"].is_numeric)
         False
         """
         return self.dtype in (DBVarType.INT, DBVarType.FLOAT)
@@ -600,15 +600,15 @@
         FrozenSeriesT
             Column or Feature with boolean values
 
         Examples
         --------
         Filter a View based on whether a column has null values:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view_filtered = view[view["Amount"].isnull()]
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.IS_NULL,
             output_var_type=DBVarType.BOOL,
             node_params={},
@@ -624,15 +624,15 @@
         FrozenSeriesT
             Column or Feature with boolean values
 
         Examples
         --------
         Filter a View by removing rows where a column has null values:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view_filtered = view[view["Amount"].notnull()]
         """
         return ~self.isnull()
 
     @typechecked
     def astype(
         self: FrozenSeriesT,
@@ -658,15 +658,15 @@
         TypeError
             If the Series dtype does not support type conversion.
 
         Examples
         --------
         Convert a numerical series to a string series, and back to an int series.
 
-        >>> event_view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> event_view = catalog.get_view("GROCERYINVOICE")
         >>> event_view["Amount"] = event_view["Amount"].astype(str)
         >>> event_view["Amount"] = event_view["Amount"].astype(int)
         """
         supported_source_dtype = {DBVarType.BOOL, DBVarType.INT, DBVarType.FLOAT, DBVarType.VARCHAR}
         if self.dtype not in supported_source_dtype:
             raise TypeError(f"astype not supported for {self.dtype}")
 
@@ -705,27 +705,27 @@
         FrozenSeriesT
             Column or Feature with absolute values
 
         Examples
         --------
         Compute absolute values for a Column in a View:
 
-        >>> view = fb.Table.get("GROCERYCUSTOMER").get_view()
+        >>> view = catalog.get_view("GROCERYCUSTOMER")
         >>> view["LongitudeAbs"] = view["Longitude"].abs()
         >>> view.preview(5).filter(regex="Longitude")
            Longitude  LongitudeAbs
         0   5.209627      5.209627
         1   7.423195      7.423195
         2   2.990572      2.990572
         3 -61.069866     61.069866
         4   3.120654      3.120654
 
         Compute absolute values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_abs = feature.abs()
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.ABS,
             output_var_type=self.dtype,
             node_params={},
@@ -742,28 +742,28 @@
         FrozenSeriesT
             Column or Feature with square root values
 
         Examples
         --------
         Compute square root values for a Column in a View:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["AmountSqrt"] = view["Amount"].sqrt()
         >>> view.preview(5).filter(regex="Amount")
            Amount  AmountSqrt
         0   10.68    3.268027
         1   38.04    6.167658
         2    1.99    1.410674
         3   37.21    6.100000
         4    1.20    1.095445
 
 
         Compute square root values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_sqrt = feature.sqrt()
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.SQRT,
             output_var_type=DBVarType.FLOAT,
             node_params={},
@@ -785,28 +785,28 @@
         FrozenSeriesT
             Column or Feature with exponential power values
 
         Examples
         --------
         Compute exponential power values for a Column in a View:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["Amount^2"] = view["Amount"].pow(2)
         >>> view.preview(5).filter(regex="Amount")
            Amount   Amount^2
         0   10.68   114.0624
         1   38.04  1447.0416
         2    1.99     3.9601
         3   37.21  1384.5841
         4    1.20     1.4400
 
 
         Compute exponential power values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_pow = feature.pow(2)
         """
         return self._binary_op(
             other=other,
             node_type=NodeType.POWER,
             output_var_type=DBVarType.FLOAT,
         )
@@ -821,28 +821,28 @@
         FrozenSeriesT
             Column or Feature with natural logarithm values
 
         Examples
         --------
         Compute natural logarithm values for a Column in a View:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["AmountLog"] = view["Amount"].log()
         >>> view.preview(5).filter(regex="Amount")
           Amount  AmountLog
         0   10.68   2.368373
         1   38.04   3.638638
         2    1.99   0.688135
         3   37.21   3.616578
         4    1.20   0.182322
 
 
         Compute natural logarithm values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_log = (feature + 1.0).log()
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.LOG,
             output_var_type=DBVarType.FLOAT,
             node_params={},
@@ -859,28 +859,28 @@
         FrozenSeriesT
             Column or Feature with exponential values
 
         Examples
         --------
         Compute exponential values for a Column in a View:
 
-        >>> view = fb.Table.get("INVOICEITEMS").get_view()
+        >>> view = catalog.get_view("INVOICEITEMS")
         >>> view["QuantityExp"] = view["Quantity"].exp()
         >>> view.preview(5).filter(regex="Quantity")
            Quantity  QuantityExp
         0       2.0     7.389056
         1       1.0     2.718282
         2       1.0     2.718282
         3       1.0     2.718282
         4       2.0     7.389056
 
 
         Compute exponential values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_exp = feature.exp()
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.EXP,
             output_var_type=DBVarType.FLOAT,
             node_params={},
@@ -897,29 +897,29 @@
         FrozenSeriesT
             Column or Feature with rounded values
 
         Examples
         --------
         Round values for a Column in a View:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> column = view["Amount"].floor()
         >>> view["AmountFloor"] = view["Amount"].floor()
         >>> view.preview(5).filter(regex="Amount")
            Amount  AmountFloor
         0   10.68          10
         1   38.04          38
         2    1.99           1
         3   37.21          37
         4    1.20           1
 
 
         Round values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_floor = feature.floor()
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.FLOOR,
             output_var_type=DBVarType.INT,
             node_params={},
@@ -936,28 +936,28 @@
         FrozenSeriesT
             Series or Feature with rounded values
 
         Examples
         --------
         Compute rounded values for a Column in a View:
 
-        >>> view = fb.Table.get("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["AmountCeil"] = view["Amount"].ceil()
         >>> view.preview(5).filter(regex="Amount")
            Amount  AmountCeil
         0   10.68          11
         1   38.04          39
         2    1.99           2
         3   37.21          38
         4    1.20           2
 
 
         Compute rounded values for a Feature:
 
-        >>> feature = fb.Feature.get("InvoiceCount_60days")
+        >>> feature = catalog.get_feature("InvoiceCount_60days")
         >>> feature_ceil = feature.ceil()
         """
         return series_unary_operation(
             input_series=self,
             node_type=NodeType.CEIL,
             output_var_type=DBVarType.INT,
             node_params={},
@@ -1111,15 +1111,15 @@
             Value to replace missing values
 
         Examples
         --------
 
         Fill missing values in a column with 0:
 
-        >>> view = catalog.get_table("GROCERYINVOICE").get_view()
+        >>> view = catalog.get_view("GROCERYINVOICE")
         >>> view["Amount"].fillna(0)
 
 
         Fill missing values in a feature with 0:
 
         >>> feature = catalog.get_feature("InvoiceAmountAvg_60days")
         >>> feature.fillna(0)
```

### Comparing `featurebyte-0.2.2/featurebyte/core/timedelta.py` & `featurebyte-0.3.0/featurebyte/core/timedelta.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,21 @@
     -------
     Series
 
     Raises
     ------
     ValueError
         if input Series is not of INT type
+
+    Examples
+    --------
+    >>> items_view = catalog.get_view("INVOICEITEMS")
+    >>> items_view["DAYS_SINCE_LAST_INVOICE"] = to_timedelta(  # doctest: +SKIP
+    ...   items_view["DAYS_SINCE_LAST_INVOICE"], "days"
+    ... )
     """
     if series.dtype != DBVarType.INT:
         raise ValueError(f"to_timedelta only supports INT type series; got {series.dtype}")
 
     timedelta_series = series_unary_operation(
         input_series=series,
         node_type=NodeType.TIMEDELTA,
```

### Comparing `featurebyte-0.2.2/featurebyte/core/util.py` & `featurebyte-0.3.0/featurebyte/core/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/datasets/__main__.py` & `featurebyte-0.3.0/featurebyte/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/datasets/app.py` & `featurebyte-0.3.0/featurebyte/datasets/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/datasets/creditcard.sql` & `featurebyte-0.3.0/featurebyte/datasets/creditcard.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/datasets/doctest_grocery.sql` & `featurebyte-0.3.0/featurebyte/datasets/doctest_grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/datasets/grocery.sql` & `featurebyte-0.3.0/featurebyte/datasets/grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/datasets/healthcare.sql` & `featurebyte-0.3.0/featurebyte/datasets/healthcare.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/docker/featurebyte.yml` & `featurebyte-0.3.0/featurebyte/docker/featurebyte.yml`

 * *Files 2% similar despite different names*

```diff
@@ -32,29 +32,29 @@
       driver: local
   featurebyte-server:
     networks:
       - featurebyte
     hostname: featurebyte-server
     restart: unless-stopped
     container_name: featurebyte-server
-    image: featurebyte/featurebyte-server:0.2.2
+    image: featurebyte/featurebyte-server:0.3.0
     depends_on:
       mongo-rs:
         condition: service_healthy
     ports:
       - "0.0.0.0:8088:8088"
     command: ["bash", "/docker-entrypoint.sh", "server"]
     environment:
       - "FEATUREBYTE_HOME=/app/.featurebyte"
       - "MPLCONFIGDIR=/app/matplotlib"
       - "REDIS_URI=redis://redis:6379"
       - "MONGODB_URI=mongodb://mongo-rs:27021,mongo-rs:27022/?replicaSet=rs0"
       - "API_HOST=0.0.0.0"
       - "API_PORT=8088"
-      - "LOG_LEVEL=info"
+      - "LOG_LEVEL=${LOG_LEVEL}"
       - "LOCAL_UID=${LOCAL_UID}"
       - "LOCAL_GID=${LOCAL_GID}"
     healthcheck:
       test: ["CMD", "curl", "-f", "http://127.0.0.1:8088/status"]
       interval: 5s
       start_period: 30s
     volumes:
@@ -65,25 +65,26 @@
       driver: local
   featurebyte-worker:
     networks:
       - featurebyte
     hostname: featurebyte-worker
     restart: unless-stopped
     container_name: featurebyte-worker
-    image: featurebyte/featurebyte-server:0.2.2
+    image: featurebyte/featurebyte-server:0.3.0
     depends_on:
       mongo-rs:
         condition: service_healthy
       redis:
         condition: service_healthy
     environment:
       - "FEATUREBYTE_HOME=/app/.featurebyte"
       - "MPLCONFIGDIR=/app/matplotlib"
       - "REDIS_URI=redis://redis:6379"
       - "MONGODB_URI=mongodb://mongo-rs:27021,mongo-rs:27022/?replicaSet=rs0"
+      - "LOG_LEVEL=${LOG_LEVEL}"
       - "LOCAL_UID=${LOCAL_UID}"
       - "LOCAL_GID=${LOCAL_GID}"
     command: ["bash", "/docker-entrypoint.sh", "worker"]
     volumes:
       - files-data:/app/.featurebyte/data/files
       - staging-data:/data/staging
       - file-store:/tmp
```

### Comparing `featurebyte-0.2.2/featurebyte/docker/manager.py` & `featurebyte-0.3.0/featurebyte/docker/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 import os
 import sys
 import tempfile
 import time
 from contextlib import contextmanager
 from enum import Enum
 
+from python_on_whales import DockerException
 from python_on_whales.docker_client import DockerClient
 from rich.align import Align
 from rich.console import Console
 from rich.panel import Panel
 from rich.status import Status
 from rich.table import Table
 from rich.text import Text
 
 from featurebyte.api.feature_store import FeatureStore, SourceType
 from featurebyte.common.path_util import get_package_root
 from featurebyte.config import Configurations
 from featurebyte.datasets.app import import_dataset
+from featurebyte.exception import DockerError
 from featurebyte.logging import get_logger
 from featurebyte.query_graph.node.schema import SparkDetails
 
 logger = get_logger(__name__)
 
 
 class ApplicationName(str, Enum):
@@ -46,30 +48,34 @@
     Yields
     -------
     Generator[DockerClient, None, None]
         Docker client
     """
     with tempfile.TemporaryDirectory() as temp_dir:
         compose_env_file = os.path.join(temp_dir, ".env")
+        env_file_lines = []
         if sys.platform != "win32":
             import pwd  # pylint: disable=import-outside-toplevel
             uid = os.getuid()
             user = pwd.getpwuid(uid)
-            with open(compose_env_file, "w", encoding="utf8") as file_obj:
-                file_obj.write(f'LOCAL_UID="{uid}"\nLOCAL_GID="{user.pw_gid}"\n')
-            docker = DockerClient(
-                compose_project_name="featurebyte",
-                compose_files=[os.path.join(get_package_root(), "docker/featurebyte.yml")],
-                compose_env_file=compose_env_file,
-            )
-        else:
-            docker = DockerClient(
-                compose_project_name="featurebyte",
-                compose_files=[os.path.join(get_package_root(), "docker/featurebyte.yml")],
+            env_file_lines.extend(
+                [
+                    f'LOCAL_UID="{uid}"\n',
+                    f'LOCAL_GID="{user.pw_gid}"\n',
+                ]
             )
+        log_level = os.environ.get("LOG_LEVEL", "INFO")
+        env_file_lines.append(f'LOG_LEVEL="{log_level}"\n')
+        with open(compose_env_file, "w", encoding="utf8") as file_obj:
+            file_obj.writelines(env_file_lines)
+        docker = DockerClient(
+            compose_project_name="featurebyte",
+            compose_files=[os.path.join(get_package_root(), "docker/featurebyte.yml")],
+            compose_env_file=compose_env_file,
+        )
         yield docker
 
 
 def get_service_names(app_name: ApplicationName) -> List[str]:
     """
     Get list of service names for application
 
@@ -140,58 +146,67 @@
     ----------
     app_name : ApplicationName
         Application name
     services : List[str]
         List of services to start
     verbose : bool
         Print verbose output
-    """
-    services = services or get_service_names(app_name)
-
-    # Load config to ensure it exists before starting containers
-    config = Configurations()  # pylint: disable=unused-variable
-    __setup_network()
-
-    with get_docker_client() as docker:
-        docker.compose.up(services=services, detach=True)
 
-        # Wait for all services to be healthy
-        def _wait_for_healthy(spinner_status: Optional[Status] = None) -> None:
-            while True:
-                unhealthy_containers = []
-                for container in docker.compose.ps():
-                    health = container.state.health.status if container.state.health else "N/A"
-                    if health not in {"healthy", "N/A"}:
-                        unhealthy_containers.append(container.name)
-                if len(unhealthy_containers) == 0:
-                    break
-                statuses = (
-                    Text("Services: [")
-                    + Text(", ").join(map(lambda s: Text(s, style="red"), unhealthy_containers))
-                    + Text("] are unhealthy", style="None")
-                )
-                if spinner_status:
-                    spinner_status.update(statuses)
-                time.sleep(1)
-
-        if verbose:
-            with console.status("Waiting for services to be healthy...") as spinner_status:
-                _wait_for_healthy(spinner_status)
-                message = (
-                    """
-                    [bold green]Featurebyte application started successfully![/]
-
-                    API server now running at: [cyan underline]http://127.0.0.1:8088[/].
-                    You can now use the featurebyte SDK with the API server.
-                    """
-                )
-            console.print(Panel(Align.left(message), title="FeatureByte Services", width=120))
-        else:
-            _wait_for_healthy()
+    Raises
+    ------
+    DockerError
+        Docker compose fails to start
+    """
+    try:
+        services = services or get_service_names(app_name)
 
+        # Load config to ensure it exists before starting containers
+        Configurations()
+        __setup_network()
+
+        with get_docker_client() as docker:
+            docker.compose.up(services=services, detach=True)
+
+            # Wait for all services to be healthy
+            def _wait_for_healthy(spinner_status: Optional[Status] = None) -> None:
+                while True:
+                    unhealthy_containers = []
+                    for container in docker.compose.ps():
+                        health = container.state.health.status if container.state.health else "N/A"
+                        if health not in {"healthy", "N/A"}:
+                            unhealthy_containers.append(container.name)
+                    if len(unhealthy_containers) == 0:
+                        break
+                    statuses = (
+                        Text("Services: [")
+                        + Text(", ").join(map(lambda s: Text(s, style="red"), unhealthy_containers))
+                        + Text("] are unhealthy", style="None")
+                    )
+                    if spinner_status:
+                        spinner_status.update(statuses)
+                    time.sleep(1)
+
+            if verbose:
+                with console.status("Waiting for services to be healthy...") as spinner_status:
+                    _wait_for_healthy(spinner_status)
+                    message = (
+                        """
+                        [bold green]Featurebyte application started successfully![/]
+
+                        API server now running at: [cyan underline]http://127.0.0.1:8088[/].
+                        You can now use the featurebyte SDK with the API server.
+                        """
+                    )
+                console.print(Panel(Align.left(message), title="FeatureByte Services", width=120))
+            else:
+                _wait_for_healthy()
+    except DockerException as exc:
+        if "Is the docker daemon running" in str(exc):
+            raise DockerError("Docker is not running, please start docker and try again.") from exc
+        raise DockerError(f"Failed to start application: {exc.stderr}") from exc
 
 def start_playground(datasets: Optional[List[str]] = None,
                      force_import: bool = False, verbose: bool = True) -> None:
     """
     Start featurebyte playground environment
 
     Parameters
```

### Comparing `featurebyte-0.2.2/featurebyte/enum.py` & `featurebyte-0.3.0/featurebyte/enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,14 +174,26 @@
 
 
 class AggFunc(StrEnum):
     """
     The AggFunc enum class provides a way to represent various aggregation methods in your code. It helps reduce
     errors by defining a set of supported aggregation methods. Each enum constant corresponds to a specific
     aggregation method.
+
+    Examples
+    --------
+    >>> items_view = catalog.get_view("INVOICEITEMS")
+    >>> # Group items by the column GroceryInvoiceGuid that references the customer entity
+    >>> items_by_invoice = items_view.groupby("GroceryInvoiceGuid")
+    >>> # Get the number of items in each invoice
+    >>> invoice_item_count = items_by_invoice.aggregate(  # doctest: +SKIP
+    ...   None,
+    ...   method=fb.AggFunc.COUNT,
+    ...   feature_name="InvoiceItemCount",
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.AggFunc")
 
     SUM = "sum", "Compute sum of values."
     AVG = "avg", "Compute average value."
     MIN = "min", "Compute minimum value."
@@ -234,14 +246,15 @@
     The StorageType enum class provides a way to represent different types of distributed storage in your code.
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.StorageType")
 
     FILE = "file", "Local file storage."
     S3 = "s3", "S3 Storage."
+    GCS = "gcs", "Google Cloud Storage."
 
 
 class SpecialColumnName(StrEnum):
     """
     Special column names such as POINT_IN_TIME
     """
 
@@ -260,14 +273,15 @@
 
     TILE_CACHE_WORKING_TABLE = "__FB_TILE_CACHE_WORKING_TABLE"
     TILE_ENTITY_TRACKER_SUFFIX = "_ENTITY_TRACKER"
     LAST_TILE_START_DATE_PREVIOUS = "__FB_LAST_TILE_START_DATE_PREVIOUS"
     ENTITY_TABLE_SQL_PLACEHOLDER = "__FB_ENTITY_TABLE_SQL_PLACEHOLDER"
     ENTITY_TABLE_NAME = "__FB_ENTITY_TABLE_NAME"
     ENTITY_TABLE_END_DATE = "__FB_ENTITY_TABLE_END_DATE"
+    ENTITY_TABLE_START_DATE = "__FB_ENTITY_TABLE_START_DATE"
 
     LAST_TILE_INDEX = "__FB_LAST_TILE_INDEX"
     FIRST_TILE_INDEX = "__FB_FIRST_TILE_INDEX"
 
     POINT_IN_TIME_SQL_PLACEHOLDER = "__FB_POINT_IN_TIME_SQL_PLACEHOLDER"
 
     MIGRATION_VERSION = "MIGRATION_VERSION"
@@ -283,14 +297,15 @@
     FEATURE_JOB_SETTING_ANALYSIS_BACKTEST = "FEATURE_JOB_SETTING_ANALYSIS_BACKTEST"
     HISTORICAL_FEATURE_TABLE_CREATE = "HISTORICAL_TABLE_CREATE"
     OBSERVATION_TABLE_CREATE = "OBSERVATION_TABLE_CREATE"
     DEPLOYMENT_CREATE_UPDATE = "DEPLOYMENT_CREATE_UPDATE"
     BATCH_REQUEST_TABLE_CREATE = "BATCH_REQUEST_TABLE_CREATE"
     BATCH_FEATURE_TABLE_CREATE = "BATCH_FEATURE_TABLE_CREATE"
     MATERIALIZED_TABLE_DELETE = "MATERIALIZED_TABLE_DELETE"
+    BATCH_FEATURE_CREATE = "BATCH_FEATURE_CREATE"
     TEST = "TEST"
     TILE_COMPUTE = "TILE_COMPUTE"
 
 
 class TableDataType(StrEnum):
     """
     TableDataType enum
```

### Comparing `featurebyte-0.2.2/featurebyte/exception.py` & `featurebyte-0.3.0/featurebyte/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,14 +212,20 @@
 
 class DocumentConflictError(DocumentError):
     """
     Raise when there exists a conflicting document at the persistent
     """
 
 
+class DocumentCreationError(DocumentError):
+    """
+    Raise when the document invalid creation happens
+    """
+
+
 class DocumentUpdateError(DocumentError):
     """
     Raise when the document invalid update happens
     """
 
 
 class DocumentDeletionError(DocumentError):
@@ -340,7 +346,31 @@
     """
 
 
 class ColumnNotFoundError(FeatureByteException):
     """
     Raised when a specified column is not found in the view or table
     """
+
+
+class DockerError(FeatureByteException):
+    """
+    Raised when there is an error with Docker
+    """
+
+
+class DatabaseNotFoundError(FeatureByteException):
+    """
+    Raise when the requested database does not exist in the data warehouse
+    """
+
+
+class SchemaNotFoundError(FeatureByteException):
+    """
+    Raise when the requested schema does not exist in the data warehouse
+    """
+
+
+class TableNotFoundError(FeatureByteException):
+    """
+    Raise when the requested table does not exist in the data warehouse
+    """
```

### Comparing `featurebyte-0.2.2/featurebyte/feature_manager/manager.py` & `featurebyte-0.3.0/featurebyte/feature_manager/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/feature_manager/model.py` & `featurebyte-0.3.0/featurebyte/feature_manager/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/feature_manager/sql_template.py` & `featurebyte-0.3.0/featurebyte/feature_manager/sql_template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/logging.py` & `featurebyte-0.3.0/featurebyte/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Logging formatting
 """
 from typing import Any, Optional
 
 import logging
+import os
 import sys
 
 from featurebyte.common.env_util import is_notebook
 from featurebyte.config import Configurations
 
 
 class CustomLogger(logging.Logger):
@@ -96,14 +97,31 @@
 )
 CONSOLE_LOG_FORMATTER = logging.Formatter(
     "%(asctime)s | %(levelname)-8s | %(name)s | %(funcName)s:%(lineno)d | %(message)s",
     "%Y-%m-%d %H:%M:%S",
 )
 
 
+def set_logger_level(logger: logging.Logger, configurations: Configurations) -> None:
+    """
+    Set logger level
+
+    Parameters
+    ----------
+    logger: logging.Logger
+        Logger to set level
+    configurations: Configurations
+        Optional configurations used to configure logger
+    """
+    if os.environ.get("LOG_LEVEL"):
+        logger.setLevel(os.environ["LOG_LEVEL"])
+    else:
+        logger.setLevel(configurations.logging.level)
+
+
 def get_logger(logger_name: str, configurations: Optional[Configurations] = None) -> logging.Logger:
     """
     Get logger
 
     Parameters
     ----------
     logger_name: str
@@ -121,28 +139,28 @@
     if is_notebook_env:
         formatter = NOTEBOOK_LOG_FORMATTER
 
     console_handler = logging.StreamHandler(stream=sys.stderr)
     console_handler.setFormatter(formatter)
     logger = logging.getLogger(logger_name)
     logger.propagate = False
-    logger.setLevel(configurations.logging.level)
     if logger.hasHandlers():
         logger.handlers.clear()
     logger.addHandler(console_handler)
+    set_logger_level(logger, configurations)
     return logger
 
 
 def reconfigure_loggers(configurations: Configurations) -> None:
     """
     Reconfigure all loggers with configurations.
 
     Parameters
     ----------
     configurations: Configurations
         Configurations to use
     """
     for name in logging.root.manager.loggerDict:  # pylint: disable=no-member
-        logging.getLogger(name).setLevel(configurations.logging.level)
+        set_logger_level(logging.getLogger(name), configurations)
 
 
 __all__ = ["get_logger"]
```

### Comparing `featurebyte-0.2.2/featurebyte/middleware.py` & `featurebyte-0.3.0/featurebyte/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 Handles API requests middleware
 """
 from typing import Any, Awaitable, Callable, Dict, Optional, Type, Union
 
 import inspect
 from http import HTTPStatus
 
-import requests
 from fastapi import FastAPI, Request, Response
 from pydantic import ValidationError
-from starlette.background import BackgroundTasks
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.responses import JSONResponse
 
 from featurebyte.exception import (
     CredentialsError,
+    DatabaseNotFoundError,
     DocumentConflictError,
     DocumentError,
     DocumentNotFoundError,
     FeatureStoreSchemaCollisionError,
     LimitExceededError,
     NoFeatureStorePresentError,
     QueryNotSupportedError,
     RequiredEntityNotProvidedError,
+    SchemaNotFoundError,
+    TableNotFoundError,
     UnexpectedServingNamesMappingError,
 )
 from featurebyte.logging import get_logger
 
 logger = get_logger(__name__)
 
 
@@ -194,14 +195,32 @@
 
 ExecutionContext.register(
     NoFeatureStorePresentError,
     handle_status_code=HTTPStatus.FAILED_DEPENDENCY,
     handle_message="No feature store found. Please create one before trying to access this functionality.",
 )
 
+ExecutionContext.register(
+    DatabaseNotFoundError,
+    handle_status_code=HTTPStatus.FAILED_DEPENDENCY,
+    handle_message="Database not found. Please specify a valid database name.",
+)
+
+ExecutionContext.register(
+    SchemaNotFoundError,
+    handle_status_code=HTTPStatus.FAILED_DEPENDENCY,
+    handle_message="Schema not found. Please specify a valid schema name.",
+)
+
+ExecutionContext.register(
+    TableNotFoundError,
+    handle_status_code=HTTPStatus.FAILED_DEPENDENCY,
+    handle_message="Table not found. Please specify a valid table name.",
+)
+
 
 class ExceptionMiddleware(BaseHTTPMiddleware):
     """
     Middleware used by FastAPI to process each request
     """
 
     def __init__(self, app: FastAPI):
@@ -229,74 +248,7 @@
                 response: Response = await executor.execute()
         except Exception as exc:  # pylint: disable=broad-except
             logger.exception(str(exc))
             return JSONResponse(
                 content={"detail": str(exc)}, status_code=HTTPStatus.INTERNAL_SERVER_ERROR
             )
         return response
-
-
-class TelemetryMiddleware(BaseHTTPMiddleware):
-    """
-    Middleware used by FastAPI to send telemetry logs
-    """
-
-    def __init__(self, app: FastAPI, endpoint: str, user_id: str, user_ip: str):
-        super().__init__(app)
-        self.endpoint = endpoint
-        self.user_id = user_id
-        self.user_ip = user_ip
-
-    async def _send_telemetry(self, payload: Dict[str, Any]) -> None:
-        try:
-            requests.post(self.endpoint, json=payload, timeout=1)  # set timeout to 1 second
-        except Exception:  # pylint: disable=broad-except
-            pass
-
-    async def dispatch(
-        self, request: Request, call_next: Callable[[Request], Awaitable[Response]]
-    ) -> Response:
-        """
-        Telemetry middleware "main" call
-
-        Parameters
-        ----------
-        request: Request
-            Request object to be handled
-        call_next: Callable[[Request], Awaitable[Response]]
-            Function that will handle the request
-
-        Returns
-        -------
-        Response
-        """
-        # Render the response
-        response = await call_next(request)
-
-        # Ignore telemetry for status endpoint
-        if request.url.path in ["/status"]:
-            return response
-
-        if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-            trace = response.body.decode("utf-8")
-        else:
-            trace = str(response.status_code)
-
-        # Render payload to server
-        payload = {
-            "method": request.method,
-            "path": request.url.path,
-            "user": self.user_id,
-            "ip": self.user_ip,
-            "trace": trace,
-        }
-        if response.background is None:
-            background = BackgroundTasks()
-            background.add_task(self._send_telemetry, payload)
-            response.background = background
-        else:
-            background = BackgroundTasks()
-            background.add_task(response.background)
-            background.add_task(self._send_telemetry, payload)
-            response.background = background
-
-        return response
```

### Comparing `featurebyte-0.2.2/featurebyte/migration/migration_data_service.py` & `featurebyte-0.3.0/featurebyte/migration/migration_data_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/migration/model.py` & `featurebyte-0.3.0/featurebyte/migration/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/migration/run.py` & `featurebyte-0.3.0/featurebyte/migration/run.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/migration/service/__init__.py` & `featurebyte-0.3.0/featurebyte/migration/service/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/migration/service/data_warehouse.py` & `featurebyte-0.3.0/featurebyte/migration/service/data_warehouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,27 +48,27 @@
         tile_column_name_to_type = {}
         # activate use of raw query filter to retrieve all documents regardless of catalog membership
         with feature_service.allow_use_raw_query_filter():
             feature_documents = feature_service.list_documents_iterator(
                 query_filter={}, use_raw_query_filter=True
             )
 
-        async for doc in feature_documents:
-            feature_model = ExtendedFeatureModel(**doc)
-            try:
-                tile_specs = feature_model.tile_specs
-            except:  # pylint: disable=bare-except
-                logger.exception(f"Failed to extract tile_specs for {doc}")
-                # For tile columns with no known type, they will be given a FLOAT type below
-                continue
-            for tile_spec in tile_specs:
-                for tile_column_name, tile_column_type in zip(
-                    tile_spec.value_column_names, tile_spec.value_column_types
-                ):
-                    tile_column_name_to_type[tile_column_name] = tile_column_type
+            async for doc in feature_documents:
+                feature_model = ExtendedFeatureModel(**doc)
+                try:
+                    tile_specs = feature_model.tile_specs
+                except:  # pylint: disable=bare-except
+                    logger.exception(f"Failed to extract tile_specs for {doc}")
+                    # For tile columns with no known type, they will be given a FLOAT type below
+                    continue
+                for tile_spec in tile_specs:
+                    for tile_column_name, tile_column_type in zip(
+                        tile_spec.value_column_names, tile_spec.value_column_types
+                    ):
+                        tile_column_name_to_type[tile_column_name] = tile_column_type
         return tile_column_name_to_type
 
     def get_tile_column_type(self, tile_column_name: str) -> str | None:
         """
         Get tile column type for the given tile column name. Return None if the column type is not
         known (when none of the existing Feature corresponds to the tile column; could be due to
         unsaved features or TILE_REGISTRY table being in a bad state)
```

### Comparing `featurebyte-0.2.2/featurebyte/migration/service/mixin.py` & `featurebyte-0.3.0/featurebyte/migration/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/__init__.py` & `featurebyte-0.3.0/featurebyte/models/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/base.py` & `featurebyte-0.3.0/featurebyte/models/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/batch_feature_table.py` & `featurebyte-0.3.0/featurebyte/models/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/batch_request_table.py` & `featurebyte-0.3.0/featurebyte/models/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/catalog.py` & `featurebyte-0.3.0/featurebyte/models/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/context.py` & `featurebyte-0.3.0/featurebyte/models/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/credential.py` & `featurebyte-0.3.0/featurebyte/models/credential.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Document model for stored credentials
 """
-from typing import List, Literal, Optional, Union
+from typing import Dict, List, Literal, Optional, Union
 from typing_extensions import Annotated
 
 import os  # pylint: disable=wrong-import-order
 
 import pymongo
 from cryptography.fernet import Fernet
 from pydantic import Field, StrictStr
@@ -69,22 +69,42 @@
     def encrypt(self) -> None:
         """
         Encrypt credentials
         """
         for field in self.__fields__.values():
             if field.type_ == StrictStr:
                 setattr(self, field.name, encrypt_value(getattr(self, field.name)))
+            elif field.type_ == str:
+                # pydantic captures dict field type as str
+                field_value = getattr(self, field.name)
+                if isinstance(field_value, dict):
+                    # Encrypt each value in the dict
+                    setattr(
+                        self,
+                        field.name,
+                        {key: encrypt_value(value) for key, value in field_value.items()},
+                    )
 
     def decrypt(self) -> None:
         """
         Decrypt credentials
         """
         for field in self.__fields__.values():
             if field.type_ == StrictStr:
                 setattr(self, field.name, decrypt_value(getattr(self, field.name)))
+            elif field.type_ == str:
+                # pydantic captures dict field type as str
+                field_value = getattr(self, field.name)
+                if isinstance(field_value, dict):
+                    # Decrypt each value in the dict
+                    setattr(
+                        self,
+                        field.name,
+                        {key: decrypt_value(value) for key, value in field_value.items()},
+                    )
 
 
 # Database Credentials
 class DatabaseCredentialType(StrEnum):
     """
     Credential Type
     """
@@ -100,28 +120,39 @@
 
     type: DatabaseCredentialType
 
 
 class UsernamePasswordCredential(BaseDatabaseCredential):
     """
     Data class for a username and password credential.
+
+    Examples
+    --------
+    >>> username_password_credential = UsernamePasswordCredential(
+    ...   username="username",
+    ...   password="password",
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.UsernamePasswordCredential")
 
     type: Literal[DatabaseCredentialType.USERNAME_PASSWORD] = Field(
         DatabaseCredentialType.USERNAME_PASSWORD, const=True
     )
     username: StrictStr = Field(description="Username of your account.")
     password: StrictStr = Field(description="Password of your account.")
 
 
 class AccessTokenCredential(BaseDatabaseCredential):
     """
     Data class for an access token credential.
+
+    Examples
+    --------
+    >>> access_token_credential = AccessTokenCredential(access_token="access_token")
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.AccessTokenCredential")
 
     type: Literal[DatabaseCredentialType.ACCESS_TOKEN] = Field(
         DatabaseCredentialType.ACCESS_TOKEN, const=True
     )
@@ -137,43 +168,90 @@
 # Storage Credentials
 class StorageCredentialType(StrEnum):
     """
     Storage Credential Type
     """
 
     S3 = "S3"
+    GCS = "GCS"
+    AZURE = "AZURE"
 
 
 class BaseStorageCredential(BaseCredential):
     """
     Base storage credential
     """
 
     type: StorageCredentialType
 
 
 class S3StorageCredential(BaseStorageCredential):
     """
     Data class for a S3 storage credential.
+
+    Examples
+    --------
+    >>> s3_storage_credential = S3StorageCredential(
+    ...   s3_access_key_id="access_key_id",
+    ...   s3_secret_access_key="s3_secret_access_key"
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.S3StorageCredential")
 
     type: StorageCredentialType = Field(StorageCredentialType.S3, const=True)
     s3_access_key_id: StrictStr = Field(
         description="S3 access key ID used for connecting to your S3 store."
     )
     s3_secret_access_key: StrictStr = Field(
-        description="S3 secret access key used for connecting to your S3 store. "
+        description="S3 secret access key used for connecting to your S3 store."
         "Avoid storing this in plain text, or in a public repository."
     )
 
 
+class GCSStorageCredential(BaseStorageCredential):
+    """
+    Data class for a GCS storage credential.
+
+    Examples
+    --------
+    >>> gcs_storage_credential = GCSStorageCredential(
+    ...   service_account_info={"type": "service_account", "private_key": "private_key"}
+    ... )
+    """
+
+    __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.GCSStorageCredential")
+
+    type: StorageCredentialType = Field(StorageCredentialType.GCS, const=True)
+    service_account_info: Dict[str, str] = Field(
+        description="Service account information used for connecting to your GCS store."
+    )
+
+
+class AzureBlobStorageCredential(BaseStorageCredential):
+    """
+    Data class for a Azure Blob storage credential.
+
+    Examples
+    --------
+    >>> azure_blob_storage_credential = AzureBlobStorageCredential(
+    ...   account_name="my_azure_storage",
+    ...   account_key="my_azure_storage_key",
+    ... )
+    """
+
+    __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.AzureBlobStorageCredential")
+
+    type: StorageCredentialType = Field(StorageCredentialType.AZURE, const=True)
+    account_name: StrictStr
+    account_key: StrictStr
+
+
 StorageCredential = Annotated[
-    Union[S3StorageCredential],
+    Union[S3StorageCredential, GCSStorageCredential, AzureBlobStorageCredential],
     Field(discriminator="type"),
 ]
 
 
 class CredentialModel(FeatureByteBaseDocumentModel):
     """
     Credential model
```

### Comparing `featurebyte-0.2.2/featurebyte/models/deployment.py` & `featurebyte-0.3.0/featurebyte/models/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/dimension_table.py` & `featurebyte-0.3.0/featurebyte/models/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/entity.py` & `featurebyte-0.3.0/featurebyte/models/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/entity_validation.py` & `featurebyte-0.3.0/featurebyte/models/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/event_table.py` & `featurebyte-0.3.0/featurebyte/models/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/feature.py` & `featurebyte-0.3.0/featurebyte/models/feature.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     FeatureByteBaseModel,
     FeatureByteCatalogBaseDocumentModel,
     PydanticObjectId,
     UniqueConstraintResolutionSignature,
     UniqueValuesConstraint,
     VersionIdentifier,
 )
-from featurebyte.query_graph.enum import NodeType
 from featurebyte.query_graph.graph import QueryGraph
 from featurebyte.query_graph.model.common_table import TabularSource
 from featurebyte.query_graph.model.graph import QueryGraphModel
 from featurebyte.query_graph.node import Node
 from featurebyte.query_graph.node.metadata.operation import GroupOperationStructure
 
 
@@ -147,74 +146,110 @@
                 [
                     ("name", pymongo.TEXT),
                 ],
             ),
         ]
 
 
-class FrozenFeatureModel(FeatureByteCatalogBaseDocumentModel):
+class FeatureModel(FeatureByteCatalogBaseDocumentModel):
     """
-    FrozenFeatureModel store all the attributes that are fixed after object construction.
+    Model for Feature asset
+
+    id: PydanticObjectId
+        Feature id of the object
+    name: str
+        Feature name
+    dtype: DBVarType
+        Variable type of the feature
+    graph: QueryGraph
+        Graph contains steps of transformation to generate the feature
+    node_name: str
+        Node name of the graph which represent the feature
+    tabular_source: TabularSource
+        Tabular source used to construct this feature
+    readiness: FeatureReadiness
+        Feature readiness
+    version: VersionIdentifier
+        Feature version
+    online_enabled: bool
+        Whether to make this feature version online enabled
+    definition: str
+        Feature definition
+    entity_ids: List[PydanticObjectId]
+        Entity IDs used by the feature
+    table_ids: List[PydanticObjectId]
+        Table IDs used by the feature
+    primary_table_ids: Optional[List[PydanticObjectId]]
+        Primary table IDs of the feature (auto-derive from graph)
+    feature_namespace_id: PydanticObjectId
+        Feature namespace id of the object
+    feature_list_ids: List[PydanticObjectId]
+        FeatureList versions which use this feature version
+    deployed_feature_list_ids: List[PydanticObjectId]
+        Deployed FeatureList versions which use this feature version
+    created_at: Optional[datetime]
+        Datetime when the Feature was first saved
+    updated_at: Optional[datetime]
+        When the Feature get updated
     """
 
-    dtype: DBVarType = Field(
-        allow_mutation=False, description="database variable type for the feature"
-    )
+    dtype: DBVarType = Field(allow_mutation=False, default=DBVarType.UNKNOWN)
     graph: QueryGraph = Field(allow_mutation=False)
     node_name: str
     tabular_source: TabularSource = Field(allow_mutation=False)
-    version: VersionIdentifier = Field(
-        allow_mutation=False,
-        default=None,
-        description="Returns the version identifier of a Feature object.",
-    )
-    entity_ids: List[PydanticObjectId] = Field(allow_mutation=False)
+    readiness: FeatureReadiness = Field(allow_mutation=False, default=FeatureReadiness.DRAFT)
+    version: VersionIdentifier = Field(allow_mutation=False, default=None)
+    online_enabled: bool = Field(allow_mutation=False, default=False)
+    definition: Optional[str] = Field(allow_mutation=False, default=None)
+
+    # list of IDs attached to this feature
+    entity_ids: List[PydanticObjectId] = Field(allow_mutation=False, default_factory=list)
     table_ids: List[PydanticObjectId] = Field(allow_mutation=False, default_factory=list)
     primary_table_ids: List[PydanticObjectId] = Field(allow_mutation=False, default_factory=list)
     feature_namespace_id: PydanticObjectId = Field(allow_mutation=False, default_factory=ObjectId)
     feature_list_ids: List[PydanticObjectId] = Field(allow_mutation=False, default_factory=list)
+    deployed_feature_list_ids: List[PydanticObjectId] = Field(
+        allow_mutation=False, default_factory=list
+    )
 
     # pydantic validators
-    _sort_ids_validator = validator("entity_ids", allow_reuse=True)(construct_sort_validator())
     _version_validator = validator("version", pre=True, allow_reuse=True)(version_validator)
 
+    @root_validator
+    @classmethod
+    def _add_derived_attributes(cls, values: dict[str, Any]) -> dict[str, Any]:
+        # extract table ids & entity ids from the graph
+        graph = values["graph"]
+        node_name = values["node_name"]
+        values["primary_table_ids"] = graph.get_primary_table_ids(node_name=node_name)
+        values["table_ids"] = graph.get_table_ids(node_name=node_name)
+        values["entity_ids"] = graph.get_entity_ids(node_name=node_name)
+
+        # extract dtype from the graph
+        node = graph.get_node_by_name(node_name)
+        op_struct = graph.extract_operation_structure(node=node)
+        if len(op_struct.aggregations) != 1:
+            raise ValueError("Feature graph must have exactly one aggregation output")
+
+        values["dtype"] = op_struct.aggregations[0].dtype
+        return values
+
     @property
     def node(self) -> Node:
         """
         Retrieve node
 
         Returns
         -------
         Node
             Node object
         """
 
         return self.graph.get_node_by_name(self.node_name)
 
-    @root_validator
-    @classmethod
-    def _add_derived_attributes(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if values.get("graph") and values.get("node_name"):
-            graph = values["graph"]
-            if isinstance(graph, dict):
-                graph = QueryGraphModel(**dict(graph))
-
-            node_name = values["node_name"]
-            node = graph.get_node_by_name(node_name)
-            primary_input_nodes = graph.get_primary_input_nodes(node_name=node_name)
-            values["primary_table_ids"] = sorted(
-                node.parameters.id for node in primary_input_nodes if node.parameters.id
-            )
-            values["table_ids"] = sorted(
-                node.parameters.id
-                for node in graph.iterate_nodes(target_node=node, node_type=NodeType.INPUT)
-                if node.parameters.id
-            )
-        return values
-
     def extract_pruned_graph_and_node(self, **kwargs: Any) -> tuple[QueryGraphModel, Node]:
         """
         Extract pruned graph and node
 
         Parameters
         ----------
         **kwargs: Any
@@ -244,95 +279,36 @@
 
     class Settings(FeatureByteCatalogBaseDocumentModel.Settings):
         """
         MongoDB settings
         """
 
         collection_name: str = "feature"
-        unique_constraints: List[UniqueValuesConstraint] = [
+        unique_constraints = [
             UniqueValuesConstraint(
                 fields=("_id",),
                 conflict_fields_signature={"id": ["_id"]},
                 resolution_signature=UniqueConstraintResolutionSignature.GET_BY_ID,
             ),
             UniqueValuesConstraint(
                 fields=("name", "version"),
                 conflict_fields_signature={"name": ["name"], "version": ["version"]},
                 resolution_signature=UniqueConstraintResolutionSignature.GET_BY_ID,
             ),
         ]
-
         indexes = FeatureByteCatalogBaseDocumentModel.Settings.indexes + [
             pymongo.operations.IndexModel("dtype"),
             pymongo.operations.IndexModel("version"),
+            pymongo.operations.IndexModel("readiness"),
+            pymongo.operations.IndexModel("online_enabled"),
             pymongo.operations.IndexModel("entity_ids"),
             pymongo.operations.IndexModel("table_ids"),
             pymongo.operations.IndexModel("primary_table_ids"),
             pymongo.operations.IndexModel("feature_namespace_id"),
             pymongo.operations.IndexModel("feature_list_ids"),
-        ]
-
-
-class FeatureModel(FrozenFeatureModel):
-    """
-    Model for Feature entity
-
-    id: PydanticObjectId
-        Feature id of the object
-    name: str
-        Feature name
-    dtype: DBVarType
-        Variable type of the feature
-    graph: QueryGraph
-        Graph contains steps of transformation to generate the feature
-    node_name: str
-        Node name of the graph which represent the feature
-    tabular_source: TabularSource
-        Tabular source used to construct this feature
-    readiness: FeatureReadiness
-        Feature readiness
-    version: VersionIdentifier
-        Feature version
-    online_enabled: bool
-        Whether to make this feature version online enabled
-    entity_ids: List[PydanticObjectId]
-        Entity IDs used by the feature
-    table_ids: List[PydanticObjectId]
-        Table IDs used by the feature
-    primary_table_ids: Optional[List[PydanticObjectId]]
-        Primary table IDs of the feature (auto-derive from graph)
-    feature_namespace_id: PydanticObjectId
-        Feature namespace id of the object
-    feature_list_ids: List[PydanticObjectId]
-        FeatureList versions which use this feature version
-    deployed_feature_list_ids: List[PydanticObjectId]
-        Deployed FeatureList versions which use this feature version
-    created_at: Optional[datetime]
-        Datetime when the Feature was first saved
-    updated_at: Optional[datetime]
-        When the Feature get updated
-    """
-
-    readiness: FeatureReadiness = Field(allow_mutation=False, default=FeatureReadiness.DRAFT)
-    online_enabled: bool = Field(allow_mutation=False, default=False)
-    deployed_feature_list_ids: List[PydanticObjectId] = Field(
-        allow_mutation=False, default_factory=list
-    )
-    definition: Optional[str] = Field(
-        allow_mutation=False, default=None, description="Feature Definition"
-    )
-
-    class Settings(FrozenFeatureModel.Settings):
-        """
-        MongoDB settings
-        """
-
-        indexes = FrozenFeatureModel.Settings.indexes + [
-            pymongo.operations.IndexModel("readiness"),
-            pymongo.operations.IndexModel("online_enabled"),
             pymongo.operations.IndexModel("deployed_feature_list_ids"),
             pymongo.operations.IndexModel(
                 [
                     ("name", pymongo.TEXT),
                     ("version", pymongo.TEXT),
                 ],
             ),
```

### Comparing `featurebyte-0.2.2/featurebyte/models/feature_job_setting_analysis.py` & `featurebyte-0.3.0/featurebyte/models/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/feature_list.py` & `featurebyte-0.3.0/featurebyte/models/feature_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FeatureByteCatalogBaseDocumentModel,
     PydanticObjectId,
     UniqueConstraintResolutionSignature,
     UniqueValuesConstraint,
     VersionIdentifier,
 )
 from featurebyte.models.feature import DefaultVersionMode, FeatureModel, FeatureReadiness
+from featurebyte.models.relationship import RelationshipType
 from featurebyte.query_graph.graph import QueryGraph
 from featurebyte.query_graph.node import Node
 from featurebyte.query_graph.pruning_util import get_prune_graph_and_nodes
 
 
 class FeatureListStatus(OrderedStrEnum):
     """FeatureList status"""
@@ -233,14 +234,26 @@
         Returns
         -------
         List[Node]
         """
         return [self.graph.get_node_by_name(name) for name in self.node_names]
 
 
+class EntityRelationshipInfo(FeatureByteBaseModel):
+    """
+    Schema for entity relationship information (subset of existing RelationshipInfo)
+    """
+
+    id: PydanticObjectId = Field(default_factory=ObjectId, alias="_id", allow_mutation=False)
+    relationship_type: RelationshipType
+    entity_id: PydanticObjectId
+    related_entity_id: PydanticObjectId
+    relation_table_id: PydanticObjectId
+
+
 class FrozenFeatureListNamespaceModel(FeatureByteCatalogBaseDocumentModel):
     """
     FrozenFeatureListNamespaceModel store all the attributes that are fixed after object construction.
     """
 
     feature_namespace_ids: List[PydanticObjectId] = Field(allow_mutation=False)
     dtype_distribution: List[FeatureTypeFeatureCount] = Field(allow_mutation=False)
@@ -425,33 +438,82 @@
             pymongo.operations.IndexModel("status"),
             [
                 ("name", pymongo.TEXT),
             ],
         ]
 
 
-class FrozenFeatureListModel(FeatureByteCatalogBaseDocumentModel):
+class FeatureListModel(FeatureByteCatalogBaseDocumentModel):
     """
-    FrozenFeatureListModel store all the attributes that are fixed after object construction.
+    Model for feature list entity
+
+    id: PydanticObjectId
+        FeatureList id of the object
+    name: str
+        Name of the feature list
+    feature_ids: List[PydanticObjectId]
+        List of feature IDs
+    online_enabled_feature_ids: List[PydanticObjectId]
+        List of online enabled feature version id
+    readiness_distribution: List[Dict[str, Any]]
+        Feature readiness distribution of this feature list
+    version: VersionIdentifier
+        Feature list version
+    deployed: bool
+        Whether to deploy this feature list version
+    feature_list_namespace_id: PydanticObjectId
+        Feature list namespace id of the object
+    created_at: Optional[datetime]
+        Datetime when the FeatureList was first saved or published
+    feature_clusters: List[FeatureCluster]
+        List of combined graphs for features from the same feature store
     """
 
-    feature_ids: List[PydanticObjectId] = Field(default_factory=list)
     version: VersionIdentifier = Field(allow_mutation=False, description="Feature list version")
+    feature_clusters: Optional[List[FeatureCluster]] = Field(allow_mutation=False)  # DEV-556
+    relationships_info: Optional[List[EntityRelationshipInfo]] = Field(
+        allow_mutation=False, default=None  # DEV-556
+    )
+    readiness_distribution: FeatureReadinessDistribution = Field(
+        allow_mutation=False, default_factory=list
+    )
+    deployed: bool = Field(allow_mutation=False, default=False)
+
+    # list of IDs attached to this feature list
+    feature_ids: List[PydanticObjectId]
     feature_list_namespace_id: PydanticObjectId = Field(
         allow_mutation=False, default_factory=ObjectId
     )
-    # DEV-556: no longer Optional once migrated
-    feature_clusters: Optional[List[FeatureCluster]] = Field(allow_mutation=False)
+    online_enabled_feature_ids: List[PydanticObjectId] = Field(
+        allow_mutation=False, default_factory=list
+    )
 
     # pydantic validators
-    _sort_feature_ids_validator = validator("feature_ids", allow_reuse=True)(
-        construct_sort_validator()
-    )
+    _sort_feature_ids_validator = validator(
+        "feature_ids", "online_enabled_feature_ids", allow_reuse=True
+    )(construct_sort_validator())
     _version_validator = validator("version", pre=True, allow_reuse=True)(version_validator)
 
+    @root_validator(pre=True)
+    @classmethod
+    def _derive_feature_related_attributes(cls, values: dict[str, Any]) -> dict[str, Any]:
+        # "features" is not an attribute to the FeatureList model, when it appears in the input to
+        # constructor, it is intended to be used to derive other feature-related attributes
+        if "features" in values:
+            values["readiness_distribution"] = cls.derive_readiness_distribution(values["features"])
+            values["feature_clusters"] = cls.derive_feature_clusters(values["features"])
+            total_count = sum(
+                read_count.count for read_count in values["readiness_distribution"].__root__
+            )
+            if total_count != len(values["feature_ids"]):
+                raise ValueError(
+                    "readiness_distribution total count is different from total feature ids."
+                )
+        return values
+
     @staticmethod
     def derive_readiness_distribution(features: List[FeatureModel]) -> FeatureReadinessDistribution:
         """
         Derive feature readiness distribution from features
 
         Parameters
         ----------
@@ -519,82 +581,18 @@
             ),
             UniqueValuesConstraint(
                 fields=("name", "version"),
                 conflict_fields_signature={"name": ["name"], "version": ["version"]},
                 resolution_signature=UniqueConstraintResolutionSignature.GET_BY_ID,
             ),
         ]
-
         indexes = FeatureByteCatalogBaseDocumentModel.Settings.indexes + [
-            pymongo.operations.IndexModel("version"),
             pymongo.operations.IndexModel("feature_ids"),
             pymongo.operations.IndexModel("feature_list_namespace_id"),
-        ]
-
-
-class FeatureListModel(FrozenFeatureListModel):
-    """
-    Model for feature list entity
-
-    id: PydanticObjectId
-        FeatureList id of the object
-    name: str
-        Name of the feature list
-    feature_ids: List[PydanticObjectId]
-        List of feature IDs
-    online_enabled_feature_ids: List[PydanticObjectId]
-        List of online enabled feature version id
-    readiness_distribution: List[Dict[str, Any]]
-        Feature readiness distribution of this feature list
-    version: VersionIdentifier
-        Feature list version
-    deployed: bool
-        Whether to deploy this feature list version
-    feature_list_namespace_id: PydanticObjectId
-        Feature list namespace id of the object
-    created_at: Optional[datetime]
-        Datetime when the FeatureList was first saved or published
-    feature_clusters: List[FeatureCluster]
-        List of combined graphs for features from the same feature store
-    """
-
-    online_enabled_feature_ids: List[PydanticObjectId] = Field(
-        allow_mutation=False, default_factory=list
-    )
-    readiness_distribution: FeatureReadinessDistribution = Field(
-        allow_mutation=False, default_factory=list
-    )
-    deployed: bool = Field(allow_mutation=False, default=False)
-
-    @root_validator(pre=True)
-    @classmethod
-    def _derive_feature_related_attributes(cls, values: dict[str, Any]) -> dict[str, Any]:
-        # "features" is not an attribute to the FeatureList model, when it appears in the input to
-        # constructor, it is intended to be used to derive other feature-related attributes
-        if "features" in values:
-            values["readiness_distribution"] = cls.derive_readiness_distribution(values["features"])
-            values["feature_clusters"] = cls.derive_feature_clusters(values["features"])
-        return values
-
-    @validator("readiness_distribution")
-    @classmethod
-    def _validate_readiness_distribution(cls, value: Any, values: dict[str, Any]) -> Any:
-        total_count = sum(read_count.count for read_count in value.__root__)
-        if total_count != len(values["feature_ids"]):
-            raise ValueError(
-                "readiness_distribution total count is different from total feature ids."
-            )
-        return value
-
-    class Settings(FrozenFeatureListModel.Settings):
-        """
-        MongoDB settings
-        """
-
-        indexes = FrozenFeatureListModel.Settings.indexes + [
+            pymongo.operations.IndexModel("version"),
             pymongo.operations.IndexModel("online_enabled_feature_ids"),
             pymongo.operations.IndexModel("deployed"),
             [
                 ("name", pymongo.TEXT),
                 ("version", pymongo.TEXT),
             ],
         ]
```

### Comparing `featurebyte-0.2.2/featurebyte/models/feature_store.py` & `featurebyte-0.3.0/featurebyte/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/historical_feature_table.py` & `featurebyte-0.3.0/featurebyte/models/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/item_table.py` & `featurebyte-0.3.0/featurebyte/models/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/materialized_table.py` & `featurebyte-0.3.0/featurebyte/models/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/observation_table.py` & `featurebyte-0.3.0/featurebyte/models/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/online_store.py` & `featurebyte-0.3.0/featurebyte/models/online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/parent_serving.py` & `featurebyte-0.3.0/featurebyte/models/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/periodic_task.py` & `featurebyte-0.3.0/featurebyte/models/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/persistent.py` & `featurebyte-0.3.0/featurebyte/models/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/proxy_table.py` & `featurebyte-0.3.0/featurebyte/models/proxy_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/relationship.py` & `featurebyte-0.3.0/featurebyte/models/relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
     Relationship Type enum
     """
 
     CHILD_PARENT = "child_parent"
 
 
-class RelationshipInfo(FeatureByteCatalogBaseDocumentModel):
+class RelationshipInfoModel(FeatureByteCatalogBaseDocumentModel):
     """
     Relationship info table model.
 
     This differs from the Relationship class above, in that each relationship is stored as a separate document.
     The Relationship class above stores all relationships for a given child in a single document.
     """
```

### Comparing `featurebyte-0.2.2/featurebyte/models/relationship_analysis.py` & `featurebyte-0.3.0/featurebyte/models/relationship_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/request_input.py` & `featurebyte-0.3.0/featurebyte/models/request_input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/scd_table.py` & `featurebyte-0.3.0/featurebyte/models/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/semantic.py` & `featurebyte-0.3.0/featurebyte/models/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/task.py` & `featurebyte-0.3.0/featurebyte/models/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/models/tile.py` & `featurebyte-0.3.0/featurebyte/models/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/persistent/audit.py` & `featurebyte-0.3.0/featurebyte/persistent/audit.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/persistent/base.py` & `featurebyte-0.3.0/featurebyte/persistent/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/persistent/mongo.py` & `featurebyte-0.3.0/featurebyte/persistent/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 from featurebyte.models.persistent import Document, DocumentUpdate, QueryFilter
 from featurebyte.persistent.base import DuplicateDocumentError, Persistent
 
 
 class MongoDB(Persistent):
     """
-    Persistent storage using MongoDB
+    Persistent storage using MongoDB. Note that this class is not thread-safe.
+    Do not use the same instance in multiple threads.
     """
 
     def __init__(self, uri: str, database: str = "featurebyte", client: Any = None) -> None:
         """
         Constructor for MongoDB
 
         Parameters
@@ -332,9 +333,8 @@
         try:
             async with await self._client.start_session() as session:
                 async with session.start_transaction():
                     self._session = session
                     yield self
         finally:
             if self._session:
-                self._session.end_session()
                 self._session = None
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/algorithm.py` & `featurebyte-0.3.0/featurebyte/query_graph/algorithm.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/enum.py` & `featurebyte-0.3.0/featurebyte/query_graph/enum.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/graph.py` & `featurebyte-0.3.0/featurebyte/query_graph/graph.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,21 +22,22 @@
 
 from featurebyte.common.singleton import SingletonMeta
 from featurebyte.query_graph.enum import NodeOutputType, NodeType
 from featurebyte.query_graph.graph_node.base import GraphNode
 from featurebyte.query_graph.model.graph import Edge, GraphNodeNameMap, QueryGraphModel
 from featurebyte.query_graph.node import Node
 from featurebyte.query_graph.node.base import NodeT
-from featurebyte.query_graph.node.generic import GroupByNode
+from featurebyte.query_graph.node.generic import GroupByNode, LookupNode
 from featurebyte.query_graph.node.input import InputNode
 from featurebyte.query_graph.node.metadata.operation import (
     DerivedDataColumn,
     OperationStructure,
     SourceDataColumn,
 )
+from featurebyte.query_graph.node.mixin import BaseGroupbyParameters
 from featurebyte.query_graph.transform.flattening import GraphFlatteningTransformer
 from featurebyte.query_graph.transform.operation_structure import OperationStructureExtractor
 from featurebyte.query_graph.transform.pruning import prune_query_graph
 from featurebyte.query_graph.transform.reconstruction import GraphReconstructionTransformer
 
 
 class QueryGraph(QueryGraphModel):
@@ -72,14 +73,101 @@
             # during the search, it will traverse the left input node first before the right input node.
             # This is important because left input node is the main table for all existing join operations.
             input_node = self.get_input_node(node_name=column.node_name)
             if input_node.name not in node_name_to_input_node:
                 node_name_to_input_node[input_node.name] = input_node
         return list(node_name_to_input_node.values())
 
+    def get_table_ids(self, node_name: str) -> List[ObjectId]:
+        """
+        Get table IDs of the query graph given the target node name
+
+        Parameters
+        ----------
+        node_name: str
+            Name of the node to get table IDs for
+
+        Returns
+        -------
+        List[ObjectId]
+            List of table IDs in the query graph
+        """
+        output = []
+        target_node = self.get_node_by_name(node_name)
+        for node in self.iterate_nodes(target_node=target_node, node_type=NodeType.INPUT):
+            assert isinstance(node, InputNode)
+            if node.parameters.id:
+                output.append(node.parameters.id)
+        return sorted(set(output))
+
+    def get_primary_table_ids(self, node_name: str) -> List[ObjectId]:
+        """
+        Get primary table IDs of the query graph given the target node name
+
+        Parameters
+        ----------
+        node_name: str
+            Name of the node to get primary table IDs for
+
+        Returns
+        -------
+        List[ObjectId]
+            List of primary table IDs in the query graph
+        """
+        primary_input_nodes = self.get_primary_input_nodes(node_name=node_name)
+        return sorted(set(node.parameters.id for node in primary_input_nodes if node.parameters.id))
+
+    def get_entity_ids(self, node_name: str) -> List[ObjectId]:
+        """
+        Get entity IDs of the query graph given the target node name
+
+        Parameters
+        ----------
+        node_name: str
+            Name of the node to get entity IDs for
+
+        Returns
+        -------
+        List[ObjectId]
+            List of entity IDs in the query graph
+        """
+        output = []
+        target_node = self.get_node_by_name(node_name)
+        for node in self.iterate_nodes(target_node=target_node, node_type=None):
+            if isinstance(node.parameters, BaseGroupbyParameters):
+                if node.parameters.entity_ids:
+                    output.extend(node.parameters.entity_ids)
+            elif isinstance(node, LookupNode):
+                output.append(node.parameters.entity_id)
+        return sorted(set(output))
+
+    def get_entity_columns(self, node_name: str) -> List[str]:
+        """
+        Get entity columns of the query graph given the target node name
+
+        Parameters
+        ----------
+        node_name: str
+            Name of the node to get entity columns for
+
+        Returns
+        -------
+        List[str]
+            List of entity columns in the query graph
+        """
+        output = []
+        target_node = self.get_node_by_name(node_name)
+        for node in self.iterate_nodes(target_node=target_node, node_type=None):
+            if isinstance(node.parameters, BaseGroupbyParameters):
+                if node.parameters.entity_ids:
+                    output.extend(node.parameters.keys)
+            elif isinstance(node, LookupNode):
+                output.append(node.parameters.entity_column)
+        return sorted(set(output))
+
     def iterate_group_by_node_and_table_id_pairs(
         self, target_node: Node
     ) -> Iterator[Tuple[GroupByNode, Optional[ObjectId]]]:
         """
         Iterate all GroupBy nodes and their corresponding Table ID
 
         Parameters
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/graph_node/base.py` & `featurebyte-0.3.0/featurebyte/query_graph/graph_node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/model/column_info.py` & `featurebyte-0.3.0/featurebyte/query_graph/model/column_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/model/common_table.py` & `featurebyte-0.3.0/featurebyte/query_graph/model/common_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/model/critical_data_info.py` & `featurebyte-0.3.0/featurebyte/query_graph/model/critical_data_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/model/feature_job_setting.py` & `featurebyte-0.3.0/featurebyte/query_graph/model/feature_job_setting.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,28 +24,26 @@
     - The blind_spot parameter sets the time gap between feature computation and the latest event timestamp to be
     processed.
 
     Note that these parameters are the same duration type strings that pandas accepts in pd.Timedelta().
 
     Examples
     --------
-    Configure a feature job to run daily at 12am
-
-    >>> feature_job_setting = FeatureJobSetting( # doctest: +SKIP
-    ...   blind_spot="0"
-    ...   frequency="24h"
-    ...   time_modulo_frequency="0"
-    ... )
-
-    Configure a feature job to run daily at 8am
-
-    >>> feature_job_setting = FeatureJobSetting( # doctest: +SKIP
-    ...   blind_spot="0"
-    ...   frequency="24h"
-    ...   time_modulo_frequency="8h"
+    Consider a case study where a data warehouse refreshes each hour. The data refresh starts 10 seconds after the hour
+    and is usually finished within 2 minutes. Sometimes the data refresh misses the latest data, up to a maximum of the
+    last 30 seconds at the end of the hour. Therefore, an appropriate feature job settings could be:
+
+    - frequency: 60m
+    = time_modulo_frequency: 10s + 2m + 5s (a safety buffer) = 135s
+    - blind_spot: 30s + 10s + 2m + 5s = 165s
+
+    >>> feature_job_setting = fb.FeatureJobSetting(  # doctest: +SKIP
+    ...  blind_spot="165s"
+    ...  frequency="60m"
+    ...  time_modulo_frequency="135s"
     ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.FeatureJobSetting")
 
     blind_spot: str = Field(
         description="Establishes the time difference between when the feature is calculated and the most recent "
@@ -141,14 +139,45 @@
 class TableFeatureJobSetting(FeatureByteBaseModel):
     """
     The TableFeatureJobSetting object serves as a link between a table and a specific feature job setting configuration.
     It is utilized when creating a new version of a feature that requires different configurations for feature job
     settings. The table_feature_job_settings parameter takes a list of these configurations. For each configuration,
     the TableFeatureJobSetting object establishes the relationship between the table involved and the corresponding
     feature job setting.
+
+    Examples
+    --------
+    Check feature job setting of this feature first:
+
+    >>> feature = catalog.get_feature("InvoiceAmountAvg_60days")
+    >>> feature.info()["table_feature_job_setting"]
+    {'this': [{'table_name': 'GROCERYINVOICE',
+     'feature_job_setting': {'blind_spot': '0s',
+     'frequency': '3600s',
+     'time_modulo_frequency': '90s'}}],
+     'default': [{'table_name': 'GROCERYINVOICE',
+     'feature_job_setting': {'blind_spot': '0s',
+     'frequency': '3600s',
+     'time_modulo_frequency': '90s'}}]}
+
+
+    Create a new feature with a different feature job setting:
+
+    >>> new_feature = feature.create_new_version(  # doctest: +SKIP
+    ...   table_feature_job_settings=[
+    ...     fb.TableFeatureJobSetting(
+    ...       table_name="GROCERYINVOICE",
+    ...       feature_job_setting=fb.FeatureJobSetting(
+    ...         blind_spot="60s",
+    ...         frequency="3600s",
+    ...         time_modulo_frequency="90s",
+    ...       )
+    ...     )
+    ...   ]
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.TableFeatureJobSetting")
 
     table_name: str = Field(
         description="Name of the table to which the feature job setting applies feature_job_setting."
     )
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/model/graph.py` & `featurebyte-0.3.0/featurebyte/query_graph/model/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,33 +360,36 @@
                     )
                     for node, input_order in target_node_input_order_pairs
                 )
             )
             return list(required_columns)
         return []
 
-    def iterate_nodes(self, target_node: Node, node_type: NodeType) -> Iterator[Node]:
+    def iterate_nodes(self, target_node: Node, node_type: Optional[NodeType]) -> Iterator[Node]:
         """
         Iterate all specified nodes in this query graph
 
         Parameters
         ----------
         target_node: Node
             Node from which to start the backward search
-        node_type: NodeType
-            Specific node type to iterate
+        node_type: Optional[NodeType]
+            Specific node type to iterate, if None, iterate all node types
 
         Yields
         ------
         Node
             Query graph nodes of the specified node type
         """
         for node in dfs_traversal(self, target_node):
-            if node.type == node_type:
+            if node_type is None:
                 yield node
+            else:
+                if node.type == node_type:
+                    yield node
 
     def iterate_sorted_graph_nodes(
         self, graph_node_types: Set[GraphNodeType]
     ) -> Iterator[BaseGraphNode]:
         """
         Iterate all specified nodes in this query graph in a topologically sorted order
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/model/table.py` & `featurebyte-0.3.0/featurebyte/query_graph/model/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 class EventTableData(BaseTableData):
     """EventTableData class"""
 
     type: Literal[TableDataType.EVENT_TABLE] = Field(TableDataType.EVENT_TABLE, const=True)
     id: PydanticObjectId = Field(default_factory=ObjectId, alias="_id")
     event_timestamp_column: StrictStr
     event_id_column: StrictStr
-    event_timestamp_timezone_offset: Optional[str] = Field(default=None)
-    event_timestamp_timezone_offset_column: Optional[str] = Field(default=None)
+    event_timestamp_timezone_offset: Optional[StrictStr] = Field(default=None)
+    event_timestamp_timezone_offset_column: Optional[StrictStr] = Field(default=None)
 
     @property
     def primary_key_columns(self) -> List[str]:
         if self.event_id_column:
             return [self.event_id_column]
         return []  # DEV-556: event_id_column should not be empty
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/__init__.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/agg_func.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/agg_func.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/base.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,19 +17,22 @@
     OperationStructure,
     OperationStructureBranchState,
     OperationStructureInfo,
     PostAggregationColumn,
 )
 from featurebyte.query_graph.node.metadata.sdk_code import (
     CodeGenerationConfig,
+    CodeGenerationContext,
     ExpressionStr,
+    InfoDict,
     StatementT,
     ValueStr,
     VariableNameGenerator,
     VariableNameStr,
+    VarNameExpressionInfo,
     VarNameExpressionStr,
 )
 from featurebyte.query_graph.node.scalar import ValueParameterType
 
 NODE_TYPES = []
 NodeT = TypeVar("NodeT", bound="BaseNode")
 
@@ -96,14 +99,49 @@
         if parameters and len(parameters) < 4:
             # Note: 4 is chosen here so that the info is more readable, with too many
             # parameters presented here, it is hard to read. This value currently is only
             # used for the signal type tagging (for feature theme).
             return f"{str(self.type).lower()}({', '.join(parameters)})"
         return str(self.type).lower()
 
+    @property
+    def is_inplace_operation_in_sdk_code(self) -> bool:
+        """
+        Check if this node is an inplace operation in SDK code. For example, if the SDK code generated
+        for this node is `view['new_col'] = 1`, then this node is an inplace operation as it will modify
+        the input view object inplace. If the SDK code generated for this node is something like
+        `joined_view = view.join_event_table_attributes(["col_float"])`, then this node is not an inplace
+        operation as it will not modify the input view object inplace.
+
+        Returns
+        -------
+        bool
+        """
+        return False
+
+    @staticmethod
+    def _assert_no_info_dict(inputs: List[VarNameExpressionInfo]) -> List[VarNameExpressionStr]:
+        """
+        Assert there is no info dict in the given inputs & convert the type to VarNameExpressionStr
+
+        Parameters
+        ----------
+        inputs: List[VarNameExpressionInfoStr]
+            List of inputs
+
+        Returns
+        -------
+        List[VarNameExpressionStr]
+        """
+        out = []
+        for input_ in inputs:
+            assert not isinstance(input_, InfoDict)
+            out.append(input_)
+        return out
+
     @classmethod
     def detect_var_type_from_value(cls, value: Any) -> DBVarType:
         """
         Detect variable type of the given scalar value
 
         Parameters
         ----------
@@ -224,63 +262,64 @@
             "is_time_based": any(input_.is_time_based for input_ in inputs)
             or operation_info.is_time_based,
         }
         return OperationStructure(**{**operation_info.dict(), **update_args})
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         """
         Derive SDK codes based on the graph traversal from starting node(s) to this node
 
         Parameters
         ----------
-        input_var_name_expressions: List[VarNameExpressionStr]
-            Input variables name
-        input_node_types: List[NodeType]
-            Input node types
+        node_inputs: List[VarNameExpressionStr]
+            Node inputs to derive SDK code
         var_name_generator: VariableNameGenerator
             Variable name generator
         operation_structure: OperationStructure
             Operation structure of current node
         config: CodeGenerationConfig
             Code generation configuration
+        context: CodeGenerationContext
+            Context for code generation
 
         Returns
         -------
         Tuple[List[StatementT], VarNameExpressionStr]
         """
-        statements, var_name_expression = self._derive_sdk_code(
-            input_var_name_expressions=input_var_name_expressions,
-            input_node_types=input_node_types,
+        statements, var_name_expression_info = self._derive_sdk_code(
+            node_inputs=node_inputs,
             var_name_generator=var_name_generator,
             operation_structure=operation_structure,
             config=config,
+            context=context,
         )
 
         if (
             self._auto_convert_expression_to_variable
-            and isinstance(var_name_expression, ExpressionStr)
-            and len(var_name_expression) > config.max_expression_length
+            and isinstance(var_name_expression_info, ExpressionStr)
+            and len(var_name_expression_info) > config.max_expression_length
         ):
             # if the output of the var_name_expression is an expression and
             # the length of expression exceeds limit specified in code generation config,
             # then assign a new variable to reduce line width.
             var_name = var_name_generator.generate_variable_name(
                 node_output_type=operation_structure.output_type,
                 node_output_category=operation_structure.output_category,
+                node_name=self.name,
             )
-            statements.append((var_name, var_name_expression))
+            statements.append((var_name, var_name_expression_info))
             return statements, var_name
-        return statements, var_name_expression
+        return statements, var_name_expression_info
 
     def clone(self: NodeT, **kwargs: Any) -> NodeT:
         """
         Clone an existing object with certain update
 
         Parameters
         ----------
@@ -311,49 +350,110 @@
         Returns
         -------
         NodeT
         """
         _ = target_node_input_order_pairs, input_operation_structures
         return self
 
-    @staticmethod
     def _convert_expression_to_variable(
+        self,
         var_name_expression: VarNameExpressionStr,
         var_name_generator: VariableNameGenerator,
         node_output_type: NodeOutputType,
         node_output_category: NodeOutputCategory,
+        to_associate_with_node_name: bool,
+        variable_name_prefix: Optional[str] = None,
     ) -> Tuple[List[StatementT], VariableNameStr]:
         """
         Convert expression to variable
 
         Parameters
         ----------
         var_name_expression: VarNameExpressionStr
             Variable name expression
         var_name_generator: VariableNameGenerator
             Variable name generator
         node_output_type: NodeOutputType
             Node output type
         node_output_category: NodeOutputCategory
             Node output category
+        to_associate_with_node_name: bool
+            Whether to associate the variable name with the node name
+        variable_name_prefix: Optional[str]
+            Variable name prefix (if any)
 
         Returns
         -------
         VarNameStr
         """
         statements: List[StatementT] = []
         if isinstance(var_name_expression, ExpressionStr):
-            var_name = var_name_generator.generate_variable_name(
-                node_output_type=node_output_type,
-                node_output_category=node_output_category,
-            )
+            if variable_name_prefix:
+                var_name = var_name_generator.convert_to_variable_name(
+                    variable_name_prefix=variable_name_prefix,
+                    node_name=self.name if to_associate_with_node_name else None,
+                )
+            else:
+                var_name = var_name_generator.generate_variable_name(
+                    node_output_type=node_output_type,
+                    node_output_category=node_output_category,
+                    node_name=self.name if to_associate_with_node_name else None,
+                )
             statements.append((var_name, var_name_expression))
             return statements, var_name
         return statements, var_name_expression
 
+    def _convert_to_proper_variable_name(
+        self,
+        var_name: VariableNameStr,
+        var_name_generator: VariableNameGenerator,
+        operation_structure: OperationStructure,
+        required_copy: bool,
+        to_associate_with_node_name: bool,
+    ) -> Tuple[List[StatementT], VariableNameStr]:
+        """
+        This method is used to convert variable name to proper variable name if the variable name is
+        not a valid identifier.
+
+        Parameters
+        ----------
+        var_name: VariableNameStr
+            Variable name
+        var_name_generator: VariableNameGenerator
+            Variable name generator
+        operation_structure: OperationStructure
+            Operation structure of current node
+        required_copy: bool
+            Whether a copy is required
+        to_associate_with_node_name: bool
+            Whether to associate the variable name with the node name
+
+        Returns
+        -------
+        Tuple[List[StatementT], VariableNameStr]
+        """
+        output_var_name = var_name
+        statements: List[StatementT] = []
+        is_var_name_valid_identifier = var_name.isidentifier()
+        if required_copy or not is_var_name_valid_identifier:
+            output_var_name = var_name_generator.generate_variable_name(
+                node_output_type=operation_structure.output_type,
+                node_output_category=operation_structure.output_category,
+                node_name=self.name if to_associate_with_node_name else None,
+            )
+            if required_copy:
+                # Copy is required as the input will be used by other nodes. This is to avoid unexpected
+                # side effects when the input is modified by other nodes.
+                statements.append((output_var_name, ExpressionStr(f"{var_name}.copy()")))
+            else:
+                # This is to handle the case where the var_name is not a valid variable name,
+                # so we need to assign it to a valid variable name first.
+                statements.append((output_var_name, ExpressionStr(var_name)))
+        return statements, output_var_name
+
     @abstractmethod
     def _derive_node_operation_info(
         self,
         inputs: List[OperationStructure],
         branch_state: OperationStructureBranchState,
         global_state: OperationStructureInfo,
     ) -> OperationStructure:
@@ -372,43 +472,44 @@
         Returns
         -------
         OperationStructure
         """
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         """
         Derive SDK codes based to be implemented at the concrete node class
 
         Parameters
         ----------
-        input_var_name_expressions: List[VarNameExpression]
-            Input variables name
-        input_node_types: List[NodeType]
-            Input node types
+        node_inputs: List[VarNameExpression]
+            Inputs for this node to generate SDK codes
         var_name_generator: VariableNameGenerator
             Variable name generator
         operation_structure: OperationStructure
             Operation structure of current node
         config: CodeGenerationConfig
             Code generation configuration
+        context: CodeGenerationContext
+            Context for code generation
 
         Returns
         -------
         Tuple[List[StatementT], VarNameExpression]
         """
         # TODO: convert this method to an abstract method and remove the following dummy implementation
-        _ = input_node_types, var_name_generator, operation_structure, config
-        input_params = ", ".join(input_var_name_expressions)
+        _ = var_name_generator, operation_structure, config, context
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        input_params = ", ".join(var_name_expressions)
         expression = ExpressionStr(f"{self.type}({input_params})")
         return [], expression
 
     @property
     @abstractmethod
     def max_input_count(self) -> int:
         """
@@ -598,20 +699,21 @@
         """
         # TODO: make this method abstract and remove the following dummy implementation
         _ = left_operand, right_operand
         return ""
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        input_var_name_expressions = self._assert_no_info_dict(node_inputs)
         left_operand: str = input_var_name_expressions[0].as_input()
         right_operand: str = ValueStr.create(self.parameters.value).as_input()
         if len(input_var_name_expressions) == 2:
             right_operand = input_var_name_expressions[1].as_input()
         left_operand, right_operand = self._reorder_operands(left_operand, right_operand)
         return [], ExpressionStr(self.generate_expression(left_operand, right_operand))
 
@@ -677,20 +779,21 @@
         Returns
         -------
         str
         """
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        input_var_name_expressions = self._assert_no_info_dict(node_inputs)
         var_name_expression = input_var_name_expressions[0]
         return [], self._derive_sdk_code_return_var_name_expression_type(
             self.generate_expression(var_name_expression.as_input())
         )
 
 
 class BasePrunableNode(BaseNode):
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/binary.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/cleaning_operation.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/cleaning_operation.py`

 * *Files 11% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     """
     MissingValueImputation class is used to declare the operation to impute the missing value of a table column.
 
     Examples
     --------
     Create an imputation rule to replace missing value with 0
 
-    >>> MissingValueImputation(imputed_value=0) # doctest: +SKIP
+    >>> fb.MissingValueImputation(imputed_value=0) # doctest: +SKIP
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.MissingValueImputation")
 
     type: Literal[ConditionOperationField.MISSING] = Field(
         ConditionOperationField.MISSING, const=True
     )
@@ -164,15 +164,19 @@
     If the imputed_value parameter is None, the values to impute are replaced by missing values and the corresponding
     rows are ignored during aggregation operations.
 
     Examples
     --------
     Create an imputation rule to replace -999 with 0
 
-    >>> DisguisedValueImputation(disguised_values=[-999], imputed_value=0) # doctest: +SKIP
+    >>> fb.DisguisedValueImputation(disguised_values=[-999], imputed_value=0)  # doctest: +SKIP
+
+    Create an imputation rule to treat -1 and -96 as missing
+
+    >>> fb.DisguisedValueImputation(disguised_values=[-1, -96], imputed_value=None)  # doctest: +SKIP
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.DisguisedValueImputation")
 
     type: Literal[ConditionOperationField.DISGUISED] = Field(
         ConditionOperationField.DISGUISED, const=True
     )
@@ -205,15 +209,15 @@
     If the imputed_value parameter is None, the values to impute are replaced by missing values and the corresponding
     rows are ignored during aggregation operations.
 
     Examples
     --------
     Create an imputation rule to replace value other than "buy" or "sell" to "missing"
 
-    >>> UnexpectedValueImputation(expected_values=["buy", "sell"], imputed_value="missing") # doctest: +SKIP
+    >>> fb.UnexpectedValueImputation(expected_values=["buy", "sell"], imputed_value="missing") # doctest: +SKIP
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.UnexpectedValueImputation")
 
     type: Literal[ConditionOperationField.NOT_IN] = Field(
         ConditionOperationField.NOT_IN, const=True
     )
@@ -250,17 +254,25 @@
     column exceeds a specified endpoint type.
 
     If the imputed_value parameter is None, the values to impute are replaced by missing values and the corresponding
     rows are ignored during aggregation operations.
 
     Examples
     --------
-    Create an imputation rule to replace value less than 0 to 0
+    Create an imputation rule to replace value less than 0 to 0.
+
+    >>> fb.ValueBeyondEndpointImputation(type="less_than", end_point=0, imputed_value=0) # doctest: +SKIP
+
 
-    >>> ValueBeyondEndpointImputation(type="less_than", end_point=0, imputed_value=0) # doctest: +SKIP
+    Create an imputation rule to ignore value higher than 1M.
+
+    >>> fb.ValueBeyondEndpointImputation(
+    ...   type="less_than", end_point=1e6, imputed_value=None
+    ... )
+    ValueBeyondEndpointImputation(imputed_value=None, type=less_than, end_point=1000000.0)
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.ValueBeyondEndpointImputation")
 
     type: Literal[
         ConditionOperationField.LESS_THAN,
         ConditionOperationField.LESS_THAN_OR_EQUAL,
@@ -322,15 +334,15 @@
     If the imputed_value parameter is None, the values to impute are replaced by missing values and the corresponding
     rows are ignored during aggregation operations.
 
     Examples
     --------
     Create an imputation rule to replace string value with 0
 
-    >>> StringValueImputation(imputed_value=0) # doctest: +SKIP
+    >>> fb,StringValueImputation(imputed_value=0) # doctest: +SKIP
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.StringValueImputation")
 
     type: Literal[ConditionOperationField.IS_STRING] = Field(
         ConditionOperationField.IS_STRING, const=True
     )
@@ -365,14 +377,39 @@
 class ColumnCleaningOperation(FeatureByteBaseModel):
     """
     The ColumnCleaningOperation object serves as a link between a table column and a specific cleaning configuration.
     It is utilized when creating a view in the manual mode that requires different configurations per colum. The
     column_cleaning_operations parameter takes a list of these configurations. For each configuration, the
     ColumnCleaningOperation object establishes the relationship between the colum involved and the corresponding
     cleaning operations.
+
+    Examples
+    --------
+    Check table cleaning operation of this feature first:
+
+    >>> feature = catalog.get_feature("InvoiceAmountAvg_60days")
+    >>> feature.info()["table_cleaning_operation"]
+    {'this': [], 'default': []}
+
+
+    Create a new version of a feature with different table cleaning operations:
+
+    >>> new_feature = feature.create_new_version(  # doctest: +SKIP
+    ...   table_cleaning_operations=[
+    ...     fb.TableCleaningOperation(
+    ...       table_name="GROCERYINVOICE",
+    ...       column_cleaning_operations=[
+    ...         fb.ColumnCleaningOperation(
+    ...           column_name="Amount",
+    ...           cleaning_operations=[fb.MissingValueImputation(imputed_value=0.0)],
+    ...         )
+    ...       ],
+    ...     )
+    ...   ]
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.ColumnCleaningOperation")
 
     column_name: str = Field(
         description="Name of the column that requires cleaning. The cleaning operations specified in the second "
         "parameter will be applied to this column."
@@ -389,14 +426,39 @@
 class TableCleaningOperation(FeatureByteBaseModel):
     """
     The TableCleaningOperation object serves as a link between a table and cleaning configurations for the columns in
     the table. It is utilized when creating a new version of a feature that requires different cleaning configurations.
     The table_cleaning_operations parameter takes a list of these configurations. For each configuration, the
     ColumnCleaningOperation object establishes the relationship between the table and the corresponding cleaning
     operations for the table.
+
+    Examples
+    --------
+    Check table cleaning operation of this feature first:
+
+    >>> feature = catalog.get_feature("InvoiceAmountAvg_60days")
+    >>> feature.info()["table_cleaning_operation"]
+    {'this': [], 'default': []}
+
+
+    Create a new version of a feature with different table cleaning operations:
+
+    >>> new_feature = feature.create_new_version(
+    ...   table_cleaning_operations=[
+    ...     fb.TableCleaningOperation(
+    ...       table_name="GROCERYINVOICE",
+    ...       column_cleaning_operations=[
+    ...         fb.ColumnCleaningOperation(
+    ...           column_name="Amount",
+    ...           cleaning_operations=[fb.MissingValueImputation(imputed_value=0.0)],
+    ...         )
+    ...       ],
+    ...     )
+    ...   ]
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.TableCleaningOperation")
 
     table_name: str = Field(
         description="Name of the table that requires cleaning. The cleaning operations specified in the second "
         "parameter will be applied to this table."
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/count_dict.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/count_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 from featurebyte.enum import DBVarType
 from featurebyte.query_graph.enum import NodeType
 from featurebyte.query_graph.node.agg_func import construct_agg_func
 from featurebyte.query_graph.node.base import BaseSeriesOutputNode
 from featurebyte.query_graph.node.metadata.operation import AggregationColumn, OperationStructure
 from featurebyte.query_graph.node.metadata.sdk_code import (
     CodeGenerationConfig,
+    CodeGenerationContext,
     ExpressionStr,
     StatementT,
     ValueStr,
     VariableNameGenerator,
-    VarNameExpressionStr,
+    VarNameExpressionInfo,
 )
 
 
 class BaseCountDictOpNode(BaseSeriesOutputNode, ABC):
     """BaseCountDictOpNode class"""
 
     @property
@@ -35,22 +36,23 @@
     def _get_required_input_columns(
         self, input_index: int, available_column_names: List[str]
     ) -> Sequence[str]:
         return self._assert_empty_required_input_columns()
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expression = input_var_name_expressions[0].as_input()
-        other_operands = [val.as_input() for val in input_var_name_expressions[1:]]
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        var_name_expression = var_name_expressions[0].as_input()
+        other_operands = [val.as_input() for val in var_name_expressions[1:]]
         expression = ExpressionStr(
             self.generate_expression(operand=var_name_expression, other_operands=other_operands)
         )
         return [], expression
 
     @abstractmethod
     def generate_expression(self, operand: str, other_operands: List[str]) -> str:
@@ -128,21 +130,21 @@
         return self._assert_empty_required_input_columns()
 
     def derive_var_type(self, inputs: List[OperationStructure]) -> DBVarType:
         return DBVarType.ARRAY
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        return [], input_var_name_expressions[0]
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        return [], node_inputs[0]
 
 
 class GetValueFromDictionaryNode(BaseCountDictOpNode):
     """Get value from dictionary node class"""
 
     class Parameters(BaseModel):
         """Parameters"""
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/date.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/date.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     BaseSeriesOutputNode,
     BaseSeriesOutputWithSingleOperandNode,
 )
 from featurebyte.query_graph.node.metadata.operation import OperationStructure
 from featurebyte.query_graph.node.metadata.sdk_code import (
     ClassEnum,
     CodeGenerationConfig,
+    CodeGenerationContext,
     ExpressionStr,
     StatementT,
     ValueStr,
     VariableNameGenerator,
     VariableNameStr,
-    VarNameExpressionStr,
+    VarNameExpressionInfo,
 )
 
 
 class DatetimeExtractNode(BaseSeriesOutputNode):
     """DatetimeExtractNode class"""
 
     class Parameters(BaseModel):
@@ -48,35 +49,36 @@
     def _get_required_input_columns(
         self, input_index: int, available_column_names: List[str]
     ) -> Sequence[str]:
         return self._assert_empty_required_input_columns()
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        ts_operand: str = input_var_name_expressions[0].as_input()
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        ts_operand: str = var_name_expressions[0].as_input()
 
         offset_operand: Optional[str]
         if self.parameters.timezone_offset is not None:
             offset_operand = ValueStr.create(self.parameters.timezone_offset).as_input()
-        elif len(input_var_name_expressions) == 2:
-            offset_operand = input_var_name_expressions[1].as_input()
+        elif len(var_name_expressions) == 2:
+            offset_operand = var_name_expressions[1].as_input()
         else:
             offset_operand = None
 
         date_property: str = self.parameters.property
         if date_property == "dayofweek":
             date_property = "day_of_week"
 
-        output: VarNameExpressionStr
+        output: VarNameExpressionInfo
         if offset_operand is None:
             output = VariableNameStr(f"{ts_operand}.dt.{date_property}")
         else:
             output = ExpressionStr(f"{ts_operand}.dt.tz_offset({offset_operand}).{date_property}")
 
         return [], output
 
@@ -114,22 +116,23 @@
         return self._assert_empty_required_input_columns()
 
     def derive_var_type(self, inputs: List[OperationStructure]) -> DBVarType:
         return DBVarType.TIMEDELTA
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        left_operand: str = input_var_name_expressions[0].as_input()
-        right_operand = input_var_name_expressions[1].as_input()
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        left_operand: str = var_name_expressions[0].as_input()
+        right_operand = var_name_expressions[1].as_input()
         return [], ExpressionStr(f"{left_operand} - {right_operand}")
 
 
 class TimeDelta(BaseSeriesOutputNode):
     """TimeDelta class"""
 
     class Parameters(BaseModel):
@@ -150,25 +153,27 @@
         return self._assert_empty_required_input_columns()
 
     def derive_var_type(self, inputs: List[OperationStructure]) -> DBVarType:
         return DBVarType.TIMEDELTA
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expression = input_var_name_expressions[0]
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        var_name_expression = var_name_expressions[0]
         statements: List[StatementT] = []
         var_name = var_name_generator.generate_variable_name(
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            node_name=self.name,
         )
         obj = ClassEnum.TO_TIMEDELTA(series=var_name_expression, unit=self.parameters.unit)
         statements.append((var_name, obj))
         return statements, var_name
 
 
 class DateAdd(BaseSeriesOutputNode):
@@ -192,16 +197,17 @@
         return self._assert_empty_required_input_columns()
 
     def derive_var_type(self, inputs: List[OperationStructure]) -> DBVarType:
         return inputs[0].columns[0].dtype
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        left_operand: str = input_var_name_expressions[0].as_input()
-        right_operand = input_var_name_expressions[1].as_input()
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        left_operand: str = var_name_expressions[0].as_input()
+        right_operand = var_name_expressions[1].as_input()
         return [], ExpressionStr(f"{left_operand} + {right_operand}")
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/generic.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/generic.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,22 +27,24 @@
     OperationStructureInfo,
     PostAggregationColumn,
     ViewDataColumn,
 )
 from featurebyte.query_graph.node.metadata.sdk_code import (
     ClassEnum,
     CodeGenerationConfig,
+    CodeGenerationContext,
     ExpressionStr,
+    InfoDict,
     ObjectClass,
     RightHandSide,
     StatementT,
     ValueStr,
     VariableNameGenerator,
     VariableNameStr,
-    VarNameExpressionStr,
+    VarNameExpressionInfo,
     get_object_class_from_function_call,
 )
 from featurebyte.query_graph.node.mixin import AggregationOpStructMixin, BaseGroupbyParameters
 from featurebyte.query_graph.util import append_to_lineage
 
 
 class ProjectNode(BaseNode):
@@ -113,41 +115,32 @@
             output_type=self.output_type,
             output_category=output_category,
             row_index_lineage=input_operation_info.row_index_lineage,
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expr = input_var_name_expressions[0]
-        if input_node_types[0] in {NodeType.ITEM_GROUPBY, NodeType.AGGREGATE_AS_AT}:
-            # special handling for item_view.aggregate output
-            # since the output is already single series, no projection is needed
-            statements, var_name = self._convert_expression_to_variable(
-                var_name_expression=var_name_expr,
-                var_name_generator=var_name_generator,
-                node_output_type=operation_structure.output_type,
-                node_output_category=operation_structure.output_category,
-            )
-            return statements, var_name
-
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         statements, var_name = self._convert_expression_to_variable(
-            var_name_expression=var_name_expr,
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=operation_structure.output_category,
+            to_associate_with_node_name=False,
         )
         out_var_name = var_name_generator.generate_variable_name(
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            node_name=self.name,
         )
 
         # must assign the projection result to a new variable
         # otherwise, it could cause issue when the original variable is modified
         # for example, the second `view["col_int", "col_float"]]` is different from the first one:
         #     view.join(view["col_int", "col_float"]], rsuffix="_y")
         #     view.join(view["col_int", "col_float"]], rsuffix="_z")
@@ -220,28 +213,30 @@
             output_type=input_operation_info.output_type,
             output_category=output_category,
             row_index_lineage=append_to_lineage(input_operation_info.row_index_lineage, self.name),
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expr = input_var_name_expressions[0]
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        var_name_expr = var_name_expressions[0]
         statements, var_name = self._convert_expression_to_variable(
             var_name_expression=var_name_expr,
             var_name_generator=var_name_generator,
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            to_associate_with_node_name=False,
         )
-        mask_name = input_var_name_expressions[1].as_input()
+        mask_name = var_name_expressions[1].as_input()
         expression = ExpressionStr(f"{var_name}[{mask_name}]")
         return statements, expression
 
 
 class AssignColumnMixin:
     """AssignColumnMixin class"""
 
@@ -327,14 +322,18 @@
     output_type: NodeOutputType = Field(NodeOutputType.FRAME, const=True)
     parameters: Parameters
 
     @property
     def max_input_count(self) -> int:
         return 2
 
+    @property
+    def is_inplace_operation_in_sdk_code(self) -> bool:
+        return True
+
     def _get_required_input_columns(
         self, input_index: int, available_column_names: List[str]
     ) -> Sequence[str]:
         return self._assert_empty_required_input_columns()
 
     @staticmethod
     def _validate_series(series_op_structure: OperationStructure) -> None:
@@ -367,33 +366,57 @@
             columns=columns,
             node_name=self.name,
             new_column_var_type=dtype,
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expr = input_var_name_expressions[0]
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expr = node_inputs[0]
+        assert not isinstance(var_name_expr, InfoDict)
         column_name = self.parameters.name
         statements, var_name = self._convert_expression_to_variable(
             var_name_expression=var_name_expr,
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=operation_structure.output_category,
+            to_associate_with_node_name=False,
         )
-        value: RightHandSide = ValueStr.create(self.parameters.value)
-        if len(input_var_name_expressions) == 2:
-            value = input_var_name_expressions[1]
-        statements.append((VariableNameStr(f"{var_name}['{column_name}']"), value))
-        return statements, var_name
+        second_input = None
+        if len(node_inputs) == 2:
+            second_input = node_inputs[1]
+
+        output_var_name = var_name
+        if context.required_copy:
+            output_var_name = var_name_generator.generate_variable_name(
+                node_output_type=operation_structure.output_type,
+                node_output_category=operation_structure.output_category,
+                node_name=self.name,
+            )
+            statements.append((output_var_name, ExpressionStr(f"{var_name}.copy()")))
+
+        value: RightHandSide
+        if isinstance(second_input, InfoDict):
+            mask_var = second_input["mask"]
+            value = ValueStr.create(second_input["value"])
+            statements.append(
+                (
+                    VariableNameStr(f"{output_var_name}['{column_name}'][{mask_var}]"),
+                    value,
+                )
+            )
+        else:
+            value = second_input if second_input else ValueStr.create(self.parameters.value)
+            statements.append((VariableNameStr(f"{output_var_name}['{column_name}']"), value))
+        return statements, output_var_name
 
 
 class LagNode(BaseSeriesOutputNode):
     """LagNode class"""
 
     class Parameters(BaseModel):
         """Parameters"""
@@ -427,21 +450,22 @@
         return [self.parameters.entity_columns[input_index - 1]]
 
     def derive_var_type(self, inputs: List[OperationStructure]) -> DBVarType:
         return inputs[0].series_output_dtype
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        col_name = input_var_name_expressions[0].as_input()
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        col_name = var_name_expressions[0].as_input()
         entity_columns = ValueStr.create(self.parameters.entity_columns)
         offset = ValueStr.create(self.parameters.offset)
         expression = f"{col_name}.lag(entity_columns={entity_columns}, offset={offset})"
         return [], ExpressionStr(expression)
 
 
 class GroupByNode(AggregationOpStructMixin, BaseNode):
@@ -526,37 +550,40 @@
                     pruned_params_dict["names"].append(name)
                     pruned_params_dict["windows"].append(window)
             return self.clone(parameters=pruned_params_dict)
         return self
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         statements, var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[0],
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         keys = ValueStr.create(self.parameters.keys)
         category = ValueStr.create(self.parameters.value_by)
         feature_job_setting: ObjectClass = ClassEnum.FEATURE_JOB_SETTING(
             blind_spot=f"{self.parameters.blind_spot}s",
             frequency=f"{self.parameters.frequency}s",
             time_modulo_frequency=f"{self.parameters.time_modulo_frequency}s",
         )
         grouped = f"{var_name}.groupby(by_keys={keys}, category={category})"
         out_var_name = var_name_generator.generate_variable_name(
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            node_name=self.name,
         )
         expression = get_object_class_from_function_call(
             callable_name=f"{grouped}.aggregate_over",
             value_column=self.parameters.parent,
             method=self.parameters.agg_func,
             windows=self.parameters.windows,
             feature_names=self.parameters.names,
@@ -620,29 +647,31 @@
                 node_name=node_name,
                 dtype=output_var_type,
             )
         ]
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # Note: this node is a special case as the output of this node is not a complete SDK code.
         # Currently, `item_view.groupby(...).aggregate()` will generate ItemGroupbyNode + ProjectNode.
         # Output of ItemGroupbyNode is just an expression, the actual variable assignment
         # will be done at the ProjectNode.
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         statements, var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[0],
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         keys = ValueStr.create(self.parameters.keys)
         category = ValueStr.create(self.parameters.value_by)
         value_column = ValueStr.create(self.parameters.parent)
         method = ValueStr.create(self.parameters.agg_func)
         feature_name = ValueStr.create(self.parameters.name)
         grouped = f"{var_name}.groupby(by_keys={keys}, category={category})"
@@ -765,49 +794,51 @@
         ]
 
     def _exclude_source_columns(self) -> List[str]:
         return [self.parameters.entity_column]
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         statements, var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[0],
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         input_column_names = self.parameters.input_column_names
         feature_names = self.parameters.feature_names
         offset = None
         if self.parameters.scd_parameters:
             offset = self.parameters.scd_parameters.offset
         grouped = (
             f"{var_name}.as_features(column_names={input_column_names}, "
             f"feature_names={feature_names}, "
             f"offset={ValueStr.create(offset)})"
         )
         out_var_name = var_name_generator.generate_variable_name(
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            node_name=self.name,
         )
         statements.append((out_var_name, ExpressionStr(grouped)))
         return statements, out_var_name
 
 
 class JoinMetadata(BaseModel):
     """Metadata to track general `view.join(...)` operation"""
 
     type: str = Field("join", const=True)
-    on: Optional[str]
     rsuffix: str
 
 
 class JoinEventTableAttributesMetadata(BaseModel):
     """Metadata to track `item_view.join_event_table_attributes(...)` operation"""
 
     type: str = Field("join_event_table_attributes", const=True)
@@ -983,51 +1014,56 @@
             output_type=NodeOutputType.FRAME,
             output_category=NodeOutputCategory.VIEW,
             row_index_lineage=row_index_lineage,
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         left_statements, left_var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[0],
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         right_statements, right_var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[1],
+            var_name_expression=var_name_expressions[1],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         statements = left_statements + right_statements
         var_name = left_var_name
         assert self.parameters.metadata is not None, "Join node metadata is not set."
         if isinstance(self.parameters.metadata, JoinMetadata):
             other_var_name = right_var_name
             expression = ExpressionStr(
                 f"{var_name}.join({other_var_name}, "
-                f"on={ValueStr.create(self.parameters.metadata.on)}, "
+                f"on={ValueStr.create(self.parameters.left_on)}, "
                 f"how={ValueStr.create(self.parameters.join_type)}, "
                 f"rsuffix={ValueStr.create(self.parameters.metadata.rsuffix)})"
             )
         else:
             expression = ExpressionStr(
                 f"{var_name}.join_event_table_attributes("
                 f"columns={ValueStr.create(self.parameters.metadata.columns)}, "
                 f"event_suffix={ValueStr.create(self.parameters.metadata.event_suffix)})"
             )
 
-        var_name = var_name_generator.convert_to_variable_name(variable_name_prefix="joined_view")
+        var_name = var_name_generator.convert_to_variable_name(
+            variable_name_prefix="joined_view", node_name=self.name
+        )
         statements.append((var_name, expression))
         return statements, var_name
 
 
 class JoinFeatureNode(AssignColumnMixin, BasePrunableNode):
     """JoinFeatureNode class
 
@@ -1106,36 +1142,40 @@
             columns=feature_operation_info.columns,
             node_name=self.name,
             new_column_var_type=feature_operation_info.series_output_dtype,
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         new_column_name = ValueStr.create(self.parameters.name)
-        feature = input_var_name_expressions[1]
+        feature = var_name_expressions[1]
         entity_column = ValueStr.create(self.parameters.view_entity_column)
         statements, var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[0],
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         expression = ExpressionStr(
             f"{var_name}.add_feature(new_column_name={new_column_name}, "
             f"feature={feature}, entity_column={entity_column})"
         )
-        var_name = var_name_generator.convert_to_variable_name(variable_name_prefix="joined_view")
-        statements.append((var_name, expression))
-        return statements, var_name
+        out_var_name = var_name_generator.convert_to_variable_name(
+            variable_name_prefix="joined_view", node_name=self.name
+        )
+        statements.append((out_var_name, expression))
+        return statements, out_var_name
 
 
 class TrackChangesNodeParameters(BaseModel):
     """Parameters for TrackChangesNode"""
 
     natural_key_column: InColumnStr
     effective_timestamp_column: InColumnStr
@@ -1210,20 +1250,20 @@
             output_type=NodeOutputType.FRAME,
             output_category=NodeOutputCategory.VIEW,
             row_index_lineage=append_to_lineage(input_operation_info.row_index_lineage, self.name),
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         raise NotImplementedError()
 
 
 class AggregateAsAtParameters(BaseGroupbyParameters, SCDBaseParameters):
     """Parameters for AggregateAsAtNode"""
 
     name: OutColumnStr
@@ -1278,29 +1318,31 @@
                 node_name=node_name,
                 dtype=output_var_type,
             )
         ]
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # Note: this node is a special case as the output of this node is not a complete SDK code.
         # Currently, `scd_view.groupby(...).aggregate_asat()` will generate AggregateAsAtNode + ProjectNode.
         # Output of AggregateAsAtNode is just an expression, the actual variable assignment
         # will be done at the ProjectNode.
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
         statements, var_name = self._convert_expression_to_variable(
-            var_name_expression=input_var_name_expressions[0],
+            var_name_expression=var_name_expressions[0],
             var_name_generator=var_name_generator,
             node_output_type=NodeOutputType.FRAME,
             node_output_category=NodeOutputCategory.VIEW,
+            to_associate_with_node_name=False,
         )
         keys = ValueStr.create(self.parameters.keys)
         category = ValueStr.create(self.parameters.value_by)
         value_column = ValueStr.create(self.parameters.parent)
         method = ValueStr.create(self.parameters.agg_func)
         feature_name = ValueStr.create(self.parameters.name)
         offset = ValueStr.create(self.parameters.offset)
@@ -1328,14 +1370,18 @@
     type: Literal[NodeType.ALIAS] = Field(NodeType.ALIAS, const=True)
     parameters: Parameters
 
     @property
     def max_input_count(self) -> int:
         return 1
 
+    @property
+    def is_inplace_operation_in_sdk_code(self) -> bool:
+        return True
+
     def _get_required_input_columns(
         self, input_index: int, available_column_names: List[str]
     ) -> Sequence[str]:
         return self._assert_empty_required_input_columns()
 
     def _derive_node_operation_info(
         self,
@@ -1372,68 +1418,111 @@
             output_type=self.output_type,
             output_category=output_category,
             row_index_lineage=input_operation_info.row_index_lineage,
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expr = input_var_name_expressions[0]
-        if isinstance(var_name_expr, VariableNameStr):
-            # Always convert into an ExpressionStr to avoid setting name to a temporary feature e.g.
-            # (feat_1 - feat_2).dt.day.name = "new_name"
-            var_name_expr = ExpressionStr(str(var_name_expr))
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        var_name_expr = var_name_expressions[0]
         statements, var_name = self._convert_expression_to_variable(
             var_name_expression=var_name_expr,
             var_name_generator=var_name_generator,
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            to_associate_with_node_name=False,
         )
+        var_statements, output_var_name = self._convert_to_proper_variable_name(
+            var_name=var_name,
+            var_name_generator=var_name_generator,
+            operation_structure=operation_structure,
+            required_copy=context.required_copy,
+            to_associate_with_node_name=True,
+        )
+        statements.extend(var_statements)
         statements.append(
-            (VariableNameStr(f"{var_name}.name"), ValueStr.create(self.parameters.name))
+            (VariableNameStr(f"{output_var_name}.name"), ValueStr.create(self.parameters.name))
         )
-        return statements, var_name
+        return statements, output_var_name
 
 
 class ConditionalNode(BaseSeriesOutputWithAScalarParamNode):
     """ConditionalNode class"""
 
     type: Literal[NodeType.CONDITIONAL] = Field(NodeType.CONDITIONAL, const=True)
 
     @property
     def max_input_count(self) -> int:
         return 3
 
+    @property
+    def is_inplace_operation_in_sdk_code(self) -> bool:
+        return True
+
     def _get_required_input_columns(
         self, input_index: int, available_column_names: List[str]
     ) -> Sequence[str]:
         return self._assert_empty_required_input_columns()
 
     def derive_var_type(self, inputs: List[OperationStructure]) -> DBVarType:
         return inputs[0].series_output_dtype
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
-        var_name_expr = input_var_name_expressions[0]
-        mask_var_name_expr = input_var_name_expressions[1]
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
+        var_name_expressions = self._assert_no_info_dict(node_inputs)
+        var_name_expr = var_name_expressions[0]
+        mask_var_name_expr = var_name_expressions[1]
         statements, var_name = self._convert_expression_to_variable(
             var_name_expression=var_name_expr,
             var_name_generator=var_name_generator,
             node_output_type=operation_structure.output_type,
             node_output_category=operation_structure.output_category,
+            to_associate_with_node_name=False,
+        )
+        mask_statements, mask_var_name = self._convert_expression_to_variable(
+            var_name_expression=mask_var_name_expr,
+            var_name_generator=var_name_generator,
+            node_output_type=NodeOutputType.SERIES,
+            node_output_category=operation_structure.output_category,
+            to_associate_with_node_name=False,
+            variable_name_prefix="mask",
         )
+        statements.extend(mask_statements)
+        # only make the copy if we are not generating info dict
+        # if generating info dict, we will delay the copy to the assign node
+        var_statements, output_var_name = self._convert_to_proper_variable_name(
+            var_name=var_name,
+            var_name_generator=var_name_generator,
+            operation_structure=operation_structure,
+            required_copy=context.required_copy and not context.as_info_dict,
+            to_associate_with_node_name=True,
+        )
+        statements.extend(var_statements)
+
         value: RightHandSide = ValueStr.create(self.parameters.value)
-        if len(input_var_name_expressions) == 3:
-            value = input_var_name_expressions[2]
-        statements.append((VariableNameStr(f"{var_name}[{mask_var_name_expr}]"), value))
-        return statements, var_name
+        if len(var_name_expressions) == 3:
+            value = var_name_expressions[2]
+
+        if context.as_info_dict:
+            # This is to handle the case where `View[<column>][<condition>] = <value>` is used.
+            # Since there is no single line in SDK code to generate conditional expression, we output info instead
+            # and delay the generation of SDK code to the assign node. This method only generates the conditional part,
+            # the assignment part will be generated in the assign node.
+            info_dict = InfoDict({"value": self.parameters.value, "mask": mask_var_name})
+            return statements, info_dict
+
+        # This handles the normal series assignment case where `col[<condition>] = <value>` is used. In this case,
+        # the conditional assignment should not update their parent view.
+        statements.append((VariableNameStr(f"{output_var_name}[{mask_var_name}]"), value))
+        return statements, output_var_name
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/input.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,20 @@
     OperationStructureBranchState,
     OperationStructureInfo,
     SourceDataColumn,
 )
 from featurebyte.query_graph.node.metadata.sdk_code import (
     ClassEnum,
     CodeGenerationConfig,
+    CodeGenerationContext,
     CommentStr,
     ObjectClass,
     StatementT,
     VariableNameGenerator,
-    VarNameExpressionStr,
+    VarNameExpressionInfo,
 )
 from featurebyte.query_graph.node.schema import ColumnSpec, FeatureStoreDetails, TableDetails
 
 
 class BaseInputNodeParameters(BaseModel):
     """BaseInputNodeParameters"""
 
@@ -398,27 +399,27 @@
             output_type=NodeOutputType.FRAME,
             output_category=NodeOutputCategory.VIEW,
             row_index_lineage=(self.name,),
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         statements: List[StatementT] = []
         table_type = self.parameters.type
         table_class_enum = self._table_type_to_table_class_enum[table_type]
 
         # construct table sdk statement
         table_var_name = var_name_generator.convert_to_variable_name(
-            variable_name_prefix=self.parameters.variable_name_prefix
+            variable_name_prefix=self.parameters.variable_name_prefix, node_name=self.name
         )
         table_id = self.parameters.id
         table_info = config.table_id_to_info.get(table_id, {}) if table_id else {}
         table_name = table_info.get("name")
         if config.to_use_saved_data and self.parameters.id:
             # to generate `*Data.get_by_id(ObjectId("<table_id>"))` statement
             comment = self.parameters.construct_comment(table_id_to_info=config.table_id_to_info)
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/metadata/column.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/metadata/column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/metadata/operation.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/metadata/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/metadata/sdk_code.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/metadata/sdk_code.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains models used for sdk code extractor.
 """
 from __future__ import annotations
 
 from typing import Any, DefaultDict, Dict, List, Optional, Set, Tuple, Union
 
+import ast
 import json
 import os
 from collections import defaultdict
 from enum import Enum
 
 from black import FileMode, format_str
 from bson import ObjectId
@@ -70,14 +71,20 @@
         Returns
         -------
         str
         """
         return str(self)
 
 
+class InfoDict(dict):  # type: ignore
+    """
+    InfoStr class is used to store the information about SDK code generation from the node to its connected node(s).
+    """
+
+
 class ExpressionStr(str):
     """
     ExpressionStr class is used to represent a combination of operations, variables, or values that will
     produce a result when evaluated, for example: `event_table['quantity'] * event_table['price_per_unit']`.
     """
 
     def as_input(self) -> str:
@@ -101,14 +108,18 @@
 class CommentStr(str):
     """
     CommentStr class is used to represent a comment in the code. The comment will be formatted and
     prepended with `#`.
     """
 
 
+# module import path str pair
+ImportPathPair = Tuple[str, str]
+
+
 class ObjectClass(BaseModel):
     """
     ObjectClass is used as a mock class object which are used to
     - capture the method/function input parameters
     - import objects
     """
 
@@ -157,27 +168,27 @@
                 output.update(cls._extract_import_helper(elem))
         if isinstance(obj, dict):
             for value in obj.values():
                 output.update(cls._extract_import_helper(value))
         return output
 
     @classmethod
-    def _extract_import(cls, obj: ObjectClass) -> Set[Tuple[str, str]]:
+    def _extract_import(cls, obj: ObjectClass) -> Set[ImportPathPair]:
         if obj.module_path is not None:
             assert obj.class_name is not None
             output = {(obj.module_path, obj.class_name)}
         else:
             output = set()
         for pos_arg in obj.positional_args:
             output.update(cls._extract_import_helper(pos_arg))
         for val_arg in obj.keyword_args.values():
             output.update(cls._extract_import_helper(val_arg))
         return output
 
-    def extract_import(self) -> Set[Tuple[str, str]]:
+    def extract_import(self) -> Set[ImportPathPair]:
         """
         Extract set of required (module_path, class_name) tuple for this object
 
         Returns
         -------
         Set[Tuple[str, str]]
         """
@@ -270,14 +281,15 @@
         positional_args=args,
         keyword_args=kwargs,
         callable_name=callable_name,
     )
 
 
 VarNameExpressionStr = Union[VariableNameStr, ExpressionStr]
+VarNameExpressionInfo = Union[VariableNameStr, ExpressionStr, InfoDict]
 RightHandSide = Union[ValueStr, VariableNameStr, ExpressionStr, ObjectClass]
 StatementT = Union[  # pylint: disable=invalid-name
     StatementStr, CommentStr, Tuple[VariableNameStr, RightHandSide]
 ]
 
 
 class CodeGenerationConfig(BaseModel):
@@ -313,37 +325,59 @@
     final_output_name: str = Field(default="output")
 
     # other configurations
     to_use_saved_data: bool = Field(default=False)
     max_expression_length: int = Field(default=40)
 
 
+class CodeGenerationContext(BaseModel):
+    """
+    CodeGenerationContext is used to store the context information during code generation. Code generation context
+    include information that need to be passed to the next code generation step.
+    """
+
+    # Whether to output current node output as info dict or not. This is used to pass the information to the next
+    # code generation step. For example, for the ConditionalNode -> AssignNode structure, ConditionalNode will pass
+    # the mask variable & value to the AssignNode, and AssignNode will use the mask variable & value to generate the
+    # assignment statement.
+    as_info_dict: bool
+    # Whether to copy the variable before generate the following SDK statement. This is used when the node operation
+    # is in-place operation, and the variable is used in the following SDK statement. See AssignNode,
+    # ConditionalNode and AliasNode for example.
+    required_copy: bool
+
+
 class VariableNameGenerator(BaseModel):
     """
     VariableNameGenerator class is used to generate the variable name given the characteristics of the
     value to be stored.
     """
 
     var_name_counter: DefaultDict[str, int] = Field(default_factory=lambda: defaultdict(int))
+    node_name_to_var_name: Dict[str, VariableNameStr] = Field(default_factory=dict)
 
     def generate_variable_name(
         self,
         node_output_type: NodeOutputType,
         node_output_category: NodeOutputCategory,
+        node_name: Optional[str],
     ) -> VariableNameStr:
         """
         Generate a valid variable name (no name collision) based on node output type (series or frame) &
         category (view or feature) characteristic.
 
         Parameters
         ----------
         node_output_type: NodeOutputType
             Node output type (series or frame)
         node_output_category: NodeOutputCategory
             Node output category (view or feature)
+        node_name: Optional[str]
+            If not None, the generated variable name will be associated with the node name. If the node name
+            already exists, its associated variable name will be returned.
 
         Returns
         -------
         VariableNameStr
         """
         if node_output_category == NodeOutputCategory.VIEW:
             if node_output_type == NodeOutputType.FRAME:
@@ -352,34 +386,82 @@
                 pre_variable_name = "col"
         else:
             if node_output_type == NodeOutputType.FRAME:
                 pre_variable_name = "grouped"
             else:
                 pre_variable_name = "feat"
 
-        return self.convert_to_variable_name(variable_name_prefix=pre_variable_name)
+        return self.convert_to_variable_name(
+            variable_name_prefix=pre_variable_name, node_name=node_name
+        )
 
-    def convert_to_variable_name(self, variable_name_prefix: str) -> VariableNameStr:
+    def convert_to_variable_name(
+        self, variable_name_prefix: str, node_name: Optional[str]
+    ) -> VariableNameStr:
         """
         Convert an input variable name into a valid variable name (no name collision).
 
         Parameters
         ----------
         variable_name_prefix: str
             Variable name before name collision check
+        node_name: Optional[str]
+            If not None, the generated variable name will be associated with the node name. If the node name
+            already exists, its associated variable name will be returned.
 
         Returns
         -------
         VariableNameStr
         """
+        if node_name is not None and node_name in self.node_name_to_var_name:
+            return self.node_name_to_var_name[node_name]
+
         count = self.var_name_counter[variable_name_prefix]
         self.var_name_counter[variable_name_prefix] += 1
+        var_name = VariableNameStr(variable_name_prefix)
         if count:
-            return VariableNameStr(f"{variable_name_prefix}_{count}")
-        return VariableNameStr(variable_name_prefix)
+            var_name = VariableNameStr(f"{variable_name_prefix}_{count}")
+
+        if node_name is not None:
+            self.node_name_to_var_name[node_name] = var_name
+        return var_name
+
+
+class UnusedVariableFinder(ast.NodeVisitor):
+    """UnusedVariableFinder class is used to find the unused variables in the generated SDK code."""
+
+    def __init__(self) -> None:
+        self.variables: Set[str] = set()
+        self.used_variables: Set[str] = set()
+
+    def visit_Name(self, node: ast.Name) -> None:  # pylint: disable=invalid-name
+        """
+        Visit the Name node in the ast.
+
+        Parameters
+        ----------
+        node: ast.Name
+            Ast name node
+        """
+        if isinstance(node.ctx, ast.Store):
+            # add variable to set of variables
+            self.variables.add(node.id)
+        elif isinstance(node.ctx, (ast.Load, ast.Del)):
+            # add variable to set of used variables
+            self.used_variables.add(node.id)
+
+    def get_unused_variables(self) -> Set[str]:
+        """
+        Get the unused variables found in the ast.
+
+        Returns
+        -------
+        Set[str]
+        """
+        return self.variables - self.used_variables
 
 
 class CodeGenerator(BaseModel):
     """
     SDKCodeGenerator class is used to generate the SDK codes from a list of import tags and statements.
 
     A statement could be one
@@ -404,41 +486,70 @@
         Parameters
         ----------
         statements: List[Union[Statement, Tuple[VariableNameStr, ExpressionStr]]]
             Statements to be inserted
         """
         self.statements.extend(statements)
 
-    def generate(self, to_format: bool = False) -> str:
-        """
-        Generate code as string using list of stored statements
-
-        Parameters
-        ----------
-        to_format: bool
-            Whether to format the final code
-
-        Returns
-        -------
-        str
-        """
+    def _generate(
+        self, unused_variables: Optional[Set[str]] = None
+    ) -> Tuple[str, Set[ImportPathPair]]:
         # process statements & extract required imports
         statement_lines = []
         import_pairs = set()
         for statement in self.statements:
             if isinstance(statement, tuple):
                 var_name, right_hand_side = statement
+                if unused_variables and var_name in unused_variables:
+                    continue
                 if isinstance(right_hand_side, ObjectClass):
                     import_pairs.update(right_hand_side.extract_import())
                 statement_lines.append(f"{var_name} = {right_hand_side}")
             elif isinstance(statement, CommentStr):
                 statement_lines.append(f"\n# {statement}")
             elif isinstance(statement, str):
                 statement_lines.append(statement)
         statements = "\n".join(statement_lines)
+        return statements, import_pairs
+
+    def generate(
+        self,
+        to_format: bool = False,
+        output_var_name: Optional[str] = None,
+        remove_unused_variables: bool = True,
+    ) -> str:
+        """
+        Generate code as string using list of stored statements
+
+        Parameters
+        ----------
+        to_format: bool
+            Whether to format the final code
+        output_var_name: Optional[str]
+            Output variable name, default to "output"
+        remove_unused_variables: bool
+            Whether to skip removing unused variables
+
+        Returns
+        -------
+        str
+        """
+        # generate statements and extract required imports
+        statements, import_pairs = self._generate()
+
+        if remove_unused_variables:
+            # extract unused variables
+            tree = ast.parse(statements)
+            finder = UnusedVariableFinder()
+            finder.visit(tree)
+            keep_var_names = {output_var_name} if output_var_name else {"output"}
+            unused_variables = finder.get_unused_variables().difference(keep_var_names)
+
+            # regenerate statements by removing unused variables
+            statements, import_pairs = self._generate(unused_variables=unused_variables)
 
         # process imports and generate import statements
         import_statements = []
         for module_path, name in sorted(import_pairs):
             import_statements.append(f"from {module_path} import {name}")
         imports = "\n".join(import_statements)
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/mixin.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/nested.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/nested.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,19 @@
     OperationStructure,
     OperationStructureBranchState,
     OperationStructureInfo,
 )
 from featurebyte.query_graph.node.metadata.sdk_code import (
     ClassEnum,
     CodeGenerationConfig,
+    CodeGenerationContext,
     ObjectClass,
     StatementT,
     VariableNameGenerator,
-    VarNameExpressionStr,
+    VarNameExpressionInfo,
     get_object_class_from_function_call,
 )
 
 
 class ProxyInputNode(BaseNode):
     """Proxy input node used by nested graph"""
 
@@ -93,35 +94,35 @@
     graph: "QueryGraphModel"  # type: ignore[name-defined]
     output_node_name: str
     type: GraphNodeType
 
     @abstractmethod
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         """
         Derive SDK code for the current graph node
 
         Parameters
         ----------
         input_var_name_expressions: List[VarNameExpressionStr]
             Input variables name
-        input_node_types: List[NodeType]
-            Input node types
         var_name_generator: VariableNameGenerator
             Variable name generator
         operation_structure: OperationStructure
             Operation structure of current node
         config: CodeGenerationConfig
             Code generation configuration
+        node_name: str
+            Node name of the current graph node
 
         Returns
         -------
         Tuple[List[StatementT], VarNameExpressionStr]
         """
 
 
@@ -129,20 +130,20 @@
     """GraphNode (type:cleaning) parameters"""
 
     type: Literal[GraphNodeType.CLEANING] = Field(GraphNodeType.CLEANING, const=True)
     metadata: Dict[str, Any] = Field(default_factory=dict)
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         raise RuntimeError("Not implemented")
 
 
 ViewMetadataT = TypeVar("ViewMetadataT", bound="ViewMetadata")
 
 
 class ViewMetadata(BaseModel):
@@ -250,23 +251,23 @@
 class EventViewGraphNodeParameters(BaseViewGraphNodeParameters):
     """GraphNode (type:event_view) parameters"""
 
     type: Literal[GraphNodeType.EVENT_VIEW] = Field(GraphNodeType.EVENT_VIEW, const=True)
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # construct event view sdk statement
         view_var_name = var_name_generator.convert_to_variable_name(
-            variable_name_prefix="event_view"
+            variable_name_prefix="event_view", node_name=node_name
         )
         assert len(input_var_name_expressions) == 1
         table_var_name = input_var_name_expressions[0]
         expression = get_object_class_from_function_call(
             callable_name=f"{table_var_name}.get_view",
             view_mode=ViewMode.MANUAL,
             drop_column_names=self.metadata.drop_column_names,
@@ -291,23 +292,23 @@
     """GraphNode (type:item_view) parameters"""
 
     type: Literal[GraphNodeType.ITEM_VIEW] = Field(GraphNodeType.ITEM_VIEW, const=True)
     metadata: ItemViewMetadata
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # construct item view sdk statement
         view_var_name = var_name_generator.convert_to_variable_name(
-            variable_name_prefix="item_view"
+            variable_name_prefix="item_view", node_name=node_name
         )
         assert len(input_var_name_expressions) == 1
         table_var_name = input_var_name_expressions[0]
         expression = get_object_class_from_function_call(
             callable_name=f"{table_var_name}.get_view",
             event_suffix=self.metadata.event_suffix,
             view_mode=ViewMode.MANUAL,
@@ -342,23 +343,23 @@
 class DimensionViewGraphNodeParameters(BaseViewGraphNodeParameters):
     """GraphNode (type:dimension_view) parameters"""
 
     type: Literal[GraphNodeType.DIMENSION_VIEW] = Field(GraphNodeType.DIMENSION_VIEW, const=True)
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # construct dimension view sdk statement
         view_var_name = var_name_generator.convert_to_variable_name(
-            variable_name_prefix="dimension_view"
+            variable_name_prefix="dimension_view", node_name=node_name
         )
         assert len(input_var_name_expressions) == 1
         table_var_name = input_var_name_expressions[0]
         expression = get_object_class_from_function_call(
             f"{table_var_name}.get_view",
             view_mode=ViewMode.MANUAL,
             drop_column_names=self.metadata.drop_column_names,
@@ -372,22 +373,24 @@
 class SCDViewGraphNodeParameters(BaseViewGraphNodeParameters):
     """GraphNode (type:scd_view) parameters"""
 
     type: Literal[GraphNodeType.SCD_VIEW] = Field(GraphNodeType.SCD_VIEW, const=True)
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # construct scd view sdk statement
-        view_var_name = var_name_generator.convert_to_variable_name(variable_name_prefix="scd_view")
+        view_var_name = var_name_generator.convert_to_variable_name(
+            variable_name_prefix="scd_view", node_name=node_name
+        )
         assert len(input_var_name_expressions) == 1
         table_var_name = input_var_name_expressions[0]
         expression = get_object_class_from_function_call(
             f"{table_var_name}.get_view",
             view_mode=ViewMode.MANUAL,
             drop_column_names=self.metadata.drop_column_names,
             column_cleaning_operations=self.prepare_column_cleaning_operation_code_generation(
@@ -409,23 +412,23 @@
     """GraphNode (type:change_view) parameters"""
 
     type: Literal[GraphNodeType.CHANGE_VIEW] = Field(GraphNodeType.CHANGE_VIEW, const=True)
     metadata: ChangeViewMetadata
 
     def derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        input_var_name_expressions: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        node_name: str,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         # construct change view sdk statement
         view_var_name = var_name_generator.convert_to_variable_name(
-            variable_name_prefix="change_view"
+            variable_name_prefix="change_view", node_name=node_name
         )
 
         feature_job_setting: Optional[ObjectClass] = None
         if self.metadata.default_feature_job_setting:
             feature_job_setting = ClassEnum.FEATURE_JOB_SETTING(
                 **self.metadata.default_feature_job_setting
             )
@@ -553,20 +556,20 @@
         target_node_input_order_pairs: Sequence[Tuple[NodeT, int]],
         input_operation_structures: List[OperationStructure],
     ) -> NodeT:
         raise RuntimeError("BaseGroupNode.prune should not be called!")
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         return self.parameters.derive_sdk_code(
-            input_var_name_expressions=input_var_name_expressions,
-            input_node_types=input_node_types,
+            input_var_name_expressions=node_inputs,
             var_name_generator=var_name_generator,
             operation_structure=operation_structure,
             config=config,
+            node_name=self.name,
         )
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/request.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     OperationStructure,
     OperationStructureBranchState,
     OperationStructureInfo,
 )
 from featurebyte.query_graph.node.metadata.sdk_code import (
     ClassEnum,
     CodeGenerationConfig,
+    CodeGenerationContext,
     StatementT,
     VariableNameGenerator,
-    VarNameExpressionStr,
+    VarNameExpressionInfo,
 )
 
 
 class RequestColumnNode(BaseNode):
     """Request column node used by on-demand features"""
 
     class RequestColumnNodeParameters(BaseModel):
@@ -74,22 +75,22 @@
             output_type=NodeOutputType.SERIES,
             output_category=NodeOutputCategory.FEATURE,
             row_index_lineage=(self.name,),
         )
 
     def _derive_sdk_code(
         self,
-        input_var_name_expressions: List[VarNameExpressionStr],
-        input_node_types: List[NodeType],
+        node_inputs: List[VarNameExpressionInfo],
         var_name_generator: VariableNameGenerator,
         operation_structure: OperationStructure,
         config: CodeGenerationConfig,
-    ) -> Tuple[List[StatementT], VarNameExpressionStr]:
+        context: CodeGenerationContext,
+    ) -> Tuple[List[StatementT], VarNameExpressionInfo]:
         statements: List[StatementT] = []
-        var_name = var_name_generator.convert_to_variable_name("request_col")
+        var_name = var_name_generator.convert_to_variable_name("request_col", node_name=self.name)
         if self.parameters.column_name == SpecialColumnName.POINT_IN_TIME:
             obj = ClassEnum.REQUEST_COLUMN(
                 _method_name="point_in_time",
             )
         else:
             raise NotImplementedError("Currently only POINT_IN_TIME column is supported")
         statements.append((var_name, obj))
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/scalar.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/scalar.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/schema.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,23 @@
 
     is_local_source: ClassVar[bool] = False
 
 
 class SnowflakeDetails(BaseDatabaseDetails):
     """
     Model for details used to connect to a Snowflake data source.
+
+    Examples
+    --------
+    >>> details= fb.SnowflakeDetails(
+    ...   account="<account>",
+    ...   warehouse="snowflake",
+    ...   database="<database_name>",
+    ...   sf_schema="<schema_name>",
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.SnowflakeDetails")
 
     account: StrictStr = Field(
         description="The host account name which can be found using one of the following "
         "formats:\n"
@@ -49,14 +58,26 @@
     filename: StrictStr
     is_local_source: ClassVar[bool] = True
 
 
 class DatabricksDetails(BaseDatabaseDetails):
     """
     Model for details used to connect to a Databricks data source.
+
+    Examples
+    --------
+    >>> details = fb.DatabricksDetails(
+    ...   host="<host_name>",
+    ...   http_path="<http_path>",
+    ...   featurebyte_catalog="hive_metastore",
+    ...   featurebyte_schema="<schema_name>",
+    ...   storage_type=fb.StorageType.S3,
+    ...   storage_url="<url>",
+    ...   storage_spark_url="dbfs:/FileStore/<schema_name>",
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.DatabricksDetails")
 
     host: StrictStr = Field(
         description="Databricks host. This is typically the URL you use to go to to access your databricks environment."
     )
@@ -78,14 +99,26 @@
         "write path, and as such, we require two fields."
     )
 
 
 class SparkDetails(BaseDatabaseDetails):
     """
     Model for details used to connect to a Spark data source.
+
+    Examples
+    --------
+    >>> details = fb.SparkDetails(
+    ...   host="<host>",
+    ...   port=10003,
+    ...   featurebyte_catalog="spark_catalog",
+    ...   featurebyte_schema="<schema_name>",
+    ...   storage_type=fb.StorageType.S3,
+    ...   storage_url="<storage_url>",
+    ...   storage_spark_url="gs://dataproc-cluster-staging/{<schema_name>}"
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.SparkDetails")
 
     host: StrictStr = Field(
         default="127.0.0.1", description="The server where your spark cluster is hosted."
     )
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/string.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/unary.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/node/validator.py` & `featurebyte-0.3.0/featurebyte/query_graph/node/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/pruning_util.py` & `featurebyte-0.3.0/featurebyte/query_graph/pruning_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/adapter.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,14 +457,30 @@
             select_expr = (
                 select(*[quoted_identifier(column_name) for column_name in column_names])
                 .from_(select_expr.subquery())
                 .where(quoted_identifier(FB_QUALIFY_CONDITION_COLUMN))
             )
         return select_expr
 
+    @classmethod
+    def any_value(cls, expr: Expression) -> Expression:
+        """
+        Expression for the aggregation function that returns any value in a group
+
+        Parameters
+        ----------
+        expr : Expression
+            Expression to be aggregated
+
+        Returns
+        -------
+        Expression
+        """
+        return expressions.Anonymous(this="ANY_VALUE", expressions=[expr])
+
 
 class SnowflakeAdapter(BaseAdapter):
     """
     Helper class to generate Snowflake specific SQL expressions
     """
 
     # Snowflake does not support the PERCENT keyword. Setting the size parameter instead to
@@ -773,14 +789,18 @@
         return expressions.Create(
             this=expressions.Table(this=destination_expr),
             kind="TABLE",
             expression=select_expr,
             properties=expressions.Properties(expressions=table_properties),
         )
 
+    @classmethod
+    def any_value(cls, expr: Expression) -> Expression:
+        return expressions.Anonymous(this="first", expressions=[expr])
+
 
 class SparkAdapter(DatabricksAdapter):
     """
     Helper class to generate Spark specific SQL expressions
 
     Spark is the OSS version of Databricks, so it shares most of the same SQL syntax.
     """
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/asat.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/asat.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 SQL generation for as-at aggregation
 """
 from __future__ import annotations
 
 from typing import Any, cast
 
 from sqlglot import expressions
-from sqlglot.expressions import Select, alias_, select
+from sqlglot.expressions import Select, select
 
 from featurebyte.enum import SpecialColumnName
 from featurebyte.query_graph.sql.aggregator.base import (
     AggregationResult,
     LeftJoinableSubquery,
     NonTileBasedAggregator,
 )
 from featurebyte.query_graph.sql.aggregator.request_table import RequestTablePlan
 from featurebyte.query_graph.sql.common import (
     CteStatements,
     get_qualified_column_identifier,
     quoted_identifier,
 )
-from featurebyte.query_graph.sql.groupby_helper import get_aggregation_expression
+from featurebyte.query_graph.sql.groupby_helper import GroupbyColumn, GroupbyKey, get_groupby_expr
 from featurebyte.query_graph.sql.scd_helper import END_TS, augment_scd_table_with_end_timestamp
 from featurebyte.query_graph.sql.specs import AggregateAsAtSpec
 
 
 class AsAtAggregator(NonTileBasedAggregator[AggregateAsAtSpec]):
     """
     AsAtAggregation is responsible for generating SQL for as at aggregation
@@ -124,50 +124,67 @@
                     this=get_qualified_column_identifier(end_timestamp_column, "SCD"),
                     expression=expressions.Null(),
                 ),
             ),
         )
         join_condition = expressions.and_(join_key_condition, record_validity_condition)
 
-        groupby_keys = [get_qualified_column_identifier(SpecialColumnName.POINT_IN_TIME, "REQ")] + [
-            get_qualified_column_identifier(serving_name, "REQ")
+        groupby_keys = [
+            GroupbyKey(
+                expr=get_qualified_column_identifier(SpecialColumnName.POINT_IN_TIME, "REQ"),
+                name=SpecialColumnName.POINT_IN_TIME,
+            )
+        ] + [
+            GroupbyKey(
+                expr=get_qualified_column_identifier(serving_name, "REQ"),
+                name=serving_name,
+            )
             for serving_name in spec.serving_names
         ]
-        agg_exprs = [
-            alias_(
-                get_aggregation_expression(
-                    agg_func=s.parameters.agg_func,
-                    input_column=(
-                        get_qualified_column_identifier(s.parameters.parent, "SCD")
-                        if s.parameters.parent
-                        else None
-                    ),
+        value_by = (
+            GroupbyKey(
+                expr=get_qualified_column_identifier(spec.parameters.value_by, "SCD"),
+                name=spec.parameters.value_by,
+            )
+            if spec.parameters.value_by
+            else None
+        )
+        groupby_columns = [
+            GroupbyColumn(
+                agg_func=s.parameters.agg_func,
+                parent_expr=(
+                    get_qualified_column_identifier(s.parameters.parent, "SCD")
+                    if s.parameters.parent
+                    else None
                 ),
-                alias=s.agg_result_name,
-                quoted=True,
+                result_name=s.agg_result_name,
             )
             for s in specs
         ]
-        request_table_name = self.request_table_plan.get_request_table_name(spec)
-        aggregate_asat_expr = (
-            select(*groupby_keys, *agg_exprs)
+        groupby_input_expr = (
+            select()
             .from_(
                 expressions.Table(
-                    this=quoted_identifier(request_table_name),
+                    this=quoted_identifier(self.request_table_plan.get_request_table_name(spec)),
                     alias="REQ",
                 )
             )
             .join(
                 scd_expr.subquery(alias="SCD"),
                 join_type="inner",
                 on=join_condition,
             )
-            .group_by(*groupby_keys)
         )
-
+        aggregate_asat_expr = get_groupby_expr(
+            input_expr=groupby_input_expr,
+            groupby_keys=groupby_keys,
+            groupby_columns=groupby_columns,
+            value_by=value_by,
+            adapter=self.adapter,
+        )
         return LeftJoinableSubquery(
             expr=aggregate_asat_expr,
             column_names=[s.agg_result_name for s in specs],
             join_keys=[SpecialColumnName.POINT_IN_TIME.value] + spec.serving_names,
         )
 
     def get_common_table_expressions(self, request_table_name: str) -> CteStatements:
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/base.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/item.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/item.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/latest.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/latest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/lookup.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/lookup.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/request_table.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/window.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/window.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/aggregate.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/aggregate.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/base.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/binary.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/count_dict.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/datetime.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/generic.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/groupby.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/groupby.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/input.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/is_in.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/is_in.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join_feature.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join_feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/literal.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/literal.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/request.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/string.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/tile.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/tile.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from __future__ import annotations
 
 from typing import cast
 
 from dataclasses import dataclass
 
-from sqlglot import expressions, parse_one
+from sqlglot import expressions
 from sqlglot.expressions import Expression, Select, alias_, select
 
 from featurebyte.enum import DBVarType, InternalName
 from featurebyte.query_graph.enum import NodeType
 from featurebyte.query_graph.sql.ast.base import SQLNodeContext, TableNode
 from featurebyte.query_graph.sql.ast.literal import make_literal_value
 from featurebyte.query_graph.sql.common import (
@@ -21,58 +21,62 @@
 )
 from featurebyte.query_graph.sql.specs import TileBasedAggregationSpec
 from featurebyte.query_graph.sql.tiling import InputColumn, TileSpec, get_aggregator
 from featurebyte.query_graph.transform.operation_structure import OperationStructureExtractor
 
 
 @dataclass
-class BuildTileNode(TableNode):
+class BuildTileNode(TableNode):  # pylint: disable=too-many-instance-attributes
     """Tile builder node
 
     This node is responsible for generating the tile building SQL for a groupby operation.
     """
 
     input_node: TableNode
     keys: list[str]
     value_by: str | None
     tile_specs: list[TileSpec]
     timestamp: str
-    frequency: int
+    frequency_minute: int
+    blind_spot: int
+    time_modulo_frequency: int
+
     is_on_demand: bool
     is_order_dependent: bool
     query_node_type = NodeType.GROUPBY
 
     # Internal names
     ROW_NUMBER = "__FB_ROW_NUMBER"
 
     @property
     def sql(self) -> Expression:
-        start_date_expr = InternalName.TILE_START_DATE_SQL_PLACEHOLDER
-        start_date_epoch = self.context.adapter.to_epoch_seconds(
-            cast(Expression, parse_one(f"CAST({start_date_expr} AS TIMESTAMP)"))
-        ).sql()
-        timestamp_epoch = self.context.adapter.to_epoch_seconds(
-            quoted_identifier(self.timestamp)
-        ).sql()
-
         input_filtered = self._get_input_filtered_within_date_range()
-        input_tiled = select(
-            "*",
-            f"FLOOR(({timestamp_epoch} - {start_date_epoch}) / {self.frequency}) AS tile_index",
-        ).from_(input_filtered.subquery())
-
-        tile_start_date = f"TO_TIMESTAMP({start_date_epoch} + tile_index * {self.frequency})"
+        tile_index_expr = alias_(
+            expressions.Anonymous(
+                this="F_TIMESTAMP_TO_INDEX",
+                expressions=[
+                    self.context.adapter.convert_to_utc_timestamp(
+                        quoted_identifier(self.timestamp)
+                    ),
+                    make_literal_value(self.time_modulo_frequency),
+                    make_literal_value(self.blind_spot),
+                    make_literal_value(self.frequency_minute),
+                ],
+            ),
+            alias="index",
+        )
+        input_tiled = select("*", tile_index_expr).from_(input_filtered.subquery())
         keys = [quoted_identifier(k) for k in self.keys]
         if self.value_by is not None:
             keys.append(quoted_identifier(self.value_by))
 
         if self.is_order_dependent:
-            return self._get_tile_sql_order_dependent(keys, tile_start_date, input_tiled)
+            return self._get_tile_sql_order_dependent(keys, input_tiled)
 
-        return self._get_tile_sql_order_independent(keys, tile_start_date, input_tiled)
+        return self._get_tile_sql_order_independent(keys, input_tiled)
 
     def _get_input_filtered_within_date_range(self) -> Select:
         """
         Construct sql to filter input data to be within a date range. Only data within this range
         will be used to calculate tiles.
 
         Returns
@@ -106,35 +110,38 @@
         Construct sql to filter the data used when building tiles for selected entities only
 
         The selected entities are expected to be available in an "entity table". It can be injected
         as a subquery by replacing the placeholder InternalName.ENTITY_TABLE_SQL_PLACEHOLDER.
 
         Entity table is expected to have these columns:
         * entity column(s)
+        * InternalName.ENTITY_TABLE_START_DATE
         * InternalName.ENTITY_TABLE_END_DATE
 
         Returns
         -------
         Select
         """
         entity_table = InternalName.ENTITY_TABLE_NAME.value
-        start_date = InternalName.TILE_START_DATE_SQL_PLACEHOLDER
+        start_date = InternalName.ENTITY_TABLE_START_DATE.value
         end_date = InternalName.ENTITY_TABLE_END_DATE.value
 
         join_conditions: list[Expression] = []
         for col in self.keys:
             condition = expressions.EQ(
                 this=get_qualified_column_identifier(col, "R"),
                 expression=get_qualified_column_identifier(col, entity_table),
             )
             join_conditions.append(condition)
         join_conditions.append(
             expressions.GTE(
                 this=get_qualified_column_identifier(self.timestamp, "R"),
-                expression=expressions.Identifier(this=start_date),
+                expression=get_qualified_column_identifier(
+                    start_date, entity_table, quote_column=False
+                ),
             )
         )
         join_conditions.append(
             expressions.LT(
                 this=get_qualified_column_identifier(self.timestamp, "R"),
                 expression=get_qualified_column_identifier(
                     end_date, entity_table, quote_column=False
@@ -156,66 +163,64 @@
             )
         )
         return cast(Select, select_expr)
 
     def _get_tile_sql_order_independent(
         self,
         keys: list[Expression],
-        tile_start_date: str,
         input_tiled: expressions.Select,
     ) -> Expression:
         groupby_sql = (
             select(
-                f"{tile_start_date} AS {InternalName.TILE_START_DATE}",
+                "index",
                 *keys,
                 *[alias_(spec.tile_expr, alias=spec.tile_column_name) for spec in self.tile_specs],
             )
             .from_(input_tiled.subquery())
-            .group_by("tile_index", *keys)
+            .group_by("index", *keys)
         )
         return groupby_sql
 
     def _get_tile_sql_order_dependent(
         self,
         keys: list[Expression],
-        tile_start_date: str,
         input_tiled: expressions.Select,
     ) -> Expression:
         def _make_window_expr(expr: str | Expression) -> Expression:
             order = expressions.Order(
                 expressions=[
                     expressions.Ordered(this=quoted_identifier(self.timestamp), desc=True),
                 ]
             )
-            partition_by = [cast(Expression, expressions.Identifier(this="tile_index"))] + keys
+            partition_by = [cast(Expression, expressions.Identifier(this="index"))] + keys
             window_expr = expressions.Window(this=expr, partition_by=partition_by, order=order)
             return window_expr
 
         window_exprs = [
             alias_(
                 _make_window_expr(expressions.Anonymous(this="ROW_NUMBER")), alias=self.ROW_NUMBER
             ),
             *[
                 alias_(_make_window_expr(spec.tile_expr), alias=spec.tile_column_name)
                 for spec in self.tile_specs
             ],
         ]
         inner_expr = select(
-            alias_(tile_start_date, alias=InternalName.TILE_START_DATE, quoted=False),
+            "index",
             *keys,
             *window_exprs,
         ).from_(input_tiled.subquery())
 
         outer_condition = expressions.EQ(
             this=quoted_identifier(self.ROW_NUMBER),
             expression=make_literal_value(1),
         )
         tile_expr = (
             select(
-                InternalName.TILE_START_DATE,
+                "index",
                 *keys,
                 *[spec.tile_column_name for spec in self.tile_specs],
             )
             .from_(inner_expr.subquery())
             .where(outer_condition)
         )
 
@@ -274,15 +279,17 @@
             context=context,
             columns_map=columns_map,
             input_node=input_node,
             keys=parameters["keys"],
             value_by=parameters["value_by"],
             tile_specs=tile_specs,
             timestamp=parameters["timestamp"],
-            frequency=parameters["frequency"],
+            frequency_minute=parameters["frequency"] // 60,
+            blind_spot=parameters["blind_spot"],
+            time_modulo_frequency=parameters["time_modulo_frequency"],
             is_on_demand=is_on_demand,
             is_order_dependent=aggregator.is_order_dependent,
         )
         return sql_node
 
 
 @dataclass
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/track_changes.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/track_changes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/unary.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/util.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/builder.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/common.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/dataframe.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/expression.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/expression.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/feature_compute.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/feature_compute.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module with logic related to feature SQL generation
 """
 from __future__ import annotations
 
-from typing import Iterable, Optional, Type, Union
+from typing import Iterable, Optional, Sequence, Type, Union
 
 from bson import ObjectId
 from sqlglot import expressions
 from sqlglot.expressions import select
 
 from featurebyte.enum import SourceType
 from featurebyte.models.parent_serving import ParentServingPreparation
@@ -42,14 +42,15 @@
     TileBasedAggregationSpec,
 )
 from featurebyte.query_graph.transform.flattening import GraphFlatteningTransformer
 
 AggregatorType = Union[
     LatestAggregator, LookupAggregator, WindowAggregator, ItemAggregator, AsAtAggregator
 ]
+AggregationSpecType = Union[TileBasedAggregationSpec, NonTileBasedAggregationSpec]
 
 
 class FeatureExecutionPlan:
     """Responsible for constructing the SQL to compute features by aggregating tiles"""
 
     AGGREGATION_TABLE_NAME = "_FB_AGGREGATED"
 
@@ -94,14 +95,24 @@
         set[ObjectId]
         """
         out = set()
         for aggregator in self.iter_aggregators():
             out.update(aggregator.get_required_entity_ids())
         return out
 
+    @property
+    def feature_names(self) -> list[str]:
+        """Returns the list of feature names
+
+        Returns
+        -------
+        list[str]
+        """
+        return list(self.feature_specs.keys())
+
     def iter_aggregators(self) -> Iterable[AggregatorType]:
         """Iterate over all the aggregators
 
         Yields
         ------
         BaseAggregator
             Instance of an aggregator
@@ -412,102 +423,99 @@
         """Update plan state for a given query graph Node
 
         Parameters
         ----------
         node : Node
             Query graph node
         """
+        agg_specs = self.get_aggregation_specs(node)
+        for agg_spec in agg_specs:
+            self.plan.add_aggregation_spec(agg_spec)
+        self.update_feature_specs(node)
+
+    def get_aggregation_specs(self, node: Node) -> list[AggregationSpecType]:
+        """Get list of aggregation specs for a given query graph node
+
+        Parameters
+        ----------
+        node : Node
+            Query graph node
+
+        Returns
+        -------
+        AggregationSpec
+        """
         groupby_nodes = list(self.graph.iterate_nodes(node, NodeType.GROUPBY))
         item_groupby_nodes = list(self.graph.iterate_nodes(node, NodeType.ITEM_GROUPBY))
         lookup_nodes = list(self.graph.iterate_nodes(node, NodeType.LOOKUP))
         asat_nodes = list(self.graph.iterate_nodes(node, NodeType.AGGREGATE_AS_AT))
+
+        out: list[AggregationSpecType] = []
         if groupby_nodes:
             # Feature involves window aggregations. In this case, tiling applies. Even if
             # ITEM_GROUPBY nodes are involved, their results would have already been incorporated in
             # tiles, so we only need to handle GROUPBY node type here.
             for groupby_node in groupby_nodes:
-                self.parse_and_update_specs_from_groupby(groupby_node)
+                out.extend(self.get_specs_from_groupby(groupby_node))
+
         elif item_groupby_nodes:
             # Feature involves non-time-aware aggregations
             for item_groupby_node in item_groupby_nodes:
-                self.parse_and_update_specs_from_item_groupby(item_groupby_node)
+                out.extend(self.get_non_tiling_specs(ItemAggregationSpec, item_groupby_node))
+
         if lookup_nodes:
             for lookup_node in lookup_nodes:
-                self.parse_and_update_specs_from_lookup(lookup_node)
+                out.extend(self.get_non_tiling_specs(LookupSpec, lookup_node))
+
         if asat_nodes:
             for asat_node in asat_nodes:
-                self.parse_and_update_specs_from_asat(asat_node)
-        self.update_feature_specs(node)
+                out.extend(self.get_non_tiling_specs(AggregateAsAtSpec, asat_node))
+
+        return out
 
-    def parse_and_update_specs_from_groupby(self, groupby_node: Node) -> None:
+    def get_specs_from_groupby(self, groupby_node: Node) -> Sequence[TileBasedAggregationSpec]:
         """Update FeatureExecutionPlan with a groupby query node
 
         Parameters
         ----------
         groupby_node : Node
             Groupby query node
+
+        Returns
+        -------
+        list[AggregationSpec]
         """
-        agg_specs = TileBasedAggregationSpec.from_groupby_query_node(
+        return TileBasedAggregationSpec.from_groupby_query_node(
             groupby_node, self.adapter, serving_names_mapping=self.serving_names_mapping
         )
-        for agg_spec in agg_specs:
-            self.plan.add_aggregation_spec(agg_spec)
 
-    def parse_and_update_specs_from_item_groupby(self, node: Node) -> None:
-        """Update FeatureExecutionPlan with an item groupby query node
-
-        Parameters
-        ----------
-        node : Node
-            Query graph node
-        """
-        self.get_non_tiling_specs_and_update_plan(ItemAggregationSpec, node)
-
-    def parse_and_update_specs_from_lookup(self, node: Node) -> None:
-        """Update FeatureExecutionPlan with a lookup query node
-
-        Parameters
-        ----------
-        node : Node
-            Query graph node
-        """
-        self.get_non_tiling_specs_and_update_plan(LookupSpec, node)
-
-    def parse_and_update_specs_from_asat(self, node: Node) -> None:
-        """Update FeatureExecutionPlan with a AggregateAsAt node
-
-        Parameters
-        ----------
-        node : Node
-            Query graph node
-        """
-        self.get_non_tiling_specs_and_update_plan(AggregateAsAtSpec, node)
-
-    def get_non_tiling_specs_and_update_plan(
+    def get_non_tiling_specs(
         self, spec_cls: Type[NonTileBasedAggregationSpec], node: Node
-    ) -> None:
+    ) -> Sequence[NonTileBasedAggregationSpec]:
         """
         Update FeatureExecutionPlan with a node that produces NonTileBasedAggregationSpec
 
         Parameters
         ----------
         node: Node
             Query graph node
         spec_cls: Type[NonTileBasedAggregationSpec]
             Aggregation specification class
+
+        Returns
+        -------
+        list[AggregationSpec]
         """
-        agg_specs = spec_cls.from_query_graph_node(
+        return spec_cls.from_query_graph_node(
             node,
             graph=self.graph,
             source_type=self.source_type,
             serving_names_mapping=self.serving_names_mapping,
             is_online_serving=self.is_online_serving,
         )
-        for agg_spec in agg_specs:
-            self.plan.add_aggregation_spec(agg_spec)
 
     def update_feature_specs(self, node: Node) -> None:
         """Update FeatureExecutionPlan with a query graph node
 
         Parameters
         ----------
         node : Node
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/feature_historical.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/scd_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,448 +1,477 @@
 """
-Historical features SQL generation
+Utilities for SCD join / lookup
 """
 from __future__ import annotations
 
-from typing import AsyncGenerator, Callable, List, Optional, Union, cast
+from typing import Literal, Optional, cast
 
-import datetime
-import time
-from abc import ABC, abstractmethod
+from dataclasses import dataclass
 
 import pandas as pd
-from pandas.api.types import is_datetime64_any_dtype
-from sqlglot import expressions
+from sqlglot import expressions, parse_one
+from sqlglot.expressions import Expression, Select, alias_, select
 
-from featurebyte.enum import SourceType, SpecialColumnName
-from featurebyte.exception import MissingPointInTimeColumnError, TooRecentPointInTimeError
-from featurebyte.logging import get_logger
-from featurebyte.models.observation_table import ObservationTableModel
-from featurebyte.models.parent_serving import ParentServingPreparation
-from featurebyte.query_graph.graph import QueryGraph
-from featurebyte.query_graph.node import Node
-from featurebyte.query_graph.node.schema import TableDetails
-from featurebyte.query_graph.sql.adapter import get_sql_adapter
-from featurebyte.query_graph.sql.common import (
-    REQUEST_TABLE_NAME,
-    get_fully_qualified_table_name,
-    sql_to_string,
-)
-from featurebyte.query_graph.sql.feature_compute import FeatureExecutionPlanner
-from featurebyte.query_graph.sql.parent_serving import construct_request_table_with_parent_entities
-from featurebyte.session.base import BaseSession
-from featurebyte.tile.manager import TILE_COMPUTE_PROGRESS_MAX_PERCENT
-from featurebyte.tile.tile_cache import TileCache
-
-HISTORICAL_REQUESTS_POINT_IN_TIME_RECENCY_HOUR = 48
-
-
-logger = get_logger(__name__)
-
-
-class ObservationSet(ABC):
-    """
-    Observation set abstraction for historical features (used internally in this module)
-    """
+from featurebyte.query_graph.sql.adapter import BaseAdapter
+from featurebyte.query_graph.sql.ast.literal import make_literal_value
+from featurebyte.query_graph.sql.common import get_qualified_column_identifier, quoted_identifier
+
+# Internally used identifiers when constructing SQL
+TS_COL = "__FB_TS_COL"
+EFFECTIVE_TS_COL = "__FB_EFFECTIVE_TS_COL"
+KEY_COL = "__FB_KEY_COL"
+LAST_TS = "__FB_LAST_TS"
+END_TS = "__FB_END_TS"
+
+# Special column name and values used to handle ties in timestamps between main table and SCD table
+TS_TIE_BREAKER_COL = "__FB_TS_TIE_BREAKER_COL"
+TS_TIE_BREAKER_VALUE_SCD_TABLE = 1
+TS_TIE_BREAKER_VALUE_ALLOW_EXACT_MATCH = 2
+TS_TIE_BREAKER_VALUE_DISALLOW_EXACT_MATCH = 0
+
+
+@dataclass
+class Table:
+    """
+    Representation of a table to be used in SCD join
+    """
+
+    expr: str | Select
+    timestamp_column: str | Expression
+    join_keys: list[str]
+    input_columns: list[str]
+    output_columns: list[str]
 
     @property
-    @abstractmethod
-    def columns(self) -> list[str]:
+    def timestamp_column_expr(self) -> Expression:
         """
-        List of columns available in the observation set
+        Returns an expression for the timestamp column (return as is if it's already an expression,
+        else return the quoted column name)
 
         Returns
         -------
-        list[str]
-        """
-
-    @property
-    @abstractmethod
-    def most_recent_point_in_time(self) -> pd.Timestamp:
-        """
-        The most recent point in time in the observation set
+        Expression
         """
+        if isinstance(self.timestamp_column, str):
+            return quoted_identifier(self.timestamp_column)
+        return self.timestamp_column
 
-    @abstractmethod
-    async def register_as_request_table(
-        self, session: BaseSession, request_table_name: str
-    ) -> None:
+    def as_subquery(self, alias: Optional[str] = None) -> Expression:
         """
-        Register the observation set as the request table in the session
+        Returns an expression that can be selected from (converted to subquery if required)
 
         Parameters
         ----------
-        session : BaseSession
-            Session
-        request_table_name : str
-            Request table name
-        """
-
-
-class DataFrameObservationSet(ObservationSet):
-    """
-    Observation set based on an in memory pandas DataFrame
-    """
-
-    def __init__(self, dataframe: pd.DataFrame):
-        self.dataframe = convert_point_in_time_dtype_if_needed(dataframe)
-
-    @property
-    def columns(self) -> List[str]:
-        return cast(List[str], self.dataframe.columns.tolist())
-
-    @property
-    def most_recent_point_in_time(self) -> pd.Timestamp:
-        return self.dataframe[SpecialColumnName.POINT_IN_TIME].max()
+        alias: Optional[str]
+            Table alias, if specified.
 
-    async def register_as_request_table(
-        self, session: BaseSession, request_table_name: str
-    ) -> None:
-        await session.register_table(request_table_name, self.dataframe)
+        Returns
+        -------
+        Expression
+        """
+        if isinstance(self.expr, str):
+            return expressions.Table(this=expressions.Identifier(this=self.expr), alias=alias)
+        assert isinstance(self.expr, Select)
+        return cast(Expression, self.expr.subquery(alias=alias))
+
+
+def get_scd_join_expr(
+    left_table: Table,
+    right_table: Table,
+    join_type: Literal["inner", "left"],
+    adapter: BaseAdapter,
+    select_expr: Optional[Select] = None,
+    offset: Optional[str] = None,
+    allow_exact_match: bool = True,
+    quote_right_input_columns: bool = True,
+    convert_timestamps_to_utc: bool = True,
+) -> Select:
+    """
+    Construct a query to perform SCD join
+
+    The general idea is to first merge the left timestamps (event timestamps) and right
+    timestamps (SCD record effective timestamps) along with join keys into a temporary table.
+    Then apply a LAG window function on this temporary table to retrieve the latest effective
+    timestamp corresponding to each event timestamp in one go.
 
+    Parameters
+    ----------
+    left_table: Table
+        Left table
+    right_table: Table
+        Right table, usually the SCD table
+    join_type: Literal["inner", "left"]
+        Join type
+    adapter: BaseAdapter
+        Instance of BaseAdapter for engine specific sql generation
+    select_expr: Optional[Select]
+        Partially constructed select expression, if any
+    offset: Optional[str]
+        Offset to apply when performing SCD join
+    allow_exact_match: bool
+        Whether to allow exact matching effective timestamps to be joined
+    quote_right_input_columns: bool
+        Whether to quote right table's input columns. Temporary and should be removed after
+        https://featurebyte.atlassian.net/browse/DEV-935
+    convert_timestamps_to_utc: bool
+        Whether timestamps should be converted to UTC for joins
 
-class MaterializedTableObservationSet(ObservationSet):
-    """
-    Observation set based on a materialized table in data warehouse
+    Returns
+    -------
+    Select
     """
+    if select_expr is None:
+        select_expr = select(
+            *[
+                alias_(
+                    get_qualified_column_identifier(input_col, "L"), alias=output_col, quoted=True
+                )
+                for input_col, output_col in zip(
+                    left_table.input_columns, left_table.output_columns
+                )
+            ],
+            *[
+                alias_(
+                    get_qualified_column_identifier(
+                        input_col, "R", quote_column=quote_right_input_columns
+                    ),
+                    alias=output_col,
+                    quoted=True,
+                )
+                for input_col, output_col in zip(
+                    right_table.input_columns, right_table.output_columns
+                )
+            ],
+        )
 
-    def __init__(self, observation_table: ObservationTableModel):
-        self.observation_table = observation_table
-
-    @property
-    def columns(self) -> list[str]:
-        return [col.name for col in self.observation_table.columns_info]
-
-    @property
-    def most_recent_point_in_time(self) -> pd.Timestamp:
-        return pd.to_datetime(self.observation_table.most_recent_point_in_time)
+    left_view_with_last_ts_expr = augment_table_with_effective_timestamp(
+        left_table=left_table,
+        right_table=right_table,
+        adapter=adapter,
+        offset=offset,
+        allow_exact_match=allow_exact_match,
+        convert_timestamps_to_utc=convert_timestamps_to_utc,
+    )
 
-    async def register_as_request_table(
-        self, session: BaseSession, request_table_name: str
-    ) -> None:
-        query = sql_to_string(
-            expressions.select("*").from_(
-                get_fully_qualified_table_name(self.observation_table.location.table_details.dict())
-            ),
-            source_type=session.source_type,
-        )
-        await session.register_table_with_query(request_table_name, query)
+    left_subquery = left_view_with_last_ts_expr.subquery(alias="L")
+    right_subquery = right_table.as_subquery(alias="R")
+    assert isinstance(right_table.timestamp_column, str)
+    join_conditions = [
+        expressions.EQ(
+            this=get_qualified_column_identifier(LAST_TS, "L"),
+            expression=get_qualified_column_identifier(right_table.timestamp_column, "R"),
+        ),
+    ] + _key_cols_equality_conditions(right_table.join_keys)
+
+    select_expr = select_expr.from_(left_subquery).join(
+        right_subquery,
+        join_type=join_type,
+        on=expressions.and_(*join_conditions),
+    )
+    return select_expr
 
 
-def get_internal_observation_set(
-    observation_set: pd.DataFrame | ObservationTableModel,
-) -> ObservationSet:
+def _convert_to_utc_ntz(
+    col_expr: expressions.Expression, adapter: BaseAdapter
+) -> expressions.Expression:
     """
-    Get the internal observation set representation
+    Convert timestamp expression to UTC values and NTZ timestamps
 
     Parameters
     ----------
-    observation_set : pd.DataFrame | ObservationTableModel
-        Observation set
+    col_expr: expressions.Expression
+        Timestamp expression to convert
+    adapter: BaseAdapter
+        Instance of BaseAdapter for engine specific sql generation
 
     Returns
     -------
-    ObservationSet
+    expressions.Expression
     """
-    if isinstance(observation_set, pd.DataFrame):
-        return DataFrameObservationSet(observation_set)
-    return MaterializedTableObservationSet(observation_set)
+    utc_ts_expr = adapter.convert_to_utc_timestamp(col_expr)
+    return expressions.Cast(this=utc_ts_expr, to=parse_one("TIMESTAMP"))
 
 
-def convert_point_in_time_dtype_if_needed(observation_set: pd.DataFrame) -> pd.DataFrame:
-    """
-    Check dtype of the point in time column and convert if necessary. The converted DataFrame will
-    later be used to create a temp table in the session.
+def augment_table_with_effective_timestamp(
+    left_table: Table,
+    right_table: Table,
+    adapter: BaseAdapter,
+    offset: Optional[str],
+    allow_exact_match: bool = True,
+    convert_timestamps_to_utc: bool = True,
+) -> Select:
+    """
+    This constructs a query that calculates the corresponding SCD effective date for each row in the
+    left table. See an example below.
+
+    Left table:
+
+    ------------------------------
+    EVENT_TS      CUST_ID    ....
+    ------------------------------
+    2022-04-10    1000
+    2022-04-15    1000
+    2022-04-20    1000
+    ------------------------------
+
+    Right table:
+
+    -------------------------------
+    SCD_TS          CUST_ID    ....
+    -------------------------------
+    2022-04-12      1000
+    2022-04-20      1000
+    -------------------------------
+
+    Merged temporary table with LAG function applied with IGNORE NULLS option:
+
+    --------------------------------------------------------------------------
+    TS            KEY     EFFECTIVE_TS    LAST_TS       ROW_OF_INTEREST    ...
+    --------------------------------------------------------------------------
+    2022-04-10    1000    NULL            NULL          *
+    2022-04-12    1000    2022-04-12      NULL
+    2022-04-15    1000    NULL            2022-04-12    *
+    2022-04-20    1000    2022-04-20      2022-04-12
+    2022-04-20    1000    NULL            2022-04-20    *
+    --------------------------------------------------------------------------
+
+    This query extracts the above table and keeps only the rows of interest (rows that are from
+    the left table). The resulting table has the same number of rows as the original left
+    table, and contains the columns specified in left_input_columns renamed as
+    left_output_columns.
 
     Parameters
     ----------
-    observation_set : pd.DataFrame
-        Observation set
+    left_table: Table
+        Left table
+    right_table: Table
+        Right table, usually the SCD table
+    adapter: BaseAdapter
+        Instance of BaseAdapter for engine specific sql generation
+    offset: Optional[str]
+        Offset to apply when performing SCD join
+    allow_exact_match: bool
+        Whether to allow exact matching effective timestamps to be joined
+    convert_timestamps_to_utc: bool
+        Whether timestamps should be converted to UTC for joins
 
     Returns
     -------
-    pd.DataFrame
+    Select
     """
-    if SpecialColumnName.POINT_IN_TIME not in observation_set.columns:
-        return observation_set
-
-    if not is_datetime64_any_dtype(observation_set[SpecialColumnName.POINT_IN_TIME]):
-        observation_set = observation_set.copy()
-        observation_set[SpecialColumnName.POINT_IN_TIME] = pd.to_datetime(
-            observation_set[SpecialColumnName.POINT_IN_TIME]
+    # Adjust left timestamps if offset is provided
+    if offset:
+        offset_seconds = pd.Timedelta(offset).total_seconds()
+        left_ts_col = adapter.dateadd_microsecond(
+            make_literal_value(offset_seconds * 1e6 * -1),
+            left_table.timestamp_column_expr,
+        )
+    else:
+        left_ts_col = left_table.timestamp_column_expr
+    right_ts_col = right_table.timestamp_column_expr
+    if convert_timestamps_to_utc:
+        left_ts_col = _convert_to_utc_ntz(left_ts_col, adapter)
+        right_ts_col = _convert_to_utc_ntz(right_ts_col, adapter)
+
+    # Left table. Set up special columns: TS_COL, KEY_COL, EFFECTIVE_TS_COL and TS_TIE_BREAKER_COL
+    left_view_with_ts_and_key = select(
+        alias_(left_ts_col, alias=TS_COL, quoted=True),
+        *_alias_join_keys_as_key_cols(left_table.join_keys),
+        alias_(expressions.NULL, alias=EFFECTIVE_TS_COL, quoted=True),
+        alias_(
+            make_literal_value(
+                TS_TIE_BREAKER_VALUE_ALLOW_EXACT_MATCH
+                if allow_exact_match
+                else TS_TIE_BREAKER_VALUE_DISALLOW_EXACT_MATCH
+            ),
+            alias=TS_TIE_BREAKER_COL,
+            quoted=True,
+        ),
+    ).from_(left_table.as_subquery())
+
+    # Include all columns specified for the left table
+    for input_col, output_col in zip(left_table.input_columns, left_table.output_columns):
+        left_view_with_ts_and_key = left_view_with_ts_and_key.select(
+            alias_(quoted_identifier(input_col), alias=output_col, quoted=True)
         )
 
-    # convert point in time to tz-naive UTC timestamps
-    observation_set = observation_set.copy()
-    observation_set[SpecialColumnName.POINT_IN_TIME] = pd.to_datetime(
-        observation_set[SpecialColumnName.POINT_IN_TIME], utc=True
-    ).dt.tz_localize(None)
-
-    return observation_set
-
+    # Right table. Set up the same special columns. The ordering of the columns in the SELECT
+    # statement matters (must match the left table's).
+    right_ts_and_key = select(
+        alias_(right_ts_col, alias=TS_COL, quoted=True),
+        *_alias_join_keys_as_key_cols(right_table.join_keys),
+        alias_(
+            right_table.timestamp_column_expr,
+            alias=EFFECTIVE_TS_COL,
+            quoted=True,
+        ),
+        alias_(
+            make_literal_value(TS_TIE_BREAKER_VALUE_SCD_TABLE),
+            alias=TS_TIE_BREAKER_COL,
+            quoted=True,
+        ),
+    ).from_(right_table.as_subquery())
+
+    # Include all columns specified for the right table, but simply set them as NULL.
+    for column in left_table.output_columns:
+        right_ts_and_key = right_ts_and_key.select(
+            alias_(expressions.NULL, alias=column, quoted=True)
+        )
 
-def validate_historical_requests_point_in_time(observation_set: ObservationSet) -> None:
-    """Validate the point in time column in the request input and perform type conversion if needed
+    # Merge the above two temporary tables into one
+    all_ts_and_key = expressions.Union(
+        this=left_view_with_ts_and_key,
+        expression=right_ts_and_key,
+        distinct=False,
+    )
 
-    A copy will be made if the point in time column does not already have timestamp dtype.
+    # Sorting additionally by TS_TIE_BREAKER_COL to respect the specified exact matching behaviour.
+    #
+    # When allow_exact_match=True and TS_COL ties, after the sorting in LAG, rows from the left
+    # table will come after SCD rows in the right table since left rows have a larger value for
+    # TS_TILE_BREAKER_VALUE (2) than right rows (always 1). This way, LAG yields the exact matching
+    # date, instead of a previous effective date. Vice versa for allow_exact_match=False.
+    order = expressions.Order(
+        expressions=[
+            expressions.Ordered(this=quoted_identifier(TS_COL)),
+            expressions.Ordered(this=quoted_identifier(TS_TIE_BREAKER_COL)),
+        ]
+    )
+    num_join_keys = len(left_table.join_keys)
+    matched_effective_timestamp_expr = expressions.Window(
+        this=expressions.IgnoreNulls(
+            this=expressions.Anonymous(
+                this="LAG", expressions=[quoted_identifier(EFFECTIVE_TS_COL)]
+            ),
+        ),
+        partition_by=_key_cols_as_quoted_identifiers(num_join_keys),
+        order=order,
+    )
 
-    Parameters
-    ----------
-    observation_set: ObservationSet
-        Observation set
+    # Need to use a nested query for this filter due to the LAG window function
+    filter_original_left_view_rows = expressions.Is(
+        this=quoted_identifier(EFFECTIVE_TS_COL),
+        expression=expressions.NULL,
+    )
 
-    Raises
-    ------
-    TooRecentPointInTimeError
-        If any of the provided point in time values are too recent
-    """
-    # Latest point in time must be older than 48 hours
-    latest_point_in_time = observation_set.most_recent_point_in_time
-    recency = datetime.datetime.now() - latest_point_in_time
-    if recency <= pd.Timedelta(HISTORICAL_REQUESTS_POINT_IN_TIME_RECENCY_HOUR, unit="h"):
-        raise TooRecentPointInTimeError(
-            f"The latest point in time ({latest_point_in_time}) should not be more recent than "
-            f"{HISTORICAL_REQUESTS_POINT_IN_TIME_RECENCY_HOUR} hours from now"
+    left_view_with_effective_timestamp_expr = (
+        select(
+            *_key_cols_as_quoted_identifiers(num_join_keys),
+            quoted_identifier(LAST_TS),
+            *[quoted_identifier(col) for col in left_table.output_columns],
         )
+        .from_(
+            select(
+                *_key_cols_as_quoted_identifiers(num_join_keys),
+                alias_(matched_effective_timestamp_expr, alias=LAST_TS, quoted=True),
+                *[quoted_identifier(col) for col in left_table.output_columns],
+                quoted_identifier(EFFECTIVE_TS_COL),
+            )
+            .from_(all_ts_and_key.subquery())
+            .subquery()
+        )
+        .where(filter_original_left_view_rows)
+    )
 
+    return left_view_with_effective_timestamp_expr
 
-def validate_request_schema(observation_set: ObservationSet) -> None:
-    """Validate observation set schema
-
-    Parameters
-    ----------
-    observation_set: ObservationSet
-        Observation set
 
-    Raises
-    ------
-    MissingPointInTimeColumnError
-        If point in time column is not provided
-    """
-    if SpecialColumnName.POINT_IN_TIME not in observation_set.columns:
-        raise MissingPointInTimeColumnError("POINT_IN_TIME column is required")
-
-
-def get_historical_features_expr(
-    request_table_name: str,
-    graph: QueryGraph,
-    nodes: list[Node],
-    request_table_columns: list[str],
-    source_type: SourceType,
-    serving_names_mapping: dict[str, str] | None = None,
-    parent_serving_preparation: Optional[ParentServingPreparation] = None,
-) -> expressions.Select:
-    """Construct the SQL code that extracts historical features
+def _alias_join_keys_as_key_cols(join_keys: list[str]) -> list[Expression]:
+    """
+    Alias join keys as internal key columns (e.g. "CUST_ID" AS "__FB_KEY_COL_0")
 
     Parameters
     ----------
-    request_table_name : str
-        Name of request table to use
-    graph : QueryGraph
-        Query graph
-    nodes : list[Node]
-        List of query graph node
-    request_table_columns : list[str]
-        List of column names in the training events
-    source_type : SourceType
-        Source type information
-    serving_names_mapping : dict[str, str] | None
-        Optional mapping from original serving name to new serving name
-    parent_serving_preparation: Optional[ParentServingPreparation]
-        Preparation required for serving parent features
+    join_keys: list[str]
+        List of join keys
 
     Returns
     -------
-    expressions.Select
+    list[Expression]
     """
-    planner = FeatureExecutionPlanner(
-        graph,
-        serving_names_mapping=serving_names_mapping,
-        source_type=source_type,
-        is_online_serving=False,
-        parent_serving_preparation=parent_serving_preparation,
-    )
-    plan = planner.generate_plan(nodes)
-
-    return plan.construct_combined_sql(
-        request_table_name=request_table_name,
-        point_in_time_column=SpecialColumnName.POINT_IN_TIME,
-        request_table_columns=request_table_columns,
-    )
+    return [
+        alias_(quoted_identifier(join_key), alias=f"{KEY_COL}_{i}", quoted=True)
+        for (i, join_key) in enumerate(join_keys)
+    ]
 
 
-async def compute_tiles_on_demand(
-    session: BaseSession,
-    graph: QueryGraph,
-    nodes: list[Node],
-    request_id: str,
-    request_table_name: str,
-    request_table_columns: list[str],
-    serving_names_mapping: Optional[dict[str, str]],
-    parent_serving_preparation: Optional[ParentServingPreparation] = None,
-    progress_callback: Optional[Callable[[int, str], None]] = None,
-) -> None:
+def _key_cols_as_quoted_identifiers(num_join_keys: int) -> list[Expression]:
     """
-    Compute tiles on demand
+    Get a list of quoted internal key columns (e.g. "__FB_KEY_COL_0")
 
     Parameters
     ----------
-    session: BaseSession
-        Session to use to make queries
-    graph: QueryGraph
-        Query graph
-    nodes: list[Node]
-        List of query graph node
-    request_id: str
-        Request ID to be used as suffix of table names when creating temporary tables
-    request_table_name: str
-        Name of request table
-    request_table_columns: list[str]
-        List of column names in the observations set
-    serving_names_mapping : dict[str, str] | None
-        Optional serving names mapping if the training events data has different serving name
-        columns than those defined in Entities
-    parent_serving_preparation: Optional[ParentServingPreparation]
-        Preparation required for serving parent features
-    progress_callback: Optional[Callable[[int, str], None]]
-        Optional progress callback function
-    """
-    tic = time.time()
-    tile_cache = TileCache(session=session)
+    num_join_keys: int
+        Length of join keys
 
-    if parent_serving_preparation is None:
-        effective_request_table_name = request_table_name
-    else:
-        # Lookup parent entities and join them with the request table since tile computation
-        # requires these entity columns to be present in the request table.
-        request_table_expr, _ = construct_request_table_with_parent_entities(
-            request_table_name=request_table_name,
-            request_table_columns=request_table_columns,
-            join_steps=parent_serving_preparation.join_steps,
-            feature_store_details=parent_serving_preparation.feature_store_details,
-        )
-        request_table_query = sql_to_string(request_table_expr, session.source_type)
-        effective_request_table_name = "JOINED_PARENTS_" + request_table_name
-        await session.register_table_with_query(
-            effective_request_table_name,
-            request_table_query,
-        )
+    Returns
+    -------
+    list[Expression]
+    """
+    return [quoted_identifier(f"{KEY_COL}_{i}") for i in range(num_join_keys)]
 
-    await tile_cache.compute_tiles_on_demand(
-        graph=graph,
-        nodes=nodes,
-        request_id=request_id,
-        request_table_name=effective_request_table_name,
-        serving_names_mapping=serving_names_mapping,
-        progress_callback=progress_callback,
-    )
-    elapsed = time.time() - tic
-    logger.debug(f"Checking and computing tiles on demand took {elapsed:.2f}s")
 
+def _key_cols_equality_conditions(right_table_join_keys: list[str]) -> list[expressions.EQ]:
+    """
+    Get a list of equality conditions used for joining with scd view
 
-async def get_historical_features(
-    session: BaseSession,
-    graph: QueryGraph,
-    nodes: list[Node],
-    observation_set: Union[pd.DataFrame, ObservationTableModel],
-    source_type: SourceType,
-    serving_names_mapping: dict[str, str] | None = None,
-    is_feature_list_deployed: bool = False,
-    parent_serving_preparation: Optional[ParentServingPreparation] = None,
-    output_table_details: Optional[TableDetails] = None,
-    progress_callback: Optional[Callable[[int, str], None]] = None,
-) -> Optional[AsyncGenerator[bytes, None]]:
-    """Get historical features
+    (e.g. L."__FB_KEY_COL_0" = R."CUST_ID")
 
     Parameters
     ----------
-    session: BaseSession
-        Session to use to make queries
-    graph : QueryGraph
-        Query graph
-    nodes : list[Node]
-        List of query graph node
-    observation_set : Union[pd.DataFrame, ObservationTableModel]
-        Observation set
-    source_type : SourceType
-        Source type information
-    serving_names_mapping : dict[str, str] | None
-        Optional serving names mapping if the observations set has different serving name columns
-        than those defined in Entities
-    is_feature_list_deployed : bool
-        Whether the feature list that triggered this historical request is deployed. If so, tile
-        tables would have already been back-filled and there is no need to check and calculate tiles
-        on demand.
-    parent_serving_preparation: Optional[ParentServingPreparation]
-        Preparation required for serving parent features
-    output_table_details: Optional[TableDetails]
-        Optional output table details to write the results to. If this parameter is provided, the
-        function will return None (intended to be used when handling asynchronous historical
-        requests).
-    progress_callback: Optional[Callable[[int, str], None]]
-        Optional progress callback function
+    right_table_join_keys: list[str]
+        Join keys in the right table, will be prefixed with table alias "R"
 
     Returns
     -------
-    AsyncGenerator[bytes, None]
+    list[expressions.EQ]
     """
-    tic_ = time.time()
-
-    observation_set = get_internal_observation_set(observation_set)
+    return [
+        expressions.EQ(
+            this=get_qualified_column_identifier(f"{KEY_COL}_{i}", "L"),
+            expression=get_qualified_column_identifier(join_key, "R"),
+        )
+        for (i, join_key) in enumerate(right_table_join_keys)
+    ]
 
-    # Validate request
-    validate_request_schema(observation_set)
-    validate_historical_requests_point_in_time(observation_set)
-
-    # use a unique request table name
-    request_id = session.generate_session_unique_id()
-    request_table_name = f"{REQUEST_TABLE_NAME}_{request_id}"
-
-    # Generate SQL code that computes the features
-    request_table_columns = observation_set.columns
-    sql_expr = get_historical_features_expr(
-        graph=graph,
-        nodes=nodes,
-        request_table_columns=request_table_columns,
-        serving_names_mapping=serving_names_mapping,
-        source_type=source_type,
-        request_table_name=request_table_name,
-        parent_serving_preparation=parent_serving_preparation,
-    )
 
-    # Execute feature SQL code
-    await observation_set.register_as_request_table(session, request_table_name)
+def augment_scd_table_with_end_timestamp(
+    table_expr: Select,
+    effective_timestamp_column: str,
+    natural_key_column: str,
+) -> Select:
+    """
+    Augment a given SCD table with end timestamp column (the timestamp when an SCD record becomes
+    ineffective because of the next SCD record)
 
-    # Compute tiles on demand if required
-    if not is_feature_list_deployed:
-        await compute_tiles_on_demand(
-            session=session,
-            graph=graph,
-            nodes=nodes,
-            request_id=request_id,
-            request_table_name=request_table_name,
-            request_table_columns=request_table_columns,
-            serving_names_mapping=serving_names_mapping,
-            parent_serving_preparation=parent_serving_preparation,
-            progress_callback=progress_callback,
-        )
+    Parameters
+    ----------
+    table_expr: Select
+        Select statement representing the SCD table
+    effective_timestamp_column: str
+        Effective timestamp column name
+    natural_key_column: str
+        Natural key column name
 
-    if progress_callback:
-        progress_callback(TILE_COMPUTE_PROGRESS_MAX_PERCENT, "Computing features")
+    Returns
+    -------
+    Select
+    """
 
-    # Execute feature query and stream results back
-    if output_table_details is None:
-        sql = sql_to_string(sql_expr, source_type=session.source_type)
-        return session.get_async_query_stream(sql)
-
-    # Execute feature query but write results to a table
-    expression = get_sql_adapter(session.source_type).create_table_as(
-        table_details=output_table_details, select_expr=sql_expr
+    order = expressions.Order(
+        expressions=[
+            expressions.Ordered(this=quoted_identifier(effective_timestamp_column)),
+        ]
     )
-    query = sql_to_string(
-        expression,
-        source_type=session.source_type,
+    end_timestamp_expr = expressions.Window(
+        this=expressions.Anonymous(
+            this="LEAD", expressions=[quoted_identifier(effective_timestamp_column)]
+        ),
+        partition_by=[quoted_identifier(natural_key_column)],
+        order=order,
     )
-    await session.execute_query_long_running(query)
-    logger.debug(f"compute_historical_features in total took {time.time() - tic_:.2f}s")
+    updated_table_expr = select(
+        "*",
+        alias_(end_timestamp_expr, alias=END_TS, quoted=True),
+    ).from_(table_expr.subquery())
 
-    return None
+    return updated_table_expr
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/feature_preview.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/feature_preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/groupby_helper.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/groupby_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/base.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/preview.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/tile.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/materialisation.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/materialisation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving_util.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/parent_serving.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/specs.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     EventLookupParameters,
     GroupByNode,
     ItemGroupbyNode,
     ItemGroupbyParameters,
     LookupNode,
     SCDLookupParameters,
 )
+from featurebyte.query_graph.node.mixin import BaseGroupbyParameters
 from featurebyte.query_graph.sql.adapter import BaseAdapter
 from featurebyte.query_graph.sql.common import apply_serving_names_mapping
 from featurebyte.query_graph.sql.tiling import InputColumn, get_aggregator
 
 NonTileBasedAggregationSpecT = TypeVar(
     "NonTileBasedAggregationSpecT", bound="NonTileBasedAggregationSpec"
 )
@@ -284,14 +285,37 @@
 
         sql_node = cast(Aggregate, sql_node)
         return sql_node.to_aggregation_source()  # type: ignore
 
     def construct_agg_result_name(self, *args: Any) -> str:
         return super().construct_agg_result_name(*args, self.aggregation_source.query_node_name)
 
+    def get_agg_result_name_from_groupby_parameters(self, parameters: BaseGroupbyParameters) -> str:
+        """
+        Get the name of the aggregation result column from groupby parameters. The name should
+        include the parameters that can affect the result of the groupby operation: aggregation
+        function, parent variable, groupby keys and category key (optional).
+
+        Parameters
+        ----------
+        parameters: BaseGroupbyParameters
+            Groupby parameters
+
+        Returns
+        -------
+        str
+        """
+        args = [
+            parameters.agg_func,
+            parameters.parent,
+            *(parameters.keys or [None]),  # type: ignore
+            parameters.value_by or None,
+        ]
+        return self.construct_agg_result_name(*args)
+
     @classmethod
     def should_filter_scd_by_current_flag(cls, graph: QueryGraphModel, node: Node) -> bool:
         """
         Whether the SCD table should be filtered by current flag during online serving
 
         Parameters
         ----------
@@ -431,15 +455,15 @@
         """Column name of the aggregated result
 
         Returns
         -------
         str
             Column name of the aggregated result
         """
-        return self.construct_agg_result_name(self.parameters.agg_func, self.parameters.parent)
+        return self.get_agg_result_name_from_groupby_parameters(self.parameters)
 
     @property
     def aggregation_type(self) -> AggregationType:
         return AggregationType.ITEM
 
     def get_source_hash_parameters(self) -> dict[str, Any]:
         params: dict[str, Any] = {"source_expr": self.source_expr.sql()}
@@ -483,15 +507,15 @@
         """Column name of the aggregated result
 
         Returns
         -------
         str
             Column name of the aggregated result
         """
-        return self.construct_agg_result_name(self.parameters.agg_func, self.parameters.parent)
+        return self.get_agg_result_name_from_groupby_parameters(self.parameters)
 
     @property
     def aggregation_type(self) -> AggregationType:
         return AggregationType.AS_AT
 
     def get_source_hash_parameters(self) -> dict[str, Any]:
         # Input to be aggregated
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/template.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/tile_compute.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/tile_compute.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import pandas as pd
 from sqlglot import expressions
 from sqlglot.expressions import Select, select
 
 from featurebyte.enum import InternalName, SourceType
 from featurebyte.query_graph.model.graph import QueryGraphModel
 from featurebyte.query_graph.node import Node
-from featurebyte.query_graph.sql.ast.literal import make_literal_value
 from featurebyte.query_graph.sql.common import CteStatements, quoted_identifier
 from featurebyte.query_graph.sql.interpreter import GraphInterpreter, TileGenSql
 from featurebyte.query_graph.sql.template import SqlExpressionTemplate
 from featurebyte.query_graph.sql.tile_util import update_maximum_window_size_dict
 
 
 class OnDemandTileComputePlan:
@@ -76,30 +75,22 @@
 
         tile_sqls: dict[str, Select] = {}
         prev_aliases: dict[str, str] = {}
 
         for tile_info in self.tile_infos:
             # Convert template SQL with concrete start and end timestamps, based on the requested
             # point-in-time and feature window sizes
-            tile_sql_with_start_end_expr = get_tile_sql_from_point_in_time(
+            tile_sql_expr = get_tile_sql_from_point_in_time(
                 sql_template=tile_info.sql_template,
                 point_in_time_list=self.point_in_time_list,
                 frequency=tile_info.frequency,
                 time_modulo_frequency=tile_info.time_modulo_frequency,
                 blind_spot=tile_info.blind_spot,
                 window=self.get_max_window_size(tile_info.tile_table_id),
             )
-            # Include global tile index that would have been computed by F_TIMESTAMP_TO_INDEX UDF
-            # during scheduled tile jobs
-            tile_sql_expr = get_tile_sql_parameterized_by_job_settings(
-                tile_sql_with_start_end_expr,
-                frequency=tile_info.frequency,
-                time_modulo_frequency=tile_info.time_modulo_frequency,
-                blind_spot=tile_info.blind_spot,
-            )
 
             # Build wide tile table by joining tile sqls with the same tile_table_id
             tile_table_id = tile_info.tile_table_id
             agg_id = tile_info.aggregation_id
             assert isinstance(tile_sql_expr, expressions.Subqueryable)
 
             if tile_table_id not in tile_sqls:
@@ -271,15 +262,15 @@
         Tuple of start and end dates
     """
     # Convert point in time to UNIX timestamp
     point_in_time_epoch_seconds_list = [
         get_epoch_seconds(point_in_time) for point_in_time in point_in_time_list
     ]
 
-    def _compute_end_date_epoch_seconds(point_in_time_epoch_seconds: int) -> pd.Timestamp:
+    def _compute_end_date_epoch_seconds(point_in_time_epoch_seconds: int) -> int:
         """
         Compute end date based on point in time in epoch seconds
 
         Parameters
         ----------
         point_in_time_epoch_seconds : int
             Point in time in epoch seconds
@@ -360,50 +351,7 @@
         {
             InternalName.TILE_START_DATE_SQL_PLACEHOLDER: str(start_date),
             InternalName.TILE_END_DATE_SQL_PLACEHOLDER: str(end_date),
         },
         as_str=False,
     )
     return cast(Select, out_expr)
-
-
-def get_tile_sql_parameterized_by_job_settings(
-    tile_sql_expr: Select,
-    frequency: int,
-    time_modulo_frequency: int,
-    blind_spot: int,
-) -> Select:
-    """Get the final tile SQL code that would have been executed by the tile schedule job
-
-    The template SQL code doesn't contain the tile index, which is computed by the tile schedule job
-    by F_TIMESTAMP_TO_INDEX. This produces a SQL that incorporates that.
-
-    Parameters
-    ----------
-    tile_sql_expr : Select
-        Tile SQL expression with placeholders already filled
-    frequency : int
-        Frequency in feature job setting
-    time_modulo_frequency : int
-        Time modulo frequency in feature job setting
-    blind_spot : int
-        Blind spot in feature job setting
-
-    Returns
-    -------
-    Select
-    """
-    frequency_minute = frequency // 60
-    f_time_to_index_expr = expressions.Anonymous(
-        this="F_TIMESTAMP_TO_INDEX",
-        expressions=[
-            InternalName.TILE_START_DATE.value,
-            make_literal_value(time_modulo_frequency),
-            make_literal_value(blind_spot),
-            make_literal_value(frequency_minute),
-        ],
-    )
-    expr = select(
-        "*",
-        expressions.alias_(expression=f_time_to_index_expr, alias=quoted_identifier("INDEX")),
-    ).from_(tile_sql_expr.subquery())
-    return expr
```

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/tile_util.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/sql/tiling.py` & `featurebyte-0.3.0/featurebyte/query_graph/sql/tiling.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/transform/base.py` & `featurebyte-0.3.0/featurebyte/query_graph/transform/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/transform/flattening.py` & `featurebyte-0.3.0/featurebyte/query_graph/transform/flattening.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/transform/operation_structure.py` & `featurebyte-0.3.0/featurebyte/query_graph/transform/operation_structure.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/transform/pruning.py` & `featurebyte-0.3.0/featurebyte/query_graph/transform/pruning.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/transform/reconstruction.py` & `featurebyte-0.3.0/featurebyte/query_graph/transform/reconstruction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/query_graph/util.py` & `featurebyte-0.3.0/featurebyte/query_graph/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/app_container.py` & `featurebyte-0.3.0/featurebyte/routes/app_container.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/app_container_config.py` & `featurebyte-0.3.0/featurebyte/routes/app_container_config.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/batch_feature_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/batch_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/batch_feature_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/batch_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/batch_request_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/batch_request_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/batch_request_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/batch_request_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/catalog/api.py` & `featurebyte-0.3.0/featurebyte/routes/catalog/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/catalog/controller.py` & `featurebyte-0.3.0/featurebyte/routes/catalog/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/common/base.py` & `featurebyte-0.3.0/featurebyte/routes/common/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         Returns
         -------
         Document
 
         Raises
         ------
-        HTTPException
+        DocumentNotFound
             If the object not found
         """
         document = await self.service.get_document(
             document_id=document_id,
             exception_detail=exception_detail,
         )
         return cast(Document, document)
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/common/base_materialized_table.py` & `featurebyte-0.3.0/featurebyte/routes/common/base_materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/common/base_table.py` & `featurebyte-0.3.0/featurebyte/routes/common/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/common/schema.py` & `featurebyte-0.3.0/featurebyte/routes/common/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/context/api.py` & `featurebyte-0.3.0/featurebyte/routes/context/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/context/controller.py` & `featurebyte-0.3.0/featurebyte/routes/context/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/credential/api.py` & `featurebyte-0.3.0/featurebyte/routes/credential/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/credential/controller.py` & `featurebyte-0.3.0/featurebyte/routes/credential/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/deployment/api.py` & `featurebyte-0.3.0/featurebyte/routes/deployment/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/deployment/controller.py` & `featurebyte-0.3.0/featurebyte/routes/deployment/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/dimension_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/dimension_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/dimension_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/dimension_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/entity/api.py` & `featurebyte-0.3.0/featurebyte/routes/entity/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/entity/controller.py` & `featurebyte-0.3.0/featurebyte/routes/entity/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/event_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/event_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/event_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/event_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature/api.py` & `featurebyte-0.3.0/featurebyte/routes/feature/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,25 @@
     SortByQuery,
     SortDirQuery,
     VerboseQuery,
     VersionQuery,
 )
 from featurebyte.schema.common.base import DeleteResponse
 from featurebyte.schema.feature import (
+    BatchFeatureCreate,
     FeatureCreate,
     FeatureModelResponse,
     FeatureNewVersionCreate,
     FeaturePaginatedList,
     FeaturePreview,
     FeatureSQL,
     FeatureUpdate,
 )
 from featurebyte.schema.info import FeatureInfo
+from featurebyte.schema.task import Task
 
 router = APIRouter(prefix="/feature")
 
 
 @router.post("", response_model=FeatureModelResponse, status_code=HTTPStatus.CREATED)
 async def create_feature(
     request: Request, data: Union[FeatureCreate, FeatureNewVersionCreate]
@@ -45,14 +47,24 @@
     Create Feature
     """
     controller = request.state.app_container.feature_controller
     feature: FeatureModelResponse = await controller.create_feature(data=data)
     return feature
 
 
+@router.post("/batch", response_model=Task, status_code=HTTPStatus.CREATED)
+async def submit_batch_feature_create_task(request: Request, data: BatchFeatureCreate) -> Task:
+    """
+    Submit Batch Feature Create Task
+    """
+    controller = request.state.app_container.feature_controller
+    task: Task = await controller.submit_batch_feature_create_task(data=data)
+    return task
+
+
 @router.get("/{feature_id}", response_model=FeatureModelResponse)
 async def get_feature(request: Request, feature_id: PydanticObjectId) -> FeatureModelResponse:
     """
     Get Feature
     """
     controller = request.state.app_container.feature_controller
     feature: FeatureModelResponse = await controller.get(document_id=feature_id)
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature/controller.py` & `featurebyte-0.3.0/featurebyte/routes/feature/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Feature API route controller
 """
 from __future__ import annotations
 
-from typing import Any, Dict, Literal, Union, cast
+from typing import Any, Dict, Literal, Optional, Union, cast
 
 from http import HTTPStatus
 from pprint import pformat
 
 from bson.objectid import ObjectId
 from fastapi.exceptions import HTTPException
 
@@ -20,36 +20,42 @@
 from featurebyte.models.base import VersionIdentifier
 from featurebyte.models.feature import DefaultVersionMode, FeatureModel, FeatureReadiness
 from featurebyte.routes.common.base import (
     BaseDocumentController,
     DerivePrimaryEntityMixin,
     PaginatedDocument,
 )
+from featurebyte.routes.task.controller import TaskController
 from featurebyte.schema.feature import (
+    BatchFeatureCreate,
     FeatureCreate,
     FeatureModelResponse,
     FeatureNewVersionCreate,
     FeaturePaginatedList,
     FeaturePreview,
+    FeatureServiceCreate,
     FeatureSQL,
     FeatureUpdate,
 )
 from featurebyte.schema.info import FeatureInfo
+from featurebyte.schema.task import Task
+from featurebyte.schema.worker.task.batch_feature_create import BatchFeatureCreateTaskPayload
 from featurebyte.service.entity import EntityService
 from featurebyte.service.feature import FeatureService
 from featurebyte.service.feature_list import FeatureListService
 from featurebyte.service.feature_namespace import FeatureNamespaceService
 from featurebyte.service.feature_readiness import FeatureReadinessService
 from featurebyte.service.feature_store_warehouse import FeatureStoreWarehouseService
 from featurebyte.service.info import InfoService
 from featurebyte.service.mixin import Document
 from featurebyte.service.preview import PreviewService
 from featurebyte.service.version import VersionService
 
 
+# pylint: disable=too-many-instance-attributes
 class FeatureController(
     BaseDocumentController[FeatureModelResponse, FeatureService, FeaturePaginatedList],
     DerivePrimaryEntityMixin,
 ):
     """
     Feature controller
     """
@@ -63,24 +69,50 @@
         entity_service: EntityService,
         feature_list_service: FeatureListService,
         feature_readiness_service: FeatureReadinessService,
         preview_service: PreviewService,
         version_service: VersionService,
         info_service: InfoService,
         feature_store_warehouse_service: FeatureStoreWarehouseService,
+        task_controller: TaskController,
     ):
+        # pylint: disable=too-many-arguments
         super().__init__(service)
         self.feature_namespace_service = feature_namespace_service
         self.entity_service = entity_service
         self.feature_list_service = feature_list_service
         self.feature_readiness_service = feature_readiness_service
         self.preview_service = preview_service
         self.version_service = version_service
         self.info_service = info_service
         self.feature_store_warehouse_service = feature_store_warehouse_service
+        self.task_controller = task_controller
+
+    async def submit_batch_feature_create_task(self, data: BatchFeatureCreate) -> Optional[Task]:
+        """
+        Submit Feature Create Task
+
+        Parameters
+        ----------
+        data: BatchFeatureCreate
+            Batch Feature creation payload
+
+        Returns
+        -------
+        Optional[Task]
+            Task object
+        """
+        payload = BatchFeatureCreateTaskPayload(
+            **{
+                **data.json_dict(),
+                "catalog_id": self.service.catalog_id,
+            }
+        )
+        task_id = await self.task_controller.task_manager.submit(payload=payload)
+        return await self.task_controller.task_manager.get_task(task_id=str(task_id))
 
     async def create_feature(
         self, data: Union[FeatureCreate, FeatureNewVersionCreate]
     ) -> FeatureModelResponse:
         """
         Create Feature at persistent (GitDB or MongoDB)
 
@@ -91,15 +123,17 @@
 
         Returns
         -------
         FeatureModelResponse
             Newly created feature object
         """
         if isinstance(data, FeatureCreate):
-            document = await self.service.create_document(data=data)
+            document = await self.service.create_document(
+                data=FeatureServiceCreate(**data.json_dict())
+            )
         else:
             document = await self.version_service.create_new_feature_version(data=data)
 
         # update feature namespace readiness due to introduction of new feature
         await self.feature_readiness_service.update_feature_namespace(
             feature_namespace_id=document.feature_namespace_id,
             return_document=False,
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/api.py` & `featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/controller.py` & `featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_list/api.py` & `featurebyte-0.3.0/featurebyte/routes/feature_list/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from typing import Any, Dict, Optional, Union, cast
 
 import json
 from http import HTTPStatus
 
 from fastapi import APIRouter, File, Form, Query, Request, UploadFile
-from fastapi.responses import StreamingResponse
 
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.feature_list import FeatureListModel
 from featurebyte.models.persistent import AuditDocumentList
 from featurebyte.routes.common.schema import (
     AuditLogSortByQuery,
     NameQuery,
@@ -174,33 +173,14 @@
         Dict[str, Any],
         await controller.preview(
             featurelist_preview=featurelist_preview, get_credential=request.state.get_credential
         ),
     )
 
 
-@router.post("/historical_features")
-async def get_historical_features(
-    request: Request,
-    payload: str = Form(),
-    observation_set: UploadFile = File(description="Observation set data in parquet format"),
-) -> StreamingResponse:
-    """
-    Retrieve historical features
-    """
-    featurelist_get_historical_features = FeatureListGetHistoricalFeatures(**json.loads(payload))
-    controller = request.state.app_container.feature_list_controller
-    result: StreamingResponse = await controller.compute_historical_features(
-        observation_set=observation_set,
-        featurelist_get_historical_features=featurelist_get_historical_features,
-        get_credential=request.state.get_credential,
-    )
-    return result
-
-
 @router.post("/sql", response_model=str)
 async def get_feature_list_sql(
     request: Request,
     featurelist_sql: FeatureListSQL,
 ) -> str:
     """
     Retrieve FeatureList SQL
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_list/controller.py` & `featurebyte-0.3.0/featurebyte/routes/feature_list/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,35 +6,34 @@
 from typing import Any, Dict, Literal, Union
 
 from http import HTTPStatus
 
 from bson.objectid import ObjectId
 from fastapi import UploadFile
 from fastapi.exceptions import HTTPException
-from fastapi.responses import StreamingResponse
 
 from featurebyte.common.utils import dataframe_from_arrow_stream
 from featurebyte.exception import (
     DocumentDeletionError,
     MissingPointInTimeColumnError,
     RequiredEntityNotProvidedError,
     TooRecentPointInTimeError,
-    UnexpectedServingNamesMappingError,
 )
 from featurebyte.feature_manager.model import ExtendedFeatureModel
 from featurebyte.models.base import VersionIdentifier
 from featurebyte.models.feature import DefaultVersionMode, FeatureReadiness
 from featurebyte.models.feature_list import FeatureListModel, FeatureListStatus
 from featurebyte.routes.common.base import BaseDocumentController
 from featurebyte.schema.feature_list import (
     FeatureListCreate,
     FeatureListGetHistoricalFeatures,
     FeatureListNewVersionCreate,
     FeatureListPaginatedList,
     FeatureListPreview,
+    FeatureListServiceCreate,
     FeatureListSQL,
     FeatureListUpdate,
 )
 from featurebyte.schema.info import FeatureListInfo
 from featurebyte.service.deploy import DeployService
 from featurebyte.service.feature import FeatureService
 from featurebyte.service.feature_list import FeatureListService
@@ -92,15 +91,17 @@
 
         Returns
         -------
         FeatureListModel
             Newly created feature list object
         """
         if isinstance(data, FeatureListCreate):
-            document = await self.service.create_document(data=data)
+            document = await self.service.create_document(
+                data=FeatureListServiceCreate(**data.json_dict())
+            )
         else:
             document = await self.version_service.create_new_feature_list_version(data=data)
 
         # update feature namespace readiness due to introduction of new feature list
         await self.feature_readiness_service.update_feature_list_namespace(
             feature_list_namespace_id=document.feature_list_namespace_id,
             return_document=False,
@@ -270,63 +271,14 @@
                 featurelist_preview=featurelist_preview, get_credential=get_credential
             )
         except (MissingPointInTimeColumnError, RequiredEntityNotProvidedError) as exc:
             raise HTTPException(
                 status_code=HTTPStatus.UNPROCESSABLE_ENTITY, detail=exc.args[0]
             ) from exc
 
-    async def compute_historical_features(
-        self,
-        observation_set: UploadFile,
-        featurelist_get_historical_features: FeatureListGetHistoricalFeatures,
-        get_credential: Any,
-    ) -> StreamingResponse:
-        """
-        Get historical features for Feature List
-
-        Parameters
-        ----------
-        observation_set: UploadFile
-            Uploaded file
-        featurelist_get_historical_features: FeatureListGetHistoricalFeatures
-            FeatureListGetHistoricalFeatures object
-        get_credential: Any
-            Get credential handler function
-
-        Returns
-        -------
-        StreamingResponse
-            StreamingResponse object
-
-        Raises
-        ------
-        HTTPException
-            Invalid request payload
-        """
-        try:
-            bytestream = await self.preview_service.compute_historical_features(
-                observation_set=dataframe_from_arrow_stream(observation_set.file),
-                featurelist_get_historical_features=featurelist_get_historical_features,
-                get_credential=get_credential,
-            )
-            assert bytestream is not None
-        except (
-            MissingPointInTimeColumnError,
-            TooRecentPointInTimeError,
-            RequiredEntityNotProvidedError,
-            UnexpectedServingNamesMappingError,
-        ) as exc:
-            raise HTTPException(
-                status_code=HTTPStatus.UNPROCESSABLE_ENTITY, detail=exc.args[0]
-            ) from exc
-        return StreamingResponse(
-            bytestream,
-            media_type="application/octet-stream",
-        )
-
     async def get_info(
         self,
         document_id: ObjectId,
         verbose: bool,
     ) -> FeatureListInfo:
         """
         Get document info given document ID
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/api.py` & `featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,62 +5,62 @@
 from __future__ import annotations
 
 from typing import Optional, cast
 
 from fastapi import APIRouter, Request
 
 from featurebyte.models.base import PydanticObjectId
-from featurebyte.models.feature_list import FeatureListNamespaceModel
 from featurebyte.models.persistent import AuditDocumentList
 from featurebyte.routes.common.schema import (
     AuditLogSortByQuery,
     NameQuery,
     PageQuery,
     PageSizeQuery,
     SearchQuery,
     SortByQuery,
     SortDirQuery,
     VerboseQuery,
 )
 from featurebyte.schema.feature_list_namespace import (
     FeatureListNamespaceList,
+    FeatureListNamespaceModelResponse,
     FeatureListNamespaceUpdate,
 )
 from featurebyte.schema.info import FeatureListNamespaceInfo
 
 router = APIRouter(prefix="/feature_list_namespace")
 
 
-@router.get("/{feature_list_namespace_id}", response_model=FeatureListNamespaceModel)
+@router.get("/{feature_list_namespace_id}", response_model=FeatureListNamespaceModelResponse)
 async def get_feature_list_namespace(
     request: Request, feature_list_namespace_id: PydanticObjectId
-) -> FeatureListNamespaceModel:
+) -> FeatureListNamespaceModelResponse:
     """
     Get FeatureListNamespace
     """
     controller = request.state.app_container.feature_list_namespace_controller
-    feature_list_namespace: FeatureListNamespaceModel = await controller.get(
+    feature_list_namespace: FeatureListNamespaceModelResponse = await controller.get(
         document_id=feature_list_namespace_id,
         exception_detail=(
             f'FeatureListNamespace (id: "{feature_list_namespace_id}") not found. '
             "Please save the FeatureList object first."
         ),
     )
     return feature_list_namespace
 
 
-@router.patch("/{feature_list_namespace_id}", response_model=FeatureListNamespaceModel)
+@router.patch("/{feature_list_namespace_id}", response_model=FeatureListNamespaceModelResponse)
 async def update_feature_list_namespace(
     request: Request, feature_list_namespace_id: PydanticObjectId, data: FeatureListNamespaceUpdate
-) -> FeatureListNamespaceModel:
+) -> FeatureListNamespaceModelResponse:
     """
     Update FeatureListNamespace
     """
     controller = request.state.app_container.feature_list_namespace_controller
-    feature_list_namespace: FeatureListNamespaceModel = (
+    feature_list_namespace: FeatureListNamespaceModelResponse = (
         await controller.update_feature_list_namespace(
             feature_list_namespace_id=feature_list_namespace_id,
             data=data,
         )
     )
     return feature_list_namespace
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/controller.py` & `featurebyte-0.3.0/featurebyte/worker/task/batch_feature_create.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,135 +1,123 @@
 """
-FeatureListNamespace API route controller
+Batch feature create task
 """
 from __future__ import annotations
 
-from bson.objectid import ObjectId
+from typing import Any, cast
 
-from featurebyte.exception import DocumentUpdateError
-from featurebyte.models.feature import DefaultVersionMode
-from featurebyte.models.feature_list import FeatureListNamespaceModel
-from featurebyte.routes.common.base import BaseDocumentController
-from featurebyte.schema.feature_list_namespace import (
-    FeatureListNamespaceList,
-    FeatureListNamespaceServiceUpdate,
-    FeatureListNamespaceUpdate,
-)
-from featurebyte.schema.info import FeatureListNamespaceInfo
-from featurebyte.service.default_version_mode import DefaultVersionModeService
-from featurebyte.service.feature_list import FeatureListService
-from featurebyte.service.feature_list_namespace import FeatureListNamespaceService
-from featurebyte.service.feature_list_status import FeatureListStatusService
-from featurebyte.service.feature_readiness import FeatureReadinessService
-from featurebyte.service.info import InfoService
-
-
-class FeatureListNamespaceController(
-    BaseDocumentController[
-        FeatureListNamespaceModel, FeatureListNamespaceService, FeatureListNamespaceList
-    ]
-):
+import asyncio
+import concurrent.futures
+
+from bson import ObjectId
+
+from featurebyte.exception import DocumentInconsistencyError
+from featurebyte.logging import get_logger
+from featurebyte.models.base import activate_catalog
+from featurebyte.models.feature import FeatureModel
+from featurebyte.schema.feature import FeatureServiceCreate
+from featurebyte.schema.worker.task.batch_feature_create import BatchFeatureCreateTaskPayload
+from featurebyte.service.feature import FeatureService
+from featurebyte.worker.task.base import BaseTask
+
+logger = get_logger(__name__)
+
+
+async def execute_sdk_code(catalog_id: ObjectId, code: str) -> None:
+    """
+    Activate the catalog and execute the code in server mode
+
+    Parameters
+    ----------
+    catalog_id: ObjectId
+        The catalog id
+    code: str
+        The SDK code to execute
     """
-    FeatureList controller
+    # activate the correct catalog before executing the code
+    activate_catalog(catalog_id=catalog_id)
+
+    # execute the code
+    with concurrent.futures.ThreadPoolExecutor() as pool:
+        await asyncio.get_event_loop().run_in_executor(pool, exec, code)
+
+
+class BatchFeatureCreateTask(BaseTask):
+    """
+    Batch feature creation task
     """
 
-    paginated_document_class = FeatureListNamespaceList
+    payload_class = BatchFeatureCreateTaskPayload
 
-    def __init__(
-        self,
-        service: FeatureListNamespaceService,
-        feature_list_service: FeatureListService,
-        default_version_mode_service: DefaultVersionModeService,
-        feature_readiness_service: FeatureReadinessService,
-        feature_list_status_service: FeatureListStatusService,
-        info_service: InfoService,
-    ):
-        super().__init__(service)
-        self.feature_list_service = feature_list_service
-        self.default_version_mode_service = default_version_mode_service
-        self.feature_readiness_service = feature_readiness_service
-        self.feature_list_status_service = feature_list_status_service
-        self.info_service = info_service
-
-    async def update_feature_list_namespace(
-        self,
-        feature_list_namespace_id: ObjectId,
-        data: FeatureListNamespaceUpdate,
-    ) -> FeatureListNamespaceModel:
+    async def is_generated_feature_consistent(
+        self, document: FeatureModel, definition: str
+    ) -> bool:
         """
-        Update FeatureListNamespace stored at persistent (GitDB or MongoDB)
+        Validate the generated feature against the expected feature
 
         Parameters
         ----------
-        feature_list_namespace_id: ObjectId
-            FeatureListNamespace ID
-        data: FeatureListNamespaceUpdate
-            FeatureListNamespace update payload
+        document: FeatureModel
+            The feature document used to generate the feature definition
+        definition: str
+            Feature definition used at server side to generate the feature
 
         Returns
         -------
-        FeatureListNamespaceModel
-            FeatureListNamespace object with updated attribute(s)
+        bool
+        """
+        # retrieve the saved feature & check if it is the same as the expected feature
+        feature_service: FeatureService = self.app_container.feature_service
+        feature = await feature_service.get_document(document_id=document.id)
+        generated_hash = feature.graph.node_name_to_ref[feature.node_name]
+        expected_hash = document.graph.node_name_to_ref[document.node_name]
+        is_consistent = definition == feature.definition and expected_hash == generated_hash
+        if not is_consistent:
+            # log the difference between the expected feature and the saved feature
+            logger.debug(
+                "Generated feature is not the same as the expected feature",
+                extra={
+                    "feature_id": feature.id,
+                    "name": feature.name,
+                    "expected_hash": expected_hash,
+                    "generated_hash": generated_hash,
+                    "match_definition": definition == feature.definition,
+                },
+            )
+        return is_consistent
+
+    async def execute(self) -> Any:
+        """
+        Execute Deployment Create & Update Task
 
         Raises
         ------
-        DocumentUpdateError
-            When the new feature list version creation fails
+        DocumentInconsistencyError
+            If the generated feature is not the same as the expected feature
         """
-        if data.default_version_mode:
-            await self.default_version_mode_service.update_feature_list_namespace(
-                feature_list_namespace_id=feature_list_namespace_id,
-                default_version_mode=data.default_version_mode,
-                return_document=False,
+        payload = cast(BatchFeatureCreateTaskPayload, self.payload)
+        feature_service: FeatureService = self.app_container.feature_service
+        total = len(payload.features)
+
+        for i, feature_create_data in enumerate(payload.iterate_features()):
+            # prepare the feature document & definition
+            document = await feature_service.prepare_feature_model(
+                data=FeatureServiceCreate(**feature_create_data.json_dict()),
+                sanitize_for_definition=True,
             )
+            definition = await feature_service.prepare_feature_definition(document=document)
 
-        if data.default_feature_list_id:
-            feature_list_namespace = await self.service.get_document(
-                document_id=feature_list_namespace_id
-            )
-            if feature_list_namespace.default_version_mode != DefaultVersionMode.MANUAL:
-                raise DocumentUpdateError(
-                    "Cannot set default feature list ID when default version mode is not MANUAL."
-                )
-
-            # update feature list namespace default feature list ID and update feature readiness
-            await self.service.update_document(
-                document_id=feature_list_namespace_id,
-                data=FeatureListNamespaceServiceUpdate(
-                    default_feature_list_id=data.default_feature_list_id
-                ),
-            )
-            await self.feature_readiness_service.update_feature_list_namespace(
-                feature_list_namespace_id=feature_list_namespace_id
-            )
+            # execute the code to save the feature
+            await execute_sdk_code(catalog_id=payload.catalog_id, code=definition)
 
-        if data.status:
-            await self.feature_list_status_service.update_feature_list_namespace_status(
-                feature_list_namespace_id=feature_list_namespace_id,
-                target_feature_list_status=data.status,
+            # retrieve the saved feature & check if it is the same as the expected feature
+            is_consistent = await self.is_generated_feature_consistent(
+                document=document, definition=definition
             )
-
-        return await self.get(document_id=feature_list_namespace_id)
-
-    async def get_info(
-        self,
-        document_id: ObjectId,
-        verbose: bool,
-    ) -> FeatureListNamespaceInfo:
-        """
-        Get document info given document ID
-
-        Parameters
-        ----------
-        document_id: ObjectId
-            Document ID
-        verbose: bool
-            Flag to control verbose level
-
-        Returns
-        -------
-        InfoDocument
-        """
-        info_document = await self.info_service.get_feature_list_namespace_info(
-            document_id=document_id, verbose=verbose
-        )
-        return info_document
+            if not is_consistent:
+                # delete the generated feature & raise an error
+                await self.app_container.feature_controller.delete_feature(feature_id=document.id)
+                raise DocumentInconsistencyError("Inconsistent feature definition detected!")
+
+            # update the progress
+            percent = 100 * (i + 1) / total
+            self.update_progress(percent=int(percent), message="Completed {i+1}/{total} features")
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_namespace/api.py` & `featurebyte-0.3.0/featurebyte/routes/feature_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_namespace/controller.py` & `featurebyte-0.3.0/featurebyte/routes/feature_namespace/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             document_id=document_id,
             exception_detail=exception_detail,
         )
         default_feature = await self.feature_service.get_document(
             document_id=document.default_feature_id
         )
         output = FeatureNamespaceModelResponse(
-            **document.dict(by_alias=True),
+            **document.json_dict(),
             primary_table_ids=default_feature.primary_table_ids,
             primary_entity_ids=await self.derive_primary_entity_ids(entity_ids=document.entity_ids),
         )
         return cast(Document, output)
 
     async def list(
         self,
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_store/api.py` & `featurebyte-0.3.0/featurebyte/routes/feature_store/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/feature_store/controller.py` & `featurebyte-0.3.0/featurebyte/routes/feature_store/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/historical_feature_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/historical_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/historical_feature_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/historical_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/item_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/item_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/item_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/item_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/observation_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/observation_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/observation_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/observation_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/periodic_tasks/api.py` & `featurebyte-0.3.0/featurebyte/routes/periodic_tasks/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/periodic_tasks/controller.py` & `featurebyte-0.3.0/featurebyte/routes/periodic_tasks/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/registry.py` & `featurebyte-0.3.0/featurebyte/routes/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
         "entity_service",
         "feature_list_service",
         "feature_readiness_service",
         "preview_service",
         "version_service",
         "info_service",
         "feature_store_warehouse_service",
+        "task_controller",
     ],
 )
 app_container_config.add_controller(
     "feature_list_controller",
     FeatureListController,
     [
         "feature_list_service",
@@ -311,14 +312,15 @@
     ["feature_job_setting_analysis_service", "task_controller", "info_service"],
 )
 app_container_config.add_controller(
     "feature_list_namespace_controller",
     FeatureListNamespaceController,
     [
         "feature_list_namespace_service",
+        "entity_service",
         "feature_list_service",
         "default_version_mode_service",
         "feature_readiness_service",
         "feature_list_status_service",
         "info_service",
     ],
 )
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/relationship_info/api.py` & `featurebyte-0.3.0/featurebyte/routes/relationship_info/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from http import HTTPStatus
 
 from fastapi import APIRouter, Request
 
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.persistent import AuditDocumentList
-from featurebyte.models.relationship import RelationshipInfo
+from featurebyte.models.relationship import RelationshipInfoModel
 from featurebyte.routes.common.schema import (
     AuditLogSortByQuery,
     NameQuery,
     PageQuery,
     PageSizeQuery,
     SearchQuery,
     SortByQuery,
@@ -27,23 +27,23 @@
     RelationshipInfoList,
     RelationshipInfoUpdate,
 )
 
 router = APIRouter(prefix="/relationship_info")
 
 
-@router.post("", response_model=RelationshipInfo, status_code=HTTPStatus.CREATED)
+@router.post("", response_model=RelationshipInfoModel, status_code=HTTPStatus.CREATED)
 async def create_relationship_info(
     request: Request, data: RelationshipInfoCreate
-) -> RelationshipInfo:
+) -> RelationshipInfoModel:
     """
     Create relationship info
     """
     controller = request.state.app_container.relationship_info_controller
-    relationship_info: RelationshipInfo = await controller.create_relationship_info(data=data)
+    relationship_info: RelationshipInfoModel = await controller.create_relationship_info(data=data)
     return relationship_info
 
 
 @router.get("", response_model=RelationshipInfoList)
 async def list_relationship_info(
     request: Request,
     page: int = PageQuery,
@@ -64,42 +64,42 @@
         sort_dir=sort_dir,
         search=search,
         name=name,
     )
     return relationship_info_list
 
 
-@router.get("/{relationship_info_id}", response_model=RelationshipInfo)
+@router.get("/{relationship_info_id}", response_model=RelationshipInfoModel)
 async def get_relationship_info(
     request: Request, relationship_info_id: PydanticObjectId
-) -> RelationshipInfo:
+) -> RelationshipInfoModel:
     """
     Retrieve relationship info
     """
     controller = request.state.app_container.relationship_info_controller
-    relationship_info: RelationshipInfo = await controller.get(
+    relationship_info: RelationshipInfoModel = await controller.get(
         document_id=relationship_info_id,
     )
     return relationship_info
 
 
 @router.patch("/{relationship_info_id}")
 async def update_relationship_info(
     request: Request,
     relationship_info_id: PydanticObjectId,
     data: RelationshipInfoUpdate,
-) -> RelationshipInfo:
+) -> RelationshipInfoModel:
     """
     Update RelationshipInfo
     """
     controller = request.state.app_container.relationship_info_controller
     relationship_info = await controller.relationship_info_service.update_document(
         relationship_info_id, data
     )
-    return cast(RelationshipInfo, relationship_info)
+    return cast(RelationshipInfoModel, relationship_info)
 
 
 @router.get("/{relationship_info_id}/info", response_model=RelationshipInfoInfo)
 async def get_relationship_info_info(
     request: Request,
     relationship_info_id: PydanticObjectId,
 ) -> RelationshipInfoInfo:
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/relationship_info/controller.py` & `featurebyte-0.3.0/featurebyte/routes/relationship_info/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 RelationshipInfo controller
 """
 from typing import Any, Dict, Literal, Optional
 
 from bson import ObjectId
 
-from featurebyte.models.relationship import RelationshipInfo
+from featurebyte.models.relationship import RelationshipInfoModel
 from featurebyte.routes.common.base import BaseDocumentController
 from featurebyte.schema.relationship_info import (
     RelationshipInfoCreate,
     RelationshipInfoInfo,
     RelationshipInfoList,
 )
 from featurebyte.service.entity import EntityService
 from featurebyte.service.info import InfoService
 from featurebyte.service.relationship_info import RelationshipInfoService
 from featurebyte.service.table import TableService
 
 
 class RelationshipInfoController(
-    BaseDocumentController[RelationshipInfo, RelationshipInfoService, RelationshipInfoList]
+    BaseDocumentController[RelationshipInfoModel, RelationshipInfoService, RelationshipInfoList]
 ):
     """
     RelationshipInfo controller
     """
 
     paginated_document_class = RelationshipInfoList
 
@@ -39,26 +39,26 @@
         self.info_service = info_service
         self.entity_service = entity_service
         self.data_service = data_service
 
     async def create_relationship_info(
         self,
         data: RelationshipInfoCreate,
-    ) -> RelationshipInfo:
+    ) -> RelationshipInfoModel:
         """
         Create RelationshipInfo at persistent
 
         Parameters
         ----------
         data: RelationshipInfoCreate
             RelationshipInfo creation payload
 
         Returns
         -------
-        RelationshipInfo
+        RelationshipInfoModel
             Newly created RelationshipInfo object
         """
         await self._validate_relationship_info_create(data)
         return await self.relationship_info_service.create_document(data)
 
     async def _validate_relationship_info_create(
         self,
```

### Comparing `featurebyte-0.2.2/featurebyte/routes/scd_table/api.py` & `featurebyte-0.3.0/featurebyte/routes/scd_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/scd_table/controller.py` & `featurebyte-0.3.0/featurebyte/routes/scd_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/semantic/api.py` & `featurebyte-0.3.0/featurebyte/routes/semantic/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/semantic/controller.py` & `featurebyte-0.3.0/featurebyte/routes/semantic/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/table/api.py` & `featurebyte-0.3.0/featurebyte/routes/table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/task/api.py` & `featurebyte-0.3.0/featurebyte/routes/task/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/task/controller.py` & `featurebyte-0.3.0/featurebyte/routes/task/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/temp_data/api.py` & `featurebyte-0.3.0/featurebyte/routes/temp_data/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/routes/temp_data/controller.py` & `featurebyte-0.3.0/featurebyte/routes/temp_data/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/batch_feature_table.py` & `featurebyte-0.3.0/featurebyte/schema/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/batch_request_table.py` & `featurebyte-0.3.0/featurebyte/schema/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/catalog.py` & `featurebyte-0.3.0/featurebyte/schema/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/common/base.py` & `featurebyte-0.3.0/featurebyte/schema/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/common/operation.py` & `featurebyte-0.3.0/featurebyte/schema/common/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/context.py` & `featurebyte-0.3.0/featurebyte/schema/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/credential.py` & `featurebyte-0.3.0/featurebyte/schema/credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         if self.database_credential:
             self.database_credential.encrypt()
         if self.storage_credential:
             self.storage_credential.encrypt()
 
     class Settings(BaseDocumentServiceUpdateSchema.Settings):
         """
-        Unique contraints checking
+        Unique constraints checking
         """
 
         unique_constraints: List[UniqueValuesConstraint] = [
             UniqueValuesConstraint(
                 fields=("_id",),
                 conflict_fields_signature={"id": ["_id"]},
                 resolution_signature=UniqueConstraintResolutionSignature.GET_BY_ID,
```

### Comparing `featurebyte-0.2.2/featurebyte/schema/deployment.py` & `featurebyte-0.3.0/featurebyte/schema/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/dimension_table.py` & `featurebyte-0.3.0/featurebyte/schema/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/entity.py` & `featurebyte-0.3.0/featurebyte/schema/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/event_table.py` & `featurebyte-0.3.0/featurebyte/schema/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/feature_job_setting_analysis.py` & `featurebyte-0.3.0/featurebyte/schema/feature_job_setting_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -72,30 +72,79 @@
 
     frequency: int
     job_time_modulo_frequency: int
     blind_spot: int
     feature_cutoff_modulo_frequency: int
 
 
+class FeatureJobSettingAnalysisWHJobFrequency(FeatureByteBaseModel):
+    """
+    FeatureJobSettingAnalysisWHJobFrequency Schema
+    """
+
+    best_estimate: int
+    confidence: str
+
+
+class FeatureJobSettingAnalysisWHJobInterval(FeatureByteBaseModel):
+    """
+    FeatureJobSettingAnalysisWHJobInterval Schema
+    """
+
+    avg: float
+    median: float
+    min: float
+    max: float
+
+
+class FeatureJobSettingAnalysisWHJobTimeModuloFrequency(FeatureByteBaseModel):
+    """
+    FeatureJobSettingAnalysisWHJobTimeModuloFrequency Schema
+    """
+
+    starts: int
+    ends: int
+    ends_wo_late: int
+    job_at_end_of_cycle: bool
+
+
+class FeatureJobSettingAnalysisWarehouseRecord(FeatureByteBaseDocumentModel):
+    """
+    FeatureJobSettingAnalysis persistent record with warehouse jobs info
+    """
+
+    job_frequency: FeatureJobSettingAnalysisWHJobFrequency
+    job_interval: FeatureJobSettingAnalysisWHJobInterval
+    job_time_modulo_frequency: FeatureJobSettingAnalysisWHJobTimeModuloFrequency
+    jobs_count: int
+    missing_jobs_count: int
+
+
 class FeatureJobSettingAnalysisRecord(FeatureByteBaseDocumentModel):
     """
     FeatureJobSettingAnalysis persistent record without report
     """
 
     event_table_id: PydanticObjectId
     analysis_options: AnalysisOptions
     recommended_feature_job_setting: FeatureJobSetting
+    stats_on_wh_jobs: FeatureJobSettingAnalysisWarehouseRecord
 
     @root_validator(pre=True)
     @classmethod
     def _extract_recommended_feature_job_setting(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "recommended_feature_job_setting" not in values:
             values["recommended_feature_job_setting"] = values["analysis_result"][
                 "recommended_feature_job_setting"
             ]
+
+        # expose statistics on warehouse jobs
+        if "stats_on_wh_jobs" not in values:
+            values["stats_on_wh_jobs"] = values["analysis_result"]["stats_on_wh_jobs"]
+
         return values
 
 
 class FeatureJobSettingAnalysisList(PaginationMixin):
     """
     Paginated list of Feature Job Setting Analysis
     """
```

### Comparing `featurebyte-0.2.2/featurebyte/schema/feature_list.py` & `featurebyte-0.3.0/featurebyte/schema/feature_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,26 +18,39 @@
 )
 from featurebyte.query_graph.node.validator import construct_unique_name_validator
 from featurebyte.schema.common.base import BaseDocumentServiceUpdateSchema, PaginationMixin
 
 
 class FeatureListCreate(FeatureByteBaseModel):
     """
-    FeatureList Creation schema
+    Feature List Creation schema
     """
 
     id: Optional[PydanticObjectId] = Field(default_factory=ObjectId, alias="_id")
     name: StrictStr
     feature_ids: List[PydanticObjectId] = Field(min_items=1)
+
+
+class FeatureListServiceCreate(FeatureListCreate):
+    """
+    Feature List Service Creation schema
+    """
+
     feature_list_namespace_id: Optional[PydanticObjectId] = Field(default_factory=ObjectId)
 
 
 class FeatureVersionInfo(FeatureByteBaseModel):
     """
-    Feature version info
+    Feature version info.
+
+    Examples
+    --------
+    >>> new_feature_list = feature_list.create_new_version(  # doctest: +SKIP
+    ...   features=[fb.FeatureVersionInfo(name="InvoiceCount_60days", version=new_feature.version)]
+    ... )
     """
 
     __fbautodoc__ = FBAutoDoc(proxy_class="featurebyte.FeatureVersionInfo")
 
     name: str = Field(description="Name of feature namespace.")
     version: VersionIdentifier = Field(description="Feature version.")
```

### Comparing `featurebyte-0.2.2/featurebyte/schema/feature_list_namespace.py` & `featurebyte-0.3.0/featurebyte/schema/feature_list_namespace.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,28 @@
     FeatureListNamespaceModel,
     FeatureListStatus,
     FeatureReadinessDistribution,
 )
 from featurebyte.schema.common.base import BaseDocumentServiceUpdateSchema, PaginationMixin
 
 
+class FeatureListNamespaceModelResponse(FeatureListNamespaceModel):
+    """
+    Extended FeatureListNamespace model
+    """
+
+    primary_entity_ids: List[PydanticObjectId]
+
+
 class FeatureListNamespaceList(PaginationMixin):
     """
     Paginated list of FeatureListNamespace
     """
 
-    data: List[FeatureListNamespaceModel]
+    data: List[FeatureListNamespaceModelResponse]
 
 
 class FeatureListNamespaceUpdate(FeatureByteBaseModel):
     """
     FeatureListNamespace update schema
     """
```

### Comparing `featurebyte-0.2.2/featurebyte/schema/feature_namespace.py` & `featurebyte-0.3.0/featurebyte/schema/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/feature_store.py` & `featurebyte-0.3.0/featurebyte/schema/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/historical_feature_table.py` & `featurebyte-0.3.0/featurebyte/schema/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/info.py` & `featurebyte-0.3.0/featurebyte/schema/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from featurebyte.schema.feature import (
     FeatureBriefInfoList,
     ReadinessComparison,
     TableCleaningOperationComparison,
     TableFeatureJobSettingComparison,
     VersionComparison,
 )
-from featurebyte.schema.feature_job_setting_analysis import AnalysisOptions, AnalysisParameters
+from featurebyte.schema.feature_job_setting_analysis import AnalysisOptions
 from featurebyte.schema.feature_list import ProductionReadyFractionComparison
 
 
 class FeatureStoreInfo(BaseInfo):
     """
     FeatureStore in schema
     """
@@ -298,48 +298,63 @@
         """
         feature_list_project = DictProject(
             rule=("data", ["version", "readiness_distribution", "created_at", "catalog_id"])
         )
         return FeatureListBriefInfoList(__root__=feature_list_project.project(paginated_data))
 
 
-class FeatureListInfo(NamespaceInfo):
+class BaseFeatureListNamespaceInfo(NamespaceInfo):
     """
-    FeatureList info schema
+    BaseFeatureListNamespace info schema
     """
 
     dtype_distribution: List[FeatureTypeFeatureCount]
+    default_feature_list_id: PydanticObjectId
     status: FeatureListStatus
     feature_count: int
-    version: VersionComparison
-    production_ready_fraction: ProductionReadyFractionComparison
-    versions_info: Optional[FeatureListBriefInfoList]
-    deployed: bool
 
 
-class FeatureListNamespaceInfo(NamespaceInfo):
+class FeatureListNamespaceInfo(BaseFeatureListNamespaceInfo):
     """
     FeatureListNamespace info schema
     """
 
-    dtype_distribution: List[FeatureTypeFeatureCount]
-    default_feature_list_id: PydanticObjectId
-    status: FeatureListStatus
-    feature_count: int
+    feature_namespace_ids: List[PydanticObjectId]
+    default_feature_ids: List[PydanticObjectId]
+
+
+class DefaultFeatureFractionComparison(FeatureByteBaseModel):
+    """
+    DefaultFeatureFractionComparison info schema
+    """
+
+    this: float
+    default: float
+
+
+class FeatureListInfo(BaseFeatureListNamespaceInfo):
+    """
+    FeatureList info schema
+    """
+
+    version: VersionComparison
+    production_ready_fraction: ProductionReadyFractionComparison
+    default_feature_fraction: DefaultFeatureFractionComparison
+    versions_info: Optional[FeatureListBriefInfoList]
+    deployed: bool
 
 
 class FeatureJobSettingAnalysisInfo(FeatureByteBaseModel):
     """
     FeatureJobSettingAnalysis info schema
     """
 
     created_at: datetime
     event_table_name: str
     analysis_options: AnalysisOptions
-    analysis_parameters: AnalysisParameters
     recommendation: FeatureJobSetting
     catalog_name: str
 
 
 class CatalogBriefInfo(BaseBriefInfo):
     """
     Catalog brief info schema
```

### Comparing `featurebyte-0.2.2/featurebyte/schema/item_table.py` & `featurebyte-0.3.0/featurebyte/schema/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/materialized_table.py` & `featurebyte-0.3.0/featurebyte/schema/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/observation_table.py` & `featurebyte-0.3.0/featurebyte/schema/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/relationship_info.py` & `featurebyte-0.3.0/featurebyte/schema/relationship_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from datetime import datetime
 
 from bson import ObjectId
 from pydantic import Field, StrictStr
 
 from featurebyte.models.base import FeatureByteBaseModel, PydanticObjectId
-from featurebyte.models.relationship import RelationshipInfo, RelationshipType
+from featurebyte.models.relationship import RelationshipInfoModel, RelationshipType
 from featurebyte.schema.common.base import BaseDocumentServiceUpdateSchema, PaginationMixin
 
 
 class RelationshipInfoCreate(FeatureByteBaseModel):
     """
     Relationship Info Creation Schema
     """
@@ -29,15 +29,15 @@
 
 
 class RelationshipInfoList(PaginationMixin):
     """
     Paginated list of RelationshipInfo
     """
 
-    data: List[RelationshipInfo]
+    data: List[RelationshipInfoModel]
 
 
 class RelationshipInfoUpdate(BaseDocumentServiceUpdateSchema):
     """
     RelationshipInfo update payload schema
     """
```

### Comparing `featurebyte-0.2.2/featurebyte/schema/request_table.py` & `featurebyte-0.3.0/featurebyte/schema/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/scd_table.py` & `featurebyte-0.3.0/featurebyte/schema/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/semantic.py` & `featurebyte-0.3.0/featurebyte/schema/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/table.py` & `featurebyte-0.3.0/featurebyte/schema/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/task.py` & `featurebyte-0.3.0/featurebyte/schema/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/base.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/batch_feature_table.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/batch_request_table.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/deployment_create_update.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/historical_feature_table.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/materialized_table_delete.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/schema/worker/task/observation_table.py` & `featurebyte-0.3.0/featurebyte/schema/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/base_document.py` & `featurebyte-0.3.0/featurebyte/service/base_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/base_service.py` & `featurebyte-0.3.0/featurebyte/service/base_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/base_table_document.py` & `featurebyte-0.3.0/featurebyte/service/base_table_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/batch_feature_table.py` & `featurebyte-0.3.0/featurebyte/service/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/batch_request_table.py` & `featurebyte-0.3.0/featurebyte/service/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/catalog.py` & `featurebyte-0.3.0/featurebyte/service/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/context.py` & `featurebyte-0.3.0/featurebyte/service/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/credential.py` & `featurebyte-0.3.0/featurebyte/service/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/default_version_mode.py` & `featurebyte-0.3.0/featurebyte/service/default_version_mode.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/deploy.py` & `featurebyte-0.3.0/featurebyte/service/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from __future__ import annotations
 
 from typing import Any, Callable, Optional
 
 from bson.objectid import ObjectId
 
-from featurebyte.exception import DocumentUpdateError
+from featurebyte.exception import DocumentCreationError, DocumentError, DocumentUpdateError
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.deployment import DeploymentModel
 from featurebyte.models.feature import FeatureModel, FeatureReadiness
 from featurebyte.models.feature_list import (
     FeatureListModel,
     FeatureListNamespaceModel,
     FeatureListStatus,
@@ -224,31 +224,28 @@
         assert isinstance(feature_list, FeatureListModel)
         await self._update_feature_list_namespace(
             feature_list_namespace_id=feature_list.feature_list_namespace_id,
             feature_list=feature_list,
             return_document=False,
         )
 
-    async def update_feature_list(
+    async def _update_feature_list(
         self,
         feature_list_id: ObjectId,
-        deployed: bool,
         get_credential: Any,
         update_progress: Optional[Callable[[int, str], None]] = None,
         return_document: bool = True,
     ) -> Optional[FeatureListModel]:
         """
         Update deployed status in feature list
 
         Parameters
         ----------
         feature_list_id: ObjectId
             Target feature list ID
-        deployed: bool
-            Target deployed status
         get_credential: Any
             Get credential handler function
         update_progress: Callable[[int, str], None]
             Update progress handler function
         return_document: bool
             Whether to return updated document
 
@@ -260,26 +257,31 @@
         ------
         Exception
             When there is an unexpected error during feature online_enabled status update
         """
         if update_progress:
             update_progress(0, "Start updating feature list")
 
+        list_deployment_results = await self.deployment_service.list_documents(
+            query_filter={"feature_list_id": feature_list_id, "enabled": True}
+        )
+        target_deployed = list_deployment_results["total"] > 0
         document = await self.feature_list_service.get_document(document_id=feature_list_id)
-        if document.deployed != deployed:
-            await self._validate_deployed_operation(document, deployed)
+
+        if document.deployed != target_deployed:
+            await self._validate_deployed_operation(document, target_deployed)
 
             # variables to store feature list's & features' initial state
             original_deployed = document.deployed
             feature_online_enabled_map = {}
 
             try:
                 feature_list = await self.feature_list_service.update_document(
                     document_id=feature_list_id,
-                    data=FeatureListServiceUpdate(deployed=deployed),
+                    data=FeatureListServiceUpdate(deployed=target_deployed),
                     document=document,
                     return_document=True,
                 )
                 assert isinstance(feature_list, FeatureListModel)
 
                 if update_progress:
                     update_progress(20, "Update features")
@@ -359,33 +361,46 @@
             Deployment name
         to_enable_deployment: bool
             Whether to enable deployment
         get_credential: Any
             Get credential handler function
         update_progress: Callable[[int, str], None]
             Update progress handler function
+
+        Raises
+        ------
+        DocumentCreationError, Exception
+            When there is an unexpected error during deployment creation
         """
         feature_list = await self.feature_list_service.get_document(document_id=feature_list_id)
         default_deployment_name = (
             f"Deployment with {feature_list.name}_{feature_list.version.to_str()}"
         )
-        await self.update_feature_list(
-            feature_list_id=feature_list_id,
-            deployed=to_enable_deployment,
-            get_credential=get_credential,
-            update_progress=update_progress,
-        )
-        await self.deployment_service.create_document(
-            data=DeploymentModel(
-                _id=deployment_id,
-                name=deployment_name or default_deployment_name,
+        try:
+            await self.deployment_service.create_document(
+                data=DeploymentModel(
+                    _id=deployment_id,
+                    name=deployment_name or default_deployment_name,
+                    feature_list_id=feature_list_id,
+                    enabled=to_enable_deployment,
+                )
+            )
+            await self._update_feature_list(
                 feature_list_id=feature_list_id,
-                enabled=to_enable_deployment,
+                get_credential=get_credential,
+                update_progress=update_progress,
             )
-        )
+        except Exception as exc:
+            try:
+                await self.deployment_service.delete_document(document_id=deployment_id)
+            except Exception as delete_exc:
+                raise DocumentCreationError("Failed to create deployment") from delete_exc
+            if isinstance(exc, DocumentError):
+                raise exc
+            raise DocumentCreationError("Failed to create deployment") from exc
 
     async def update_deployment(
         self,
         deployment_id: ObjectId,
         enabled: bool,
         get_credential: Any,
         update_progress: Optional[Callable[[int, str], None]] = None,
@@ -399,20 +414,37 @@
             Deployment ID
         enabled: bool
             Enabled status
         get_credential: Any
             Get credential handler function
         update_progress: Callable[[int, str], None]
             Update progress handler function
+
+        Raises
+        ------
+        DocumentUpdateError, Exception
+            When there is an unexpected error during deployment update
         """
         deployment = await self.deployment_service.get_document(document_id=deployment_id)
-        if deployment.enabled != enabled:
-            await self.update_feature_list(
-                feature_list_id=deployment.feature_list_id,
-                deployed=enabled,
-                get_credential=get_credential,
-                update_progress=update_progress,
-            )
-            await self.deployment_service.update_document(
-                document_id=deployment_id,
-                data=DeploymentUpdate(enabled=enabled),
-            )
+        original_enabled = deployment.enabled
+        if original_enabled != enabled:
+            try:
+                await self.deployment_service.update_document(
+                    document_id=deployment_id,
+                    data=DeploymentUpdate(enabled=enabled),
+                )
+                await self._update_feature_list(
+                    feature_list_id=deployment.feature_list_id,
+                    get_credential=get_credential,
+                    update_progress=update_progress,
+                )
+            except Exception as exc:
+                try:
+                    await self.deployment_service.update_document(
+                        document_id=deployment_id,
+                        data=DeploymentUpdate(enabled=original_enabled),
+                    )
+                except Exception as revert_exc:
+                    raise DocumentUpdateError("Failed to update deployment") from revert_exc
+                if isinstance(exc, DocumentError):
+                    raise exc
+                raise DocumentUpdateError("Failed to update deployment") from exc
```

### Comparing `featurebyte-0.2.2/featurebyte/service/dimension_table.py` & `featurebyte-0.3.0/featurebyte/service/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/entity.py` & `featurebyte-0.3.0/featurebyte/service/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/entity_validation.py` & `featurebyte-0.3.0/featurebyte/service/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/event_table.py` & `featurebyte-0.3.0/featurebyte/service/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/feature.py` & `featurebyte-0.3.0/featurebyte/service/feature.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from featurebyte.models.feature import (
     DefaultVersionMode,
     FeatureModel,
     FeatureNamespaceModel,
     FeatureReadiness,
 )
 from featurebyte.persistent import Persistent
+from featurebyte.query_graph.enum import NodeType
 from featurebyte.query_graph.graph import QueryGraph
 from featurebyte.query_graph.model.graph import QueryGraphModel
 from featurebyte.query_graph.transform.sdk_code import SDKCodeExtractor
-from featurebyte.schema.feature import FeatureCreate, FeatureServiceUpdate
+from featurebyte.schema.feature import FeatureServiceCreate, FeatureServiceUpdate
 from featurebyte.schema.feature_namespace import (
     FeatureNamespaceCreate,
     FeatureNamespaceServiceUpdate,
 )
 from featurebyte.service.base_document import BaseDocumentService
 from featurebyte.service.feature_namespace import FeatureNamespaceService
 from featurebyte.service.table import TableService
@@ -67,15 +68,40 @@
             raise DocumentInconsistencyError(
                 f'Feature (name: "{feature.name}") object(s) within the same namespace '
                 f'must have the same "{attr}" value (namespace: {namespace_attr_str}, '
                 f"feature: {version_attr_str})."
             )
 
 
-class FeatureService(BaseDocumentService[FeatureModel, FeatureCreate, FeatureServiceUpdate]):
+def sanitize_query_graph_for_feature_definition(graph: QueryGraphModel) -> QueryGraphModel:
+    """
+    Sanitize the query graph for feature creation
+
+    Parameters
+    ----------
+    graph: QueryGraphModel
+        The query graph
+
+    Returns
+    -------
+    QueryGraphModel
+    """
+    # Since the generated feature definition contains all the settings in manual mode,
+    # we need to sanitize the graph to make sure that the graph is in manual mode.
+    # Otherwise, the generated feature definition & graph hash before and after
+    # feature creation could be different.
+    output = graph.dict()
+    for node in output["nodes"]:
+        if node["type"] == NodeType.GRAPH:
+            if "view_mode" in node["parameters"]["metadata"]:
+                node["parameters"]["metadata"]["view_mode"] = "manual"
+    return QueryGraphModel(**output)
+
+
+class FeatureService(BaseDocumentService[FeatureModel, FeatureServiceCreate, FeatureServiceUpdate]):
     """
     FeatureService class
     """
 
     document_class = FeatureModel
 
     def __init__(self, user: Any, persistent: Persistent, catalog_id: ObjectId):
@@ -88,90 +114,117 @@
         version_name = get_version()
         query_result = await self.list_documents(
             query_filter={"name": name, "version.name": version_name}
         )
         count = query_result["total"]
         return VersionIdentifier(name=version_name, suffix=count or None)
 
-    async def prepare_graph_to_store(self, feature: FeatureModel) -> tuple[QueryGraphModel, str]:
-        """
-        Prepare the graph to store
-
-        Parameters
-        ----------
-        feature: FeatureModel
-            Feature object
-
-        Returns
-        -------
-        Tuple[GraphNode, str]
-            GraphNode object & target node name
-        """
+    async def _prepare_graph_to_store(
+        self, feature: FeatureModel, sanitize_for_definition: bool = False
+    ) -> tuple[QueryGraphModel, str]:
         # reconstruct view graph node to remove unused column cleaning operations
         graph, node_name_map = await self.view_construction_service.construct_graph(
             query_graph=feature.graph,
             target_node=feature.node,
             table_cleaning_operations=[],
         )
         node = graph.get_node_by_name(node_name_map[feature.node_name])
 
         # prune the graph to remove unused nodes
         pruned_graph, pruned_node_name_map = QueryGraph(**graph.dict(by_alias=True)).prune(
             target_node=node, aggressive=True
         )
+        if sanitize_for_definition:
+            pruned_graph = sanitize_query_graph_for_feature_definition(graph=pruned_graph)
         return pruned_graph, pruned_node_name_map[node.name]
 
-    async def create_document(self, data: FeatureCreate) -> FeatureModel:
+    async def prepare_feature_model(
+        self, data: FeatureServiceCreate, sanitize_for_definition: bool
+    ) -> FeatureModel:
+        """
+        Prepare the feature model by pruning the query graph
+
+        Parameters
+        ----------
+        data: FeatureServiceCreate
+            Feature creation data
+        sanitize_for_definition: bool
+            Whether to sanitize the query graph for generating feature definition
+
+        Returns
+        -------
+        FeatureModel
+        """
         document = FeatureModel(
             **{
                 **data.json_dict(),
                 "readiness": FeatureReadiness.DRAFT,
                 "version": await self._get_feature_version(data.name),
                 "user_id": self.user.id,
                 "catalog_id": self.catalog_id,
             }
         )
 
-        # prepare the raw graph (without getting aggressively pruned) & aggressively pruned graph
-        raw_graph = document.graph
-        graph, node_name = await self.prepare_graph_to_store(feature=document)
-
-        # create a new feature document (so that the derived attributes like table_ids is
-        # generated properly)
-        document = FeatureModel(**{**document.json_dict(), "graph": graph, "node_name": node_name})
+        # prepare the graph to store
+        graph, node_name = await self._prepare_graph_to_store(
+            feature=document, sanitize_for_definition=sanitize_for_definition
+        )
+
+        # create a new feature document (so that the derived attributes like table_ids is generated properly)
+        return FeatureModel(**{**document.json_dict(), "graph": graph, "node_name": node_name})
+
+    async def prepare_feature_definition(self, document: FeatureModel) -> str:
+        """
+        Prepare the feature definition for the given feature document
+
+        Parameters
+        ----------
+        document: FeatureModel
+            Feature document
+
+        Returns
+        -------
+        str
+        """
+        # check whether table has been saved at persistent storage
+        table_service = TableService(
+            user=self.user, persistent=self.persistent, catalog_id=self.catalog_id
+        )
+        table_id_to_info: Dict[ObjectId, Dict[str, Any]] = {}
+        for table_id in document.table_ids:
+            table = await table_service.get_document(document_id=table_id)
+            table_id_to_info[table_id] = table.dict()
+
+        # create feature definition
+        graph, node_name = document.graph, document.node_name
+        sdk_code_gen_state = SDKCodeExtractor(graph=graph).extract(
+            node=graph.get_node_by_name(node_name),
+            to_use_saved_data=True,
+            table_id_to_info=table_id_to_info,
+            output_id=document.id,
+        )
+        definition = sdk_code_gen_state.code_generator.generate(to_format=True)
+        return definition
 
+    async def create_document(self, data: FeatureServiceCreate) -> FeatureModel:
+        document = await self.prepare_feature_model(data=data, sanitize_for_definition=False)
         async with self.persistent.start_transaction() as session:
             # check any conflict with existing documents
             await self._check_document_unique_constraints(document=document)
 
-            # check whether table has been saved at persistent storage
-            table_service = TableService(
-                user=self.user, persistent=self.persistent, catalog_id=self.catalog_id
-            )
-            table_id_to_info: Dict[ObjectId, Dict[str, Any]] = {}
-            for table_id in document.table_ids:
-                table = await table_service.get_document(document_id=table_id)
-                table_id_to_info[table_id] = table.dict()
-
-            # create feature definition
-            sdk_code_gen_state = SDKCodeExtractor(graph=graph).extract(
-                node=graph.get_node_by_name(node_name),
-                to_use_saved_data=True,
-                table_id_to_info=table_id_to_info,
-            )
-            definition = sdk_code_gen_state.code_generator.generate(to_format=True)
+            # prepare feature definition
+            definition = await self.prepare_feature_definition(document=document)
 
+            # insert the document
             insert_id = await session.insert_one(
                 collection_name=self.collection_name,
                 document={
                     **document.dict(by_alias=True),
-                    "graph": graph.dict(),
-                    "node_name": node_name,
                     "definition": definition,
-                    "raw_graph": raw_graph.dict(),
+                    "raw_graph": data.graph.dict(),
                 },
                 user_id=self.user.id,
             )
             assert insert_id == document.id
 
             feature_namespace_service = FeatureNamespaceService(
                 user=self.user, persistent=self.persistent, catalog_id=self.catalog_id
```

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_job_setting_analysis.py` & `featurebyte-0.3.0/featurebyte/service/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_list.py` & `featurebyte-0.3.0/featurebyte/service/feature_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 """
 FeatureListService class
 """
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from bson.objectid import ObjectId
 
 from featurebyte.common.model_util import get_version
 from featurebyte.exception import DocumentError, DocumentInconsistencyError, DocumentNotFoundError
 from featurebyte.models.base import VersionIdentifier
+from featurebyte.models.entity import EntityModel
 from featurebyte.models.feature import DefaultVersionMode, FeatureModel
-from featurebyte.models.feature_list import FeatureListModel, FeatureListNamespaceModel
+from featurebyte.models.feature_list import (
+    EntityRelationshipInfo,
+    FeatureListModel,
+    FeatureListNamespaceModel,
+)
 from featurebyte.schema.feature import FeatureServiceUpdate
-from featurebyte.schema.feature_list import FeatureListCreate, FeatureListServiceUpdate
+from featurebyte.schema.feature_list import FeatureListServiceCreate, FeatureListServiceUpdate
 from featurebyte.schema.feature_list_namespace import FeatureListNamespaceServiceUpdate
 from featurebyte.service.base_document import BaseDocumentService
+from featurebyte.service.entity import EntityService
 from featurebyte.service.feature import FeatureService
 from featurebyte.service.feature_list_namespace import FeatureListNamespaceService
+from featurebyte.service.relationship_info import RelationshipInfoService
 
 
 async def validate_feature_list_version_and_namespace_consistency(
     feature_list: FeatureListModel,
     feature_list_namespace: FeatureListNamespaceModel,
     feature_service: FeatureService,
 ) -> None:
@@ -58,15 +65,15 @@
         raise DocumentInconsistencyError(
             f'FeatureList (name: "{feature_list.name}") object(s) within the same namespace '
             f"must share the same feature name(s)."
         )
 
 
 class FeatureListService(
-    BaseDocumentService[FeatureListModel, FeatureListCreate, FeatureListServiceUpdate]
+    BaseDocumentService[FeatureListModel, FeatureListServiceCreate, FeatureListServiceUpdate]
 ):
     """
     FeatureListService class
     """
 
     document_class = FeatureListModel
 
@@ -103,14 +110,54 @@
 
         derived_output = {
             "feature_store_id": feature_store_id,
             "features": features,
         }
         return derived_output
 
+    async def _extract_relationships_info(
+        self, features: List[FeatureModel]
+    ) -> List[EntityRelationshipInfo]:
+        relationship_info_service = RelationshipInfoService(
+            user=self.user, persistent=self.persistent, catalog_id=self.catalog_id
+        )
+        entity_service = EntityService(
+            user=self.user, persistent=self.persistent, catalog_id=self.catalog_id
+        )
+        entity_ids = set()
+        for feature in features:
+            entity_ids.update(feature.entity_ids)
+
+        ancestor_entity_ids = set(entity_ids)
+        async for entity_doc in entity_service.list_documents_iterator(
+            query_filter={"_id": {"$in": list(entity_ids)}}
+        ):
+            entity = EntityModel(**entity_doc)
+            ancestor_entity_ids.update(entity.ancestor_ids)
+
+        descendant_entity_ids = set(entity_ids)
+        async for entity_doc in entity_service.list_documents_iterator(
+            query_filter={"ancestor_ids": {"$in": list(entity_ids)}}
+        ):
+            entity = EntityModel(**entity_doc)
+            descendant_entity_ids.add(entity.id)
+
+        relationships_info = [
+            EntityRelationshipInfo(**relationship_info)
+            async for relationship_info in relationship_info_service.list_documents_iterator(
+                query_filter={
+                    "$or": [
+                        {"entity_id": {"$in": list(descendant_entity_ids)}},
+                        {"related_entity_id": {"$in": list(ancestor_entity_ids)}},
+                    ]
+                }
+            )
+        ]
+        return relationships_info
+
     async def _update_features(
         self, features: list[FeatureModel], feature_list_id: ObjectId
     ) -> None:
         feature_service = FeatureService(
             user=self.user, persistent=self.persistent, catalog_id=self.catalog_id
         )
         for feature in features:
@@ -129,39 +176,42 @@
         version_name = get_version()
         query_result = await self.list_documents(
             query_filter={"name": name, "version.name": version_name}
         )
         count = query_result["total"]
         return VersionIdentifier(name=version_name, suffix=count or None)
 
-    async def create_document(self, data: FeatureListCreate) -> FeatureListModel:
+    async def create_document(self, data: FeatureListServiceCreate) -> FeatureListModel:
         # sort feature_ids before saving to persistent storage to ease feature_ids comparison in uniqueness check
         document = FeatureListModel(
             **{
                 **data.json_dict(),
                 "feature_ids": sorted(data.feature_ids),
                 "version": await self._get_feature_list_version(data.name),
                 "user_id": self.user.id,
                 "catalog_id": self.catalog_id,
             }
         )
+        # check any conflict with existing documents
+        await self._check_document_unique_constraints(document=document)
 
-        async with self.persistent.start_transaction() as session:
-            # check any conflict with existing documents
-            await self._check_document_unique_constraints(document=document)
-
-            # check whether the feature(s) in the feature list saved to persistent or not
-            feature_data = await self._extract_feature_data(document)
+        # check whether the feature(s) in the feature list saved to persistent or not
+        feature_data = await self._extract_feature_data(document)
+        relationships_info = await self._extract_relationships_info(feature_data["features"])
 
-            # update document with derived output
-            document = FeatureListModel(
+        # update document with derived output
+        document = FeatureListModel(
+            **{
                 **document.dict(by_alias=True),
-                features=feature_data["features"],
-            )
+                "features": feature_data["features"],
+                "relationships_info": relationships_info,
+            }
+        )
 
+        async with self.persistent.start_transaction() as session:
             insert_id = await session.insert_one(
                 collection_name=self.collection_name,
                 document=document.dict(by_alias=True),
                 user_id=self.user.id,
             )
             assert insert_id == document.id
```

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_list_namespace.py` & `featurebyte-0.3.0/featurebyte/service/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_list_status.py` & `featurebyte-0.3.0/featurebyte/service/feature_list_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_namespace.py` & `featurebyte-0.3.0/featurebyte/service/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_readiness.py` & `featurebyte-0.3.0/featurebyte/service/feature_readiness.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/feature_store.py` & `featurebyte-0.3.0/featurebyte/service/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/info.py` & `featurebyte-0.3.0/featurebyte/service/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from bson.objectid import ObjectId
 
 from featurebyte import TableCleaningOperation
 from featurebyte.models.base import PydanticObjectId
 from featurebyte.models.entity import EntityModel
 from featurebyte.models.feature import FeatureModel
+from featurebyte.models.feature_list import FeatureListModel
 from featurebyte.models.feature_store import TableModel
 from featurebyte.models.relationship_analysis import derive_primary_entity
 from featurebyte.persistent import Persistent
 from featurebyte.query_graph.enum import GraphNodeType
 from featurebyte.query_graph.model.feature_job_setting import (
     FeatureJobSetting,
     TableFeatureJobSetting,
@@ -24,14 +25,15 @@
 from featurebyte.query_graph.node.metadata.operation import GroupOperationStructure
 from featurebyte.schema.feature import FeatureBriefInfoList
 from featurebyte.schema.info import (
     BatchFeatureTableInfo,
     BatchRequestTableInfo,
     CatalogInfo,
     CredentialInfo,
+    DefaultFeatureFractionComparison,
     DeploymentInfo,
     DimensionTableInfo,
     EntityBriefInfoList,
     EntityInfo,
     EventTableInfo,
     FeatureInfo,
     FeatureJobSettingAnalysisInfo,
@@ -679,14 +681,33 @@
             default_version_mode=namespace.default_version_mode,
             default_feature_id=namespace.default_feature_id,
             dtype=namespace.dtype,
             version_count=len(namespace.feature_ids),
             catalog_name=catalog.name,
         )
 
+    @staticmethod
+    def _compute_default_feature_fraction(
+        feature_list: FeatureListModel,
+        default_feature_list: FeatureListModel,
+        feature_list_namespace_info: FeatureListNamespaceInfo,
+    ) -> DefaultFeatureFractionComparison:
+        default_feature_ids = set(feature_list_namespace_info.default_feature_ids)
+        this_count, default_count = 0, 0
+        for feat_id in feature_list.feature_ids:
+            if feat_id in default_feature_ids:
+                this_count += 1
+        for feat_id in default_feature_list.feature_ids:
+            if feat_id in default_feature_ids:
+                default_count += 1
+        return DefaultFeatureFractionComparison(
+            this=this_count / len(feature_list.feature_ids),
+            default=default_count / len(default_feature_list.feature_ids),
+        )
+
     async def get_feature_list_info(self, document_id: ObjectId, verbose: bool) -> FeatureListInfo:
         """
         Get feature list info
 
         Parameters
         ----------
         document_id: ObjectId
@@ -727,14 +748,17 @@
                 if default_feature_list.version
                 else None,
             },
             production_ready_fraction={
                 "this": feature_list.readiness_distribution.derive_production_ready_fraction(),
                 "default": default_feature_list.readiness_distribution.derive_production_ready_fraction(),
             },
+            default_feature_fraction=self._compute_default_feature_fraction(
+                feature_list, default_feature_list, namespace_info
+            ),
             versions_info=versions_info,
             deployed=feature_list.deployed,
         )
 
     def _get_primary_entity_from_entities(self, entities: dict[str, Any]) -> dict[str, Any]:
         """
         Get primary entity from entities data
@@ -792,28 +816,42 @@
         for entity in entities["data"]:
             assert entity["catalog_id"] == catalog.id
             entity["catalog_name"] = catalog.name
         for table in tables["data"]:
             assert table["catalog_id"] == catalog.id
             table["catalog_name"] = catalog.name
 
+        # get default feature ids
+        feat_namespace_to_default_id = {}
+        async for feat_namespace in self.feature_namespace_service.list_documents_iterator(
+            query_filter={"_id": {"$in": namespace.feature_namespace_ids}}
+        ):
+            feat_namespace_to_default_id[feat_namespace["_id"]] = feat_namespace[
+                "default_feature_id"
+            ]
+
         return FeatureListNamespaceInfo(
             name=namespace.name,
             created_at=namespace.created_at,
             updated_at=namespace.updated_at,
             entities=EntityBriefInfoList.from_paginated_data(entities),
             primary_entity=EntityBriefInfoList.from_paginated_data(primary_entity),
             tables=TableBriefInfoList.from_paginated_data(tables),
             default_version_mode=namespace.default_version_mode,
             default_feature_list_id=namespace.default_feature_list_id,
             dtype_distribution=namespace.dtype_distribution,
             version_count=len(namespace.feature_list_ids),
             feature_count=len(namespace.feature_namespace_ids),
             status=namespace.status,
             catalog_name=catalog.name,
+            feature_namespace_ids=namespace.feature_namespace_ids,
+            default_feature_ids=[
+                feat_namespace_to_default_id[feat_namespace_id]
+                for feat_namespace_id in namespace.feature_namespace_ids
+            ],
         )
 
     async def get_feature_job_setting_analysis_info(
         self, document_id: ObjectId, verbose: bool
     ) -> FeatureJobSettingAnalysisInfo:
         """
         Get item table info
```

### Comparing `featurebyte-0.2.2/featurebyte/service/item_table.py` & `featurebyte-0.3.0/featurebyte/service/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/materialized_table.py` & `featurebyte-0.3.0/featurebyte/service/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/mixin.py` & `featurebyte-0.3.0/featurebyte/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/observation_table.py` & `featurebyte-0.3.0/featurebyte/service/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/online_enable.py` & `featurebyte-0.3.0/featurebyte/service/online_enable.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/online_serving.py` & `featurebyte-0.3.0/featurebyte/service/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/parent_serving.py` & `featurebyte-0.3.0/featurebyte/service/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/preview.py` & `featurebyte-0.3.0/featurebyte/service/preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,37 +447,32 @@
         return dataframe_to_json(result)
 
     async def compute_historical_features(
         self,
         observation_set: Union[pd.DataFrame, ObservationTableModel],
         featurelist_get_historical_features: FeatureListGetHistoricalFeatures,
         get_credential: Any,
-        output_table_details: Optional[TableDetails] = None,
+        output_table_details: TableDetails,
         progress_callback: Optional[Callable[[int, str], None]] = None,
-    ) -> Optional[AsyncGenerator[bytes, None]]:
+    ) -> None:
         """
         Get historical features for Feature List
 
         Parameters
         ----------
         observation_set: pd.DataFrame
             Observation set data
         featurelist_get_historical_features: FeatureListGetHistoricalFeatures
             FeatureListGetHistoricalFeatures object
         get_credential: Any
             Get credential handler function
-        output_table_details: Optional[TableDetails]
-            Optional output table details to write the results to
+        output_table_details: TableDetails
+            Table details to write the results to
         progress_callback: Optional[Callable[[int, str], None]]
             Optional progress callback function
-
-        Returns
-        -------
-        AsyncGenerator[bytes, None]
-            Asynchronous bytes generator
         """
         # multiple feature stores not supported
         feature_clusters = featurelist_get_historical_features.feature_clusters
         assert len(feature_clusters) == 1
 
         feature_cluster = feature_clusters[0]
         feature_store = await self.feature_store_service.get_document(
@@ -510,15 +505,15 @@
                 is_feature_list_deployed = False
             else:
                 feature_list = await self.feature_list_service.get_document(feature_list_id)
                 is_feature_list_deployed = feature_list.deployed
         except DocumentNotFoundError:
             is_feature_list_deployed = False
 
-        return await get_historical_features(
+        await get_historical_features(
             session=db_session,
             graph=feature_cluster.graph,
             nodes=feature_cluster.nodes,
             observation_set=observation_set,
             serving_names_mapping=featurelist_get_historical_features.serving_names_mapping,
             source_type=feature_store.type,
             is_feature_list_deployed=is_feature_list_deployed,
@@ -610,15 +605,15 @@
         assert len(feature_clusters) == 1
         feature_cluster = feature_clusters[0]
 
         source_type = feature_cluster.graph.get_input_node(
             feature_cluster.node_names[0]
         ).parameters.feature_store_details.type
 
-        expr = get_historical_features_expr(
+        expr, _ = get_historical_features_expr(
             request_table_name=REQUEST_TABLE_NAME,
             graph=feature_cluster.graph,
             nodes=feature_cluster.nodes,
             request_table_columns=observation_set.columns.tolist(),
             source_type=source_type,
             serving_names_mapping=featurelist_get_historical_features.serving_names_mapping,
         )
```

### Comparing `featurebyte-0.2.2/featurebyte/service/relationship.py` & `featurebyte-0.3.0/featurebyte/service/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/relationship_info.py` & `featurebyte-0.3.0/featurebyte/service/relationship_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Relationship Info Service
 """
 
 from featurebyte.exception import DocumentNotFoundError
 from featurebyte.models.base import PydanticObjectId
-from featurebyte.models.relationship import RelationshipInfo
+from featurebyte.models.relationship import RelationshipInfoModel
 from featurebyte.schema.relationship_info import RelationshipInfoCreate, RelationshipInfoUpdate
 from featurebyte.service.base_document import BaseDocumentService
 
 
 class RelationshipInfoService(
-    BaseDocumentService[RelationshipInfo, RelationshipInfoCreate, RelationshipInfoUpdate]
+    BaseDocumentService[RelationshipInfoModel, RelationshipInfoCreate, RelationshipInfoUpdate]
 ):
     """
     RelationshipInfoService class is responsible for keeping track of the relationship info of various types.
     """
 
-    document_class = RelationshipInfo
+    document_class = RelationshipInfoModel
 
     async def remove_relationship(
         self,
         primary_entity_id: PydanticObjectId,
         related_entity_id: PydanticObjectId,
     ) -> None:
         """
```

### Comparing `featurebyte-0.2.2/featurebyte/service/scd_table.py` & `featurebyte-0.3.0/featurebyte/service/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/semantic.py` & `featurebyte-0.3.0/featurebyte/service/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/session_manager.py` & `featurebyte-0.3.0/featurebyte/service/session_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/session_validator.py` & `featurebyte-0.3.0/featurebyte/service/session_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/table.py` & `featurebyte-0.3.0/featurebyte/service/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/table_columns_info.py` & `featurebyte-0.3.0/featurebyte/service/table_columns_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/table_status.py` & `featurebyte-0.3.0/featurebyte/service/table_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/task_manager.py` & `featurebyte-0.3.0/featurebyte/service/task_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     async def schedule_interval_task(
         self,
         name: str,
         payload: BaseTaskPayload,
         interval: Interval,
         time_modulo_frequency_second: Optional[int] = None,
         start_after: Optional[datetime.datetime] = None,
+        time_limit: Optional[int] = None,
     ) -> ObjectId:
         """
         Schedule task to run periodically
 
         Parameters
         ----------
         name: str
@@ -216,36 +217,45 @@
             Payload to use for scheduled task
         interval: Interval
             Interval specification
         time_modulo_frequency_second: Optional[int]
             Time modulo frequency in seconds
         start_after: Optional[datetime.datetime]
             Start after this time
+        time_limit: Optional[int]
+            Execution time limit in seconds
 
         Returns
         -------
         ObjectId
             PeriodicTask ID
         """
         assert self.user.id == payload.user_id
         if time_modulo_frequency_second:
             last_run_at = datetime.datetime.utcnow()
         else:
             last_run_at = None
 
+        # if time limit is not set default to interval length
+        if not time_limit:
+            time_limit = int(
+                datetime.timedelta(**{str(interval.period): interval.every}).total_seconds()
+            )
+
         periodic_task = PeriodicTask(
             name=name,
             task=payload.task,
             interval=interval,
             args=[],
             kwargs=payload.json_dict(),
             time_modulo_frequency_second=time_modulo_frequency_second,
             start_after=start_after,
             last_run_at=last_run_at,
             queue=payload.queue,
+            soft_time_limit=time_limit,
         )
         periodic_task_service = PeriodicTaskService(
             user=self.user,
             persistent=self.persistent,
             catalog_id=self.catalog_id,
         )
         await periodic_task_service.create_document(data=periodic_task)
@@ -253,42 +263,46 @@
 
     async def schedule_cron_task(
         self,
         name: str,
         payload: BaseTaskPayload,
         crontab: Crontab,
         start_after: Optional[datetime.datetime] = None,
+        time_limit: Optional[int] = None,
     ) -> ObjectId:
         """
         Schedule task to run on cron setting
 
         Parameters
         ----------
         name: str
             Task name
         payload: BaseTaskPayload
             Payload to use for scheduled task
         crontab: Crontab
             Cron specification
         start_after: Optional[datetime.datetime]
             Start after this time
+        time_limit: Optional[int]
+            Execution time limit in seconds
 
         Returns
         -------
         ObjectId
             PeriodicTask ID
         """
         assert self.user.id == payload.user_id
         periodic_task = PeriodicTask(
             name=name,
             task=payload.task,
             crontab=crontab,
             args=[],
             kwargs=payload.json_dict(),
             start_after=start_after,
+            soft_time_limit=time_limit,
         )
         periodic_task_service = PeriodicTaskService(
             user=self.user,
             persistent=self.persistent,
             catalog_id=self.catalog_id,
         )
         await periodic_task_service.create_document(data=periodic_task)
```

### Comparing `featurebyte-0.2.2/featurebyte/service/user_service.py` & `featurebyte-0.3.0/featurebyte/service/user_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/validator/materialized_table_delete.py` & `featurebyte-0.3.0/featurebyte/service/validator/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/validator/production_ready_validator.py` & `featurebyte-0.3.0/featurebyte/service/validator/production_ready_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/version.py` & `featurebyte-0.3.0/featurebyte/service/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 from featurebyte.query_graph.model.feature_job_setting import (
     FeatureJobSetting,
     TableFeatureJobSetting,
 )
 from featurebyte.query_graph.node import Node
 from featurebyte.query_graph.node.cleaning_operation import TableCleaningOperation
 from featurebyte.query_graph.node.generic import GroupByNode
-from featurebyte.schema.feature import FeatureCreate, FeatureNewVersionCreate
-from featurebyte.schema.feature_list import FeatureListCreate, FeatureListNewVersionCreate
+from featurebyte.schema.feature import FeatureNewVersionCreate, FeatureServiceCreate
+from featurebyte.schema.feature_list import FeatureListNewVersionCreate, FeatureListServiceCreate
 from featurebyte.service.base_service import BaseService
 from featurebyte.service.feature import FeatureService
 from featurebyte.service.feature_list import FeatureListService
 from featurebyte.service.feature_list_namespace import FeatureListNamespaceService
 from featurebyte.service.feature_namespace import FeatureNamespaceService
 from featurebyte.service.table import TableService
 from featurebyte.service.view_construction import ViewConstructionService
@@ -261,15 +261,15 @@
         new_feature = await self._create_new_feature_version(
             feature,
             data.table_feature_job_settings,
             data.table_cleaning_operations,
             use_source_settings=False,
         )
         return await self.feature_service.create_document(
-            data=FeatureCreate(**new_feature.dict(by_alias=True))
+            data=FeatureServiceCreate(**new_feature.dict(by_alias=True))
         )
 
     async def create_new_feature_version_using_source_settings(
         self, document_id: ObjectId
     ) -> FeatureModel:
         """
         Create new feature version based on feature job settings & cleaning operation from the source table
@@ -368,9 +368,9 @@
             query_filter={"_id": {"$in": feature_list_namespace.feature_namespace_ids}},
             page_size=0,
         )
         new_feature_list = await self._create_new_feature_list_version(
             feature_list, feature_namespaces["data"], data
         )
         return await self.feature_list_service.create_document(
-            data=FeatureListCreate(**new_feature_list.dict(by_alias=True)),
+            data=FeatureListServiceCreate(**new_feature_list.dict(by_alias=True)),
         )
```

### Comparing `featurebyte-0.2.2/featurebyte/service/view_construction.py` & `featurebyte-0.3.0/featurebyte/service/view_construction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/service/working_schema.py` & `featurebyte-0.3.0/featurebyte/service/working_schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/session/base.py` & `featurebyte-0.3.0/featurebyte/session/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,32 +433,39 @@
         await self.execute_query_long_running(f"{create_command} {table_name} AS {query}")
 
     async def drop_table(
         self,
         table_name: str,
         schema_name: str,
         database_name: str,
+        if_exists: bool = False,
     ) -> None:
         """
         Drop a table
 
         Parameters
         ----------
         table_name : str
             Table name
         schema_name : str
             Schema name
         database_name : str
             Database name
+        if_exists : bool
+            If True, drop the table only if it exists
         """
         fully_qualified_table_name = get_fully_qualified_table_name(
             {"table_name": table_name, "schema_name": schema_name, "database_name": database_name}
         )
         query = sql_to_string(
-            expressions.Drop(this=expressions.Table(this=fully_qualified_table_name), kind="TABLE"),
+            expressions.Drop(
+                this=expressions.Table(this=fully_qualified_table_name),
+                kind="TABLE",
+                exists=if_exists,
+            ),
             source_type=self.source_type,
         )
         await self.execute_query(query)
 
     @property
     @abstractmethod
     def schema_name(self) -> str:
```

### Comparing `featurebyte-0.2.2/featurebyte/session/base_spark.py` & `featurebyte-0.3.0/featurebyte/session/base_spark.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,19 +12,24 @@
 from bson import ObjectId
 from pydantic import PrivateAttr
 
 from featurebyte import StorageType
 from featurebyte.common.path_util import get_package_root
 from featurebyte.enum import DBVarType, InternalName
 from featurebyte.logging import get_logger
-from featurebyte.models.credential import StorageCredential
+from featurebyte.models.credential import (
+    GCSStorageCredential,
+    S3StorageCredential,
+    StorageCredential,
+)
 from featurebyte.session.base import BaseSchemaInitializer, BaseSession, MetadataSchemaInitializer
 from featurebyte.session.simple_storage import (
     FileMode,
     FileSimpleStorage,
+    GCSStorage,
     S3SimpleStorage,
     SimpleStorage,
 )
 
 logger = get_logger(__name__)
 
 
@@ -73,22 +78,45 @@
         # add prefix to compartmentalize assets
         self.storage_url = self.storage_url.rstrip("/")
         self.storage_spark_url = self.storage_spark_url.rstrip("/")
 
         if self.storage_type == StorageType.FILE:
             self._storage = FileSimpleStorage(storage_url=self.storage_url)
         elif self.storage_type == StorageType.S3:
+            if self.storage_credential is None:
+                raise NotImplementedError("Storage credential is required for S3")
+            if not isinstance(self.storage_credential, S3StorageCredential):
+                raise NotImplementedError(
+                    f"Unsupported storage credential for S3: {self.storage_credential.__class__.__name__}"
+                )
             self._storage = S3SimpleStorage(
                 storage_url=self.storage_url,
                 storage_credential=self.storage_credential,
                 region_name=self.region_name,
             )
+        elif self.storage_type == StorageType.GCS:
+            if self.storage_credential is None:
+                raise NotImplementedError("Storage credential is required for GCS")
+            if self.storage_credential is None or not isinstance(
+                self.storage_credential, GCSStorageCredential
+            ):
+                raise NotImplementedError(
+                    f"Unsupported storage credential for GCS: {self.storage_credential.__class__.__name__}"
+                )
+            self._storage = GCSStorage(
+                storage_url=self.storage_url,
+                storage_credential=self.storage_credential,
+            )
         else:
             raise NotImplementedError("Unsupported remote storage type")
 
+    def test_storage_connection(self) -> None:
+        """
+        Test storage connection
+        """
         # test connectivity
         self._storage.test_connection()
 
     def upload_file_to_storage(
         self, local_path: str, remote_path: str, is_binary: bool = True
     ) -> None:
         """
@@ -200,14 +228,17 @@
             except Exception as exc:  # pylint: disable=broad-exception-caught
                 logger.error(f"Exception while deleting temp file {temp_filename}: {exc}")
 
 
 class BaseSparkMetadataSchemaInitializer(MetadataSchemaInitializer):
     """BaseSpark metadata initializer class"""
 
+    def __init__(self, session: BaseSparkSession):
+        super().__init__(session)
+
     def create_metadata_table_queries(self, current_migration_version: int) -> List[str]:
         """Query to create metadata table
 
         Parameters
         ----------
         current_migration_version: int
             Current migration version
@@ -239,15 +270,15 @@
             ),
         ]
 
 
 class BaseSparkSchemaInitializer(BaseSchemaInitializer):
     """BaseSpark schema initializer class"""
 
-    def __init__(self, session: BaseSession):
+    def __init__(self, session: BaseSparkSession):
         super().__init__(session=session)
         self.metadata_schema_initializer = BaseSparkMetadataSchemaInitializer(session)
 
     @property
     def current_working_schema_version(self) -> int:
         return 1
 
@@ -308,30 +339,35 @@
             out.extend(df_result["function"].apply(_function_name_to_identifier))
         return out
 
     async def list_procedures(self) -> list[str]:
         return []
 
     async def register_missing_objects(self) -> None:
+        # check storage connection is working
+        session = cast(BaseSparkSession, self.session)
+        session.test_storage_connection()
+
         # upload jar file to storage
         udf_jar_file_name = os.path.basename(self.udf_jar_local_path)
-        self.session.upload_file_to_storage(  # type: ignore[attr-defined]
+        session.upload_file_to_storage(
             local_path=self.udf_jar_local_path, remote_path=udf_jar_file_name
         )
         await super().register_missing_objects()
 
     async def register_missing_functions(self, functions: list[dict[str, Any]]) -> None:
         await super().register_missing_functions(functions)
         # Note that Spark does not seem to be able to reload the same class until the spark app is restarted.
         # To ensure functionality is updated for a function we should create a new class
         # and re-register the function with the new class
         udf_functions = [
             ("OBJECT_AGG", "com.featurebyte.hive.udf.ObjectAggregate"),
             ("OBJECT_DELETE", "com.featurebyte.hive.udf.ObjectDelete"),
             ("F_TIMESTAMP_TO_INDEX", "com.featurebyte.hive.udf.TimestampToIndex"),
+            ("F_INDEX_TO_TIMESTAMP", "com.featurebyte.hive.udf.IndexToTimestamp"),
             (
                 "F_COUNT_DICT_COSINE_SIMILARITY",
                 "com.featurebyte.hive.udf.CountDictCosineSimilarity",
             ),
             ("F_COUNT_DICT_ENTROPY", "com.featurebyte.hive.udf.CountDictEntropy"),
             ("F_COUNT_DICT_MOST_FREQUENT", "com.featurebyte.hive.udf.CountDictMostFrequent"),
             (
```

### Comparing `featurebyte-0.2.2/featurebyte/session/databricks.py` & `featurebyte-0.3.0/featurebyte/session/databricks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 DatabricksSession class
 """
 # pylint: disable=duplicate-code
 from __future__ import annotations
 
-from typing import Any, OrderedDict
+from typing import Any, AsyncGenerator, Dict, OrderedDict
 
 import collections
 import json
 
 import pandas as pd
+import pyarrow as pa
 from pydantic import Field
 
 from featurebyte import AccessTokenCredential
 from featurebyte.enum import DBVarType, SourceType
 from featurebyte.session.base_spark import BaseSparkSession
 
 try:
@@ -21,14 +22,50 @@
     from databricks.sql.exc import ServerOperationError
 
     HAS_DATABRICKS_SQL_CONNECTOR = True
 except ImportError:
     HAS_DATABRICKS_SQL_CONNECTOR = False
 
 
+class ArrowTablePostProcessor:
+    """
+    Post processor for Arrow table to fix databricks return format
+    """
+
+    def __init__(self, schema: Dict[str, str]):
+        self._map_columns = []
+        for col_name, var_type in schema.items():
+            if var_type.upper() == "MAP":
+                self._map_columns.append(col_name)
+
+    def to_dataframe(self, arrow_table: pa.Table) -> pd.DataFrame:
+        """
+        Convert Arrow table to Pandas dataframe
+
+        Parameters
+        ----------
+        arrow_table: pa.Table
+            Arrow table to convert
+
+        Returns
+        -------
+        pd.DataFrame:
+            Pandas dataframe
+        """
+        # handle map type. Databricks returns map as list of tuples
+        # https://docs.databricks.com/sql/language-manual/sql-ref-datatypes.html#map
+        # which is not supported by pyarrow. Below converts the tuple list to json string
+        dataframe = arrow_table.to_pandas()
+        for col_name in self._map_columns:
+            dataframe[col_name] = dataframe[col_name].apply(
+                lambda x: json.dumps(dict(x)) if x is not None else None
+            )
+        return dataframe
+
+
 class DatabricksSession(BaseSparkSession):
     """
     Databricks session class
     """
 
     _no_schema_error = ServerOperationError
 
@@ -105,20 +142,28 @@
 
     def fetch_query_result_impl(self, cursor: Any) -> pd.DataFrame | None:
         schema = None
         if cursor.description:
             schema = {row[0]: row[1] for row in cursor.description}
 
         if schema:
+            post_processor = ArrowTablePostProcessor(schema=schema)
             arrow_table = cursor.fetchall_arrow()
-            dataframe = arrow_table.to_pandas()
-            for col_name in schema:
-                # handle map type. Databricks returns map as list of tuples
-                # https://docs.databricks.com/sql/language-manual/sql-ref-datatypes.html#map
-                # which is not supported by pyarrow. Below converts the tuple list to json string
-                if schema[col_name].upper() == "MAP":
-                    dataframe[col_name] = dataframe[col_name].apply(
-                        lambda x: json.dumps(dict(x)) if x is not None else None
-                    )
-            return dataframe
+            return post_processor.to_dataframe(arrow_table)
 
         return None
+
+    async def fetch_query_stream_impl(self, cursor: Any) -> AsyncGenerator[pa.RecordBatch, None]:
+        schema = None
+        if cursor.description:
+            schema = {row[0]: row[1] for row in cursor.description}
+
+        if schema:
+            post_processor = ArrowTablePostProcessor(schema=schema)
+            # fetch results in batches
+            while True:
+                dataframe = post_processor.to_dataframe(cursor.fetchmany_arrow(size=1000))
+                arrow_table = pa.Table.from_pandas(dataframe)
+                if arrow_table.num_rows == 0:
+                    break
+                for record_batch in arrow_table.to_batches():
+                    yield record_batch
```

### Comparing `featurebyte-0.2.2/featurebyte/session/hive.py` & `featurebyte-0.3.0/featurebyte/session/hive.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/session/manager.py` & `featurebyte-0.3.0/featurebyte/session/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/session/snowflake.py` & `featurebyte-0.3.0/featurebyte/session/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 from typing import Any, AsyncGenerator, OrderedDict
 
 import collections
 import datetime
 import json
+import logging
 
 import pandas as pd
 import pyarrow as pa
 from pydantic import Field
 from snowflake import connector
 from snowflake.connector.errors import (
     DatabaseError,
@@ -28,14 +29,16 @@
 from featurebyte.models.credential import UsernamePasswordCredential
 from featurebyte.query_graph.sql.common import quoted_identifier
 from featurebyte.session.base import BaseSchemaInitializer, BaseSession
 from featurebyte.session.enum import SnowflakeDataType
 
 logger = get_logger(__name__)
 
+logging.getLogger("snowflake.connector").setLevel(logging.ERROR)
+
 
 class SnowflakeSession(BaseSession):
     """
     Snowflake session class
 
 
     References
```

### Comparing `featurebyte-0.2.2/featurebyte/session/spark.py` & `featurebyte-0.3.0/featurebyte/session/spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/session/sqlite.py` & `featurebyte-0.3.0/featurebyte/session/sqlite.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/base.py` & `featurebyte-0.3.0/featurebyte/sql/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/F_GET_RANK.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/F_GET_RANK.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql` & `featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_REGISTRY.sql` & `featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_REGISTRY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar` & `featurebyte-0.3.0/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 27440 bytes, number of entries: 22
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-May-10 09:28 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/featurebyte/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/featurebyte/hive/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/
--rw-r--r--  2.0 unx      963 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
--rw-r--r--  2.0 unx     2544 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate.class
--rw-r--r--  2.0 unx     3769 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
--rw-r--r--  2.0 unx     5593 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictRank.class
--rw-r--r--  2.0 unx     3869 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
--rw-r--r--  2.0 unx     2923 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictNumUnique.class
--rw-r--r--  2.0 unx     3730 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
--rw-r--r--  2.0 unx     5098 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictUDF.class
--rw-r--r--  2.0 unx     2741 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectDelete.class
--rw-r--r--  2.0 unx     2570 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
--rw-r--r--  2.0 unx     5044 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/TimestampToIndex.class
--rw-r--r--  2.0 unx     3721 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictEntropy.class
--rw-r--r--  2.0 unx     6348 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
--rw-r--r--  2.0 unx     3796 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictMostFrequent.class
--rw-r--r--  2.0 unx     5161 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
--rw-r--r--  2.0 unx     1070 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate$1.class
-22 files, 58965 bytes uncompressed, 23428 bytes compressed:  60.3%
+Zip file size: 29690 bytes, number of entries: 23
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 04:29 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/featurebyte/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/featurebyte/hive/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/
+-rw-r--r--  2.0 unx     2544 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate.class
+-rw-r--r--  2.0 unx     3869 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
+-rw-r--r--  2.0 unx     5593 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictRank.class
+-rw-r--r--  2.0 unx      963 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
+-rw-r--r--  2.0 unx     3769 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
+-rw-r--r--  2.0 unx     2570 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
+-rw-r--r--  2.0 unx     2923 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictNumUnique.class
+-rw-r--r--  2.0 unx     3796 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictMostFrequent.class
+-rw-r--r--  2.0 unx     3721 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictEntropy.class
+-rw-r--r--  2.0 unx     5044 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/TimestampToIndex.class
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate$1.class
+-rw-r--r--  2.0 unx     2741 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectDelete.class
+-rw-r--r--  2.0 unx     5098 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictUDF.class
+-rw-r--r--  2.0 unx     6348 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
+-rw-r--r--  2.0 unx     5565 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/IndexToTimestamp.class
+-rw-r--r--  2.0 unx     3730 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
+-rw-r--r--  2.0 unx     5161 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+23 files, 64530 bytes uncompressed, 25488 bytes compressed:  60.5%
```

#### zipnote «TEMP»/diffoscope_an9zg753_/tmpdauarp_p_.zip

```diff
@@ -12,56 +12,59 @@
 
 Filename: com/featurebyte/hive/
 Comment: 
 
 Filename: com/featurebyte/hive/udf/
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
-Comment: 
-
 Filename: com/featurebyte/hive/udf/ObjectAggregate.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
+Filename: com/featurebyte/hive/udf/CountDictRelativeFrequency.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/CountDictRank.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictRelativeFrequency.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictNumUnique.class
+Filename: com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictMostFrequentValue.class
+Filename: com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictUDF.class
+Filename: com/featurebyte/hive/udf/CountDictNumUnique.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectDelete.class
+Filename: com/featurebyte/hive/udf/CountDictMostFrequent.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
+Filename: com/featurebyte/hive/udf/CountDictEntropy.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/TimestampToIndex.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictEntropy.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$1.class
+Comment: 
+
+Filename: com/featurebyte/hive/udf/ObjectDelete.class
+Comment: 
+
+Filename: com/featurebyte/hive/udf/CountDictUDF.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/CountDictCosineSimilarity.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictMostFrequent.class
+Filename: com/featurebyte/hive/udf/IndexToTimestamp.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+Filename: com/featurebyte/hive/udf/CountDictMostFrequentValue.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$1.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
 Comment: 
 
 Zip file comment:
```

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_common.py` & `featurebyte-0.3.0/featurebyte/sql/tile_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     frequency_minute: int
 
     sql: str
     entity_column_names: List[str]
     value_column_names: List[str]
     value_column_types: List[str]
 
+    class Config:
+        """Model configuration"""
+
+        extra = "forbid"
+
     def __init__(self, session: BaseSession, **kwargs: Any):
         """
         Initialize Tile Operation Instance
 
         Parameters
         ----------
         session: BaseSession
```

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_generate.py` & `featurebyte-0.3.0/featurebyte/sql/tile_generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 Databricks Tile Generate Job Script
 """
 from typing import Optional
 
 import dateutil.parser
 
 from featurebyte.common import date_util
+from featurebyte.enum import InternalName
 from featurebyte.logging import get_logger
 from featurebyte.sql.common import construct_create_table_query, retry_sql
 from featurebyte.sql.tile_common import TileCommon
 from featurebyte.sql.tile_registry import TileRegistry
 
 logger = get_logger(__name__)
 
 
 class TileGenerate(TileCommon):
     """
     Tile Generate script
     """
 
-    tile_start_date_column: str
     tile_type: str
     last_tile_start_str: Optional[str]
-    tile_last_start_date_column: Optional[str]
 
     async def execute(self) -> None:
         """
         Execute tile generate operation
         """
         # pylint: disable=too-many-statements
         tile_table_exist_flag = await self.table_exists(self.tile_id)
@@ -37,23 +36,21 @@
 
         # pylint: disable=duplicate-code
         await TileRegistry(
             session=self._session,
             sql=tile_sql,
             table_name=self.tile_id,
             table_exist=tile_table_exist_flag,
-            tile_start_date_column=self.tile_start_date_column,
             tile_modulo_frequency_second=self.tile_modulo_frequency_second,
             blind_spot_second=self.blind_spot_second,
             frequency_minute=self.frequency_minute,
             entity_column_names=self.entity_column_names,
             value_column_names=self.value_column_names,
             value_column_types=self.value_column_types,
             tile_id=self.tile_id,
-            tile_type=self.tile_type,
             aggregation_id=self.aggregation_id,
         ).execute()
 
         tile_sql = self._construct_tile_sql_with_index()
 
         entity_insert_cols = []
         entity_filter_cols = []
@@ -82,15 +79,14 @@
         logger.debug(f"value_insert_cols_str: {value_insert_cols_str}")
         logger.debug(f"value_update_cols_str: {value_update_cols_str}")
 
         # insert new records and update existing records
         if not tile_table_exist_flag:
             logger.debug(f"creating tile table: {self.tile_id}")
             create_sql = construct_create_table_query(self.tile_id, tile_sql, session=self._session)
-            logger.debug(f"create_sql: {create_sql}")
             await retry_sql(self._session, create_sql)
             logger.debug(f"done creating table: {self.tile_id}")
         else:
             if self.entity_column_names:
                 on_condition_str = f"a.INDEX = b.INDEX AND {entity_filter_cols_str}"
                 insert_str = f"INDEX, {self.entity_column_names_str}, {self.value_column_names_str}, CREATED_AT"
                 values_str = f"b.INDEX, {entity_insert_cols_str}, {value_insert_cols_str}, current_timestamp()"
@@ -122,15 +118,15 @@
 
             logger.debug(f"ind_value: {ind_value}")
 
             update_tile_last_ind_sql = f"""
                 UPDATE TILE_REGISTRY
                     SET
                         LAST_TILE_INDEX_{self.tile_type} = {ind_value},
-                        {self.tile_last_start_date_column}_{self.tile_type} = to_timestamp('{self.last_tile_start_str}')
+                        {InternalName.TILE_LAST_START_DATE}_{self.tile_type} = to_timestamp('{self.last_tile_start_str}')
                 WHERE TILE_ID = '{self.tile_id}'
                 AND AGGREGATION_ID = '{self.aggregation_id}'
             """
             await retry_sql(self._session, update_tile_last_ind_sql)
 
     def _construct_tile_sql_with_index(self) -> str:
         if self.entity_column_names:
@@ -138,17 +134,13 @@
                 f"{self.entity_column_names_str}, {self.value_column_names_str}"
             )
         else:
             entity_and_value_column_names_str = self.value_column_names_str
 
         tile_sql = f"""
             select
-                F_TIMESTAMP_TO_INDEX({self.tile_start_date_column},
-                    {self.tile_modulo_frequency_second},
-                    {self.blind_spot_second},
-                    {self.frequency_minute}
-                ) as index,
+                index,
                 {entity_and_value_column_names_str},
                 current_timestamp() as created_at
             from ({self.sql})
         """
         return tile_sql
```

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_generate_entity_tracking.py` & `featurebyte-0.3.0/featurebyte/sql/tile_generate_entity_tracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Tile Generate entity tracking Job script
 """
 from typing import Any, List
 
+from featurebyte.enum import InternalName
 from featurebyte.logging import get_logger
 from featurebyte.session.base import BaseSession
 from featurebyte.sql.base import BaselSqlModel
 from featurebyte.sql.common import construct_create_table_query, retry_sql
 
 logger = get_logger(__name__)
 
 
 class TileGenerateEntityTracking(BaselSqlModel):
     """
     Tile Generate entity tracking script
     """
 
-    tile_last_start_date_column: str
     entity_column_names: List[str]
     tile_id: str
     entity_table: str
 
     def __init__(self, session: BaseSession, **kwargs: Any):
         """
         Initialize Tile Generate Entity Tracking
@@ -53,36 +53,37 @@
             entity_filter_cols.append(
                 self.quote_column_null_aware_equal(f"a.{quote_element}", f"b.{quote_element}")
             )
 
         escaped_entity_column_names_str = ",".join(escaped_entity_column_names)
 
         # create table or insert new records or update existing records
+        tile_last_start_date_column = InternalName.TILE_LAST_START_DATE
         if not tracking_table_exist_flag:
             create_sql = construct_create_table_query(
                 tracking_table_name, self.entity_table, session=self._session
             )
             await retry_sql(self._session, create_sql)
         else:
             if self.entity_column_names:
                 entity_insert_cols_str = ", ".join(entity_insert_cols)
                 entity_filter_cols_str = " AND ".join(entity_filter_cols)
                 merge_sql = f"""
                     merge into {tracking_table_name} a using ({self.entity_table}) b
                         on {entity_filter_cols_str}
                         when matched then
-                            update set a.{self.tile_last_start_date_column} = b.{self.tile_last_start_date_column}
+                            update set a.{tile_last_start_date_column} = b.{tile_last_start_date_column}
                         when not matched then
-                            insert ({escaped_entity_column_names_str}, {self.tile_last_start_date_column})
-                                values ({entity_insert_cols_str}, b.{self.tile_last_start_date_column})
+                            insert ({escaped_entity_column_names_str}, {tile_last_start_date_column})
+                                values ({entity_insert_cols_str}, b.{tile_last_start_date_column})
                 """
             else:
                 merge_sql = f"""
                     merge into {tracking_table_name} a using ({self.entity_table}) b
                         on true
                         when matched then
-                            update set a.{self.tile_last_start_date_column} = b.{self.tile_last_start_date_column}
+                            update set a.{tile_last_start_date_column} = b.{tile_last_start_date_column}
                         when not matched then
-                            insert ({self.tile_last_start_date_column})
-                                values (b.{self.tile_last_start_date_column})
+                            insert ({tile_last_start_date_column})
+                                values (b.{tile_last_start_date_column})
                 """
             await retry_sql(session=self._session, sql=merge_sql)
```

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_generate_schedule.py` & `featurebyte-0.3.0/featurebyte/sql/tile_generate_schedule.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 class TileGenerateSchedule(TileCommon):
     """
     Tile Generate Schedule script
     """
 
     offline_period_minute: int
-    tile_start_date_column: str
-    tile_last_start_date_column: str
-    tile_start_date_placeholder: str
-    tile_end_date_placeholder: str
     tile_type: str
     monitor_periods: int
     job_schedule_ts: Optional[str] = Field(default=None)
 
     # pylint: disable=too-many-locals,too-many-statements
     async def execute(self) -> None:
         """
@@ -120,21 +116,23 @@
         logger.debug(insert_sql)
         await retry_sql(self._session, insert_sql)
 
         monitor_end_ts = tile_end_ts - timedelta(minutes=self.frequency_minute)
         monitor_tile_end_ts_str = monitor_end_ts.strftime(date_format)
 
         monitor_input_sql = self.sql.replace(
-            f"{self.tile_start_date_placeholder}", "'" + monitor_tile_start_ts_str + "'"
-        ).replace(f"{self.tile_end_date_placeholder}", "'" + monitor_tile_end_ts_str + "'")
+            f"{InternalName.TILE_START_DATE_SQL_PLACEHOLDER}", "'" + monitor_tile_start_ts_str + "'"
+        ).replace(
+            f"{InternalName.TILE_END_DATE_SQL_PLACEHOLDER}", "'" + monitor_tile_end_ts_str + "'"
+        )
 
         tile_end_ts_str = tile_end_ts.strftime(date_format)
         generate_input_sql = self.sql.replace(
-            f"{self.tile_start_date_placeholder}", "'" + tile_start_ts_str + "'"
-        ).replace(f"{self.tile_end_date_placeholder}", "'" + tile_end_ts_str + "'")
+            f"{InternalName.TILE_START_DATE_SQL_PLACEHOLDER}", "'" + tile_start_ts_str + "'"
+        ).replace(f"{InternalName.TILE_END_DATE_SQL_PLACEHOLDER}", "'" + tile_end_ts_str + "'")
 
         logger.info(
             "Tile Schedule information",
             extra={
                 "tile_id": tile_id,
                 "tile_start_ts_str": tile_start_ts_str,
                 "tile_end_ts_str": tile_end_ts_str,
@@ -150,32 +148,29 @@
             frequency_minute=self.frequency_minute,
             sql=generate_input_sql,
             monitor_sql=monitor_input_sql,
             entity_column_names=self.entity_column_names,
             value_column_names=self.value_column_names,
             value_column_types=self.value_column_types,
             tile_type=self.tile_type,
-            tile_start_date_column=InternalName.TILE_START_DATE,
             aggregation_id=self.aggregation_id,
         )
 
         tile_generate_ins = TileGenerate(
             session=self._session,
             tile_id=tile_id,
             tile_modulo_frequency_second=self.tile_modulo_frequency_second,
             blind_spot_second=self.blind_spot_second,
             frequency_minute=self.frequency_minute,
             sql=generate_input_sql,
             entity_column_names=self.entity_column_names,
             value_column_names=self.value_column_names,
             value_column_types=self.value_column_types,
             tile_type=self.tile_type,
-            tile_start_date_column=InternalName.TILE_START_DATE,
             last_tile_start_str=tile_end_ts_str,
-            tile_last_start_date_column=self.tile_last_start_date_column,
             aggregation_id=self.aggregation_id,
         )
 
         tile_online_store_ins = TileScheduleOnlineStore(
             session=self._session,
             aggregation_id=self.aggregation_id,
             job_schedule_ts_str=last_tile_end_ts.strftime(date_format),
```

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_monitor.py` & `featurebyte-0.3.0/featurebyte/sql/tile_monitor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 Tile Monitor Job
 """
+from featurebyte.enum import InternalName
 from featurebyte.logging import get_logger
 from featurebyte.sql.common import construct_create_table_query, retry_sql
 from featurebyte.sql.tile_common import TileCommon
 from featurebyte.sql.tile_registry import TileRegistry
 
 logger = get_logger(__name__)
 
 
 class TileMonitor(TileCommon):
     """
     Tile Monitor script
     """
 
     monitor_sql: str
-    tile_start_date_column: str
     tile_type: str
 
     async def execute(self) -> None:
         """
         Execute tile monitor operation
         """
 
@@ -32,35 +32,33 @@
             tile_sql = self.monitor_sql.replace("'", "''")
 
             await TileRegistry(
                 session=self._session,
                 sql=tile_sql,
                 table_name=self.tile_id,
                 table_exist=True,
-                tile_start_date_column=self.tile_start_date_column,
                 tile_modulo_frequency_second=self.tile_modulo_frequency_second,
                 blind_spot_second=self.blind_spot_second,
                 frequency_minute=self.frequency_minute,
                 entity_column_names=self.entity_column_names,
                 value_column_names=self.value_column_names,
                 value_column_types=self.value_column_types,
                 tile_id=self.tile_id,
-                tile_type=self.tile_type,
                 aggregation_id=self.aggregation_id,
             ).execute()
 
             new_tile_sql = f"""
                 select
-                    {self.tile_start_date_column},
-                    F_TIMESTAMP_TO_INDEX(
-                        {self.tile_start_date_column},
+                    F_INDEX_TO_TIMESTAMP(
+                        INDEX,
                         {self.tile_modulo_frequency_second},
                         {self.blind_spot_second},
                         {self.frequency_minute}
-                    ) as INDEX,
+                    ) as {InternalName.TILE_START_DATE},
+                    INDEX,
                     {self.entity_column_names_str},
                     {self.value_column_names_str}
                 from ({self.monitor_sql})
             """
 
             entity_filter_cols_str = " AND ".join(
                 [
@@ -83,15 +81,15 @@
                     (select
                         a.*,
                         {value_select_cols_str},
                         cast('{self.tile_type}' as string) as TILE_TYPE,
                         DATEADD(
                             SECOND,
                             ({self.blind_spot_second}+{self.frequency_minute}*60),
-                            a.{self.tile_start_date_column}
+                            a.{InternalName.TILE_START_DATE}
                         ) as EXPECTED_CREATED_AT,
                         current_timestamp() as CREATED_AT
                     from
                         ({new_tile_sql}) a left outer join {self.tile_id} b
                     on
                         a.INDEX = b.INDEX AND {entity_filter_cols_str})
                 where {value_filter_cols_str}
@@ -108,23 +106,21 @@
                 await retry_sql(self._session, create_sql)
             else:
                 tile_registry_ins = TileRegistry(
                     session=self._session,
                     sql=tile_sql,
                     table_name=monitor_table_name,
                     table_exist=True,
-                    tile_start_date_column=self.tile_start_date_column,
                     tile_modulo_frequency_second=self.tile_modulo_frequency_second,
                     blind_spot_second=self.blind_spot_second,
                     frequency_minute=self.frequency_minute,
                     entity_column_names=self.entity_column_names,
                     value_column_names=self.value_column_names,
                     value_column_types=self.value_column_types,
                     tile_id=self.tile_id,
-                    tile_type=self.tile_type,
                     aggregation_id=self.aggregation_id,
                 )
                 logger.info("Calling tile_registry.execute")
                 await tile_registry_ins.execute()
                 logger.info("End of calling tile_registry.execute")
 
                 # spark does not support insert with partial columns
@@ -142,25 +138,25 @@
 
                 insert_sql = f"""
                     MERGE into {monitor_table_name} a using ({compare_sql}) b
                         ON a.INDEX = b.INDEX AND a.CREATED_AT = b.CREATED_AT
                     WHEN NOT MATCHED THEN
                         INSERT
                         (
-                            {self.tile_start_date_column},
+                            {InternalName.TILE_START_DATE},
                             INDEX,
                             {self.entity_column_names_str},
                             {self.value_column_names_str},
                             {old_value_insert_cols_str_target},
                             TILE_TYPE,
                             EXPECTED_CREATED_AT,
                             CREATED_AT
                         ) VALUES
                         (
-                            b.{self.tile_start_date_column},
+                            b.{InternalName.TILE_START_DATE},
                             b.INDEX,
                             {entity_column_names_str_src},
                             {value_insert_cols_str},
                             {old_value_insert_cols_str},
                             b.TILE_TYPE,
                             b.EXPECTED_CREATED_AT,
                             b.CREATED_AT
@@ -168,13 +164,13 @@
                 """
                 await retry_sql(session=self._session, sql=insert_sql)
 
             insert_monitor_summary_sql = f"""
                 INSERT INTO TILE_MONITOR_SUMMARY(TILE_ID, TILE_START_DATE, TILE_TYPE, CREATED_AT)
                 SELECT
                     '{self.tile_id}' as TILE_ID,
-                    {self.tile_start_date_column} as TILE_START_DATE,
+                    {InternalName.TILE_START_DATE} as TILE_START_DATE,
                     TILE_TYPE,
                     current_timestamp()
                 FROM ({compare_sql})
             """
             await retry_sql(self._session, insert_monitor_summary_sql)
```

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_registry.py` & `featurebyte-0.3.0/featurebyte/sql/tile_registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/sql/tile_schedule_online_store.py` & `featurebyte-0.3.0/featurebyte/sql/tile_schedule_online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/storage/base.py` & `featurebyte-0.3.0/featurebyte/storage/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/storage/local.py` & `featurebyte-0.3.0/featurebyte/storage/local.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/tile/manager.py` & `featurebyte-0.3.0/featurebyte/tile/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Base Tile class
 """
 from __future__ import annotations
 
 from typing import Any, Callable, List, Optional, Tuple
 
+import time
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 from pydantic import BaseModel, PrivateAttr
 
 from featurebyte.enum import InternalName
@@ -20,15 +21,14 @@
 from featurebyte.sql.tile_generate import TileGenerate
 from featurebyte.sql.tile_generate_entity_tracking import TileGenerateEntityTracking
 from featurebyte.sql.tile_generate_schedule import TileGenerateSchedule
 from featurebyte.sql.tile_schedule_online_store import TileScheduleOnlineStore
 from featurebyte.tile.scheduler import TileScheduler
 from featurebyte.tile.sql_template import tm_retrieve_tile_job_audit_logs
 
-TILE_COMPUTE_PROGRESS_MAX_PERCENT = 90  #  Progress percentage to report at end of tile computation
 logger = get_logger(__name__)
 
 
 class TileManager(BaseModel):
     """
     Base Tile class
     """
@@ -71,27 +71,35 @@
             Optional progress callback function
         """
         num_jobs = len(tile_inputs)
         if progress_callback:
             progress_callback(0, f"0/{num_jobs} completed")
 
         for index, (tile_spec, entity_table) in enumerate(tile_inputs):
+            tic = time.time()
             await self.generate_tiles(
                 tile_spec=tile_spec, tile_type=TileType.OFFLINE, start_ts_str=None, end_ts_str=None
             )
-            logger.debug(f"Done generating tiles for {tile_spec}")
+            logger.debug(
+                "Done generating tiles",
+                extra={"tile_id": tile_spec.tile_id, "duration": time.time() - tic},
+            )
 
+            tic = time.time()
             await self.update_tile_entity_tracker(
                 tile_spec=tile_spec, temp_entity_table=entity_table
             )
-            logger.debug(f"Done update_tile_entity_tracker for {tile_spec}")
+            logger.debug(
+                "Done update_tile_entity_tracker",
+                extra={"tile_id": tile_spec.tile_id, "duration": time.time() - tic},
+            )
 
             if progress_callback:
                 progress_callback(
-                    int(np.floor((index + 1) / num_jobs * TILE_COMPUTE_PROGRESS_MAX_PERCENT)),
+                    int(100 * np.floor((index + 1) / num_jobs)),
                     f"{index+1}/{num_jobs} completed",
                 )
 
     async def tile_job_exists(self, tile_spec: TileSpec) -> bool:
         """
         Get existing tile jobs for the given tile_spec
 
@@ -178,16 +186,14 @@
             blind_spot_second=tile_spec.blind_spot_second,
             frequency_minute=tile_spec.frequency_minute,
             sql=tile_sql,
             entity_column_names=tile_spec.entity_column_names,
             value_column_names=tile_spec.value_column_names,
             value_column_types=tile_spec.value_column_types,
             tile_type=tile_type,
-            tile_start_date_column=InternalName.TILE_START_DATE,
-            tile_last_start_date_column=InternalName.TILE_LAST_START_DATE.value,
             last_tile_start_str=last_tile_start_ts_str,
             aggregation_id=tile_spec.aggregation_id,
         )
         await tile_generate_ins.execute()
 
         return tile_generate_ins.json()
 
@@ -214,15 +220,14 @@
             ]
 
         tile_entity_tracking_ins = TileGenerateEntityTracking(
             session=self._session,
             tile_id=tile_spec.aggregation_id,
             entity_column_names=entity_column_names,
             entity_table=temp_entity_table,
-            tile_last_start_date_column=InternalName.TILE_LAST_START_DATE.value,
         )
 
         await tile_entity_tracking_ins.execute()
 
         return tile_entity_tracking_ins.json()
 
     async def schedule_online_tiles(
@@ -332,18 +337,14 @@
                 frequency_minute=tile_spec.frequency_minute,
                 sql=tile_spec.tile_sql,
                 entity_column_names=tile_spec.entity_column_names,
                 value_column_names=tile_spec.value_column_names,
                 value_column_types=tile_spec.value_column_types,
                 tile_type=tile_type,
                 offline_period_minute=offline_minutes,
-                tile_last_start_date_column=InternalName.TILE_LAST_START_DATE,
-                tile_start_date_column=InternalName.TILE_START_DATE,
-                tile_start_date_placeholder=InternalName.TILE_START_DATE_SQL_PLACEHOLDER,
-                tile_end_date_placeholder=InternalName.TILE_END_DATE_SQL_PLACEHOLDER,
                 monitor_periods=monitor_periods,
                 aggregation_id=tile_spec.aggregation_id,
             )
 
             interval_seconds = (
                 tile_spec.frequency_minute * 60
                 if tile_type == TileType.ONLINE
```

### Comparing `featurebyte-0.2.2/featurebyte/tile/scheduler.py` & `featurebyte-0.3.0/featurebyte/tile/scheduler.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/tile/tile_cache.py` & `featurebyte-0.3.0/featurebyte/tile/tile_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -211,60 +211,62 @@
         Returns
         -------
         list[OnDemandTileComputeRequest]
         """
         unique_tile_infos = self._get_unique_tile_infos(
             graph=graph, nodes=nodes, serving_names_mapping=serving_names_mapping
         )
-        tile_ids_with_tracker = await self._filter_tile_ids_with_tracker(
+        agg_ids_with_tracker = await self._filter_agg_ids_with_tracker(
             list(unique_tile_infos.keys())
         )
-        tile_ids_without_tracker = list(set(unique_tile_infos.keys()) - set(tile_ids_with_tracker))
+        agg_ids_without_tracker = list(set(unique_tile_infos.keys()) - set(agg_ids_with_tracker))
 
         # Construct a temp table and query from it whether each tile has updated cache
         tic = time.time()
         await self._register_working_table(
             unique_tile_infos=unique_tile_infos,
-            tile_ids_with_tracker=tile_ids_with_tracker,
-            tile_ids_no_tracker=tile_ids_without_tracker,
+            agg_ids_with_tracker=agg_ids_with_tracker,
+            agg_ids_no_tracker=agg_ids_without_tracker,
             request_id=request_id,
             request_table_name=request_table_name,
         )
 
-        # Create a validity flag for each tile id
+        # Create a validity flag for each aggregation id
         tile_cache_validity = {}
-        for tile_id in tile_ids_without_tracker:
-            tile_cache_validity[tile_id] = False
-        if tile_ids_with_tracker:
+        for agg_id in agg_ids_without_tracker:
+            tile_cache_validity[agg_id] = False
+        if agg_ids_with_tracker:
             existing_validity = await self._get_tile_cache_validity_from_working_table(
-                request_id=request_id, tile_ids=tile_ids_with_tracker
+                request_id=request_id,
+                agg_ids=agg_ids_with_tracker,
+                unique_tile_infos=unique_tile_infos,
             )
             tile_cache_validity.update(existing_validity)
         elapsed = time.time() - tic
         logger.debug(f"Registering working table and validity check took {elapsed:.2f}s")
 
-        # Construct requests for outdated tile ids
+        # Construct requests for outdated aggregation ids
         requests = []
-        for tile_id, is_cache_valid in tile_cache_validity.items():
+        for agg_id, is_cache_valid in tile_cache_validity.items():
             if is_cache_valid:
-                logger.debug(f"Cache for {tile_id} can be resued")
+                logger.debug(f"Cache for {agg_id} can be resued")
             else:
-                logger.debug(f"Need to recompute cache for {tile_id}")
+                logger.debug(f"Need to recompute cache for {agg_id}")
                 request = self._construct_request_from_working_table(
                     request_id=request_id,
-                    tile_info=unique_tile_infos[tile_id],
+                    tile_info=unique_tile_infos[agg_id],
                 )
                 requests.append(request)
 
         return requests
 
     def _get_unique_tile_infos(
         self, graph: QueryGraph, nodes: list[Node], serving_names_mapping: dict[str, str] | None
     ) -> dict[str, TileGenSql]:
-        """Construct mapping from tile_table_id to TileGenSql for easier manipulation
+        """Construct mapping from aggregation id to TileGenSql for easier manipulation
 
         Parameters
         ----------
         graph : QueryGraph
             Query graph
         nodes : list[Node]
             List of query graph node
@@ -284,21 +286,22 @@
                     if serving_names_mapping is not None:
                         info.serving_names = apply_serving_names_mapping(
                             info.serving_names, serving_names_mapping
                         )
                     out[info.aggregation_id] = info
         return out
 
-    async def _filter_tile_ids_with_tracker(self, tile_ids: list[str]) -> list[str]:
-        """Query tracker tables in data warehouse to identify tile IDs with existing tracking tables
+    async def _filter_agg_ids_with_tracker(self, agg_ids: list[str]) -> list[str]:
+        """Query tracker tables in data warehouse to identify aggregation IDs with existing tracking
+        tables
 
         Parameters
         ----------
-        tile_ids : list[str]
-            List of tile table IDs
+        agg_ids : list[str]
+            List of aggregation IDs
 
         Returns
         -------
         list[str]
             List of tile table IDs with existing entity tracker tables
         """
         all_trackers = set()
@@ -307,137 +310,160 @@
         ):
             # always convert to upper case in case some backends change the casing
             table = table.upper()
             if table.endswith(InternalName.TILE_ENTITY_TRACKER_SUFFIX.value):
                 all_trackers.add(table)
 
         out = []
-        for tile_id in tile_ids:
-            tile_id_tracker_name = self._get_tracker_name_from_tile_id(tile_id)
-            if tile_id_tracker_name in all_trackers:
-                out.append(tile_id)
+        for agg_id in agg_ids:
+            agg_id_tracker_name = self._get_tracker_name_from_agg_id(agg_id)
+            if agg_id_tracker_name in all_trackers:
+                out.append(agg_id)
         return out
 
     @staticmethod
-    def _get_tracker_name_from_tile_id(tile_id: str) -> str:
-        return f"{tile_id}{InternalName.TILE_ENTITY_TRACKER_SUFFIX}".upper()
+    def _get_tracker_name_from_agg_id(agg_id: str) -> str:
+        return f"{agg_id}{InternalName.TILE_ENTITY_TRACKER_SUFFIX}".upper()
 
     async def _register_working_table(
         self,
         unique_tile_infos: dict[str, TileGenSql],
-        tile_ids_with_tracker: list[str],
-        tile_ids_no_tracker: list[str],
+        agg_ids_with_tracker: list[str],
+        agg_ids_no_tracker: list[str],
         request_id: str,
         request_table_name: str,
     ) -> None:
         """Register a temp table from which we can query whether each (POINT_IN_TIME, ENTITY_ID,
-        TILE_ID) pair has updated tile cache: a null value in this table indicates that the pair has
-        outdated tile cache. A non-null value refers to the valid last tile start date registered in
-        the data warehouse's tracking table for that pair.
-
-        Two possible reasons that can cause tile cache to be outdated: 1) tiles were never computed
-        for the entity; or 2) tiles were previously computed for the entity but more recent tiles
-        are required due to the requested point in time.
+        TILE_ID) triplet has updated tile cache:
+
+        * Each column in the table represents a specific aggregation_id
+        * Each value in the table is the date of the last computed tile for historical features
+        * Null value in this table means that tiles were never computed for this specific entity
+
+        We can then query this table to identify which tiles need to be recomputed.
 
         This table has the same number of rows as the request table, and has tile IDs as the
         additional columns. For example,
 
         ---------------------------------------------------------------
-        POINT_IN_TIME  CUST_ID  TILE_ID_1   TILE_ID_2   TILE_ID_3  ...
+        POINT_IN_TIME  CUST_ID  AGG_ID_1    AGG_ID_2    AGG_ID_3   ...
         ---------------------------------------------------------------
-        2022-04-01     C1       null        2022-04-05  2022-04-15
+        2022-04-01     C1       2022-03-01  2022-04-05  2022-04-15
         2022-04-10     C2       2022-04-20  null        2022-04-11
         ---------------------------------------------------------------
 
         The table above indicates that the following tile tables need to be recomputed:
-        - TILE_ID_1 for C1
-        - TILE_ID_2 for C2
+        - AGG_ID_1 for C1 (last tile start date is prior to the point in time)
+        - AGG_ID_2 for C2 (no tile has been computed for this entity)
 
         Parameters
         ----------
         unique_tile_infos : dict[str, TileGenSql]
             Mapping from tile id to TileGenSql
-        tile_ids_with_tracker : list[str]
+        agg_ids_with_tracker : list[str]
             List of tile ids with existing tracker tables
-        tile_ids_no_tracker : list[str]
+        agg_ids_no_tracker : list[str]
             List of tile ids without existing tracker table
         request_id : str
             Request ID
         request_table_name : str
             Name of the request table
         """
         # pylint: disable=too-many-locals
         table_expr = select().from_(f"{request_table_name} AS REQ")
 
         columns = []
-        for table_index, tile_id in enumerate(tile_ids_with_tracker):
-            tile_info = unique_tile_infos[tile_id]
-            point_in_time_epoch_expr = self._get_point_in_time_epoch_expr(in_groupby_context=False)
-            last_tile_start_date_expr = self._get_last_tile_start_date_expr(
-                point_in_time_epoch_expr, tile_info
-            )
-            tracker_table_name = self._get_tracker_name_from_tile_id(tile_id)
+        for table_index, agg_id in enumerate(agg_ids_with_tracker):
+            tile_info = unique_tile_infos[agg_id]
+            tracker_table_name = self._get_tracker_name_from_agg_id(agg_id)
             table_alias = f"T{table_index}"
             join_conditions = []
             for serving_name, key in zip(tile_info.serving_names, tile_info.entity_columns):
                 join_conditions.append(
                     parse_one(
                         f"REQ.{quoted_identifier(serving_name).sql()} <=> {table_alias}.{quoted_identifier(key).sql()}"
                     )
                 )
-            join_conditions.append(
-                expressions.LTE(
-                    this=last_tile_start_date_expr,
-                    expression=expressions.Identifier(
-                        this=f"{table_alias}.{InternalName.TILE_LAST_START_DATE}"
-                    ),
-                )
-            )
+            # Note: join_conditions is empty list if there is no entity column. In this case, there
+            # is only one row in the tracking table and the join condition can be omitted.
             table_expr = table_expr.join(
                 tracker_table_name,
                 join_type="left",
                 join_alias=table_alias,
-                on=expressions.and_(*join_conditions),
+                on=expressions.and_(*join_conditions) if join_conditions else None,
             )
-            columns.append(f"{table_alias}.{InternalName.TILE_LAST_START_DATE} AS {tile_id}")
+            columns.append(f"{table_alias}.{InternalName.TILE_LAST_START_DATE} AS {agg_id}")
 
-        for tile_id in tile_ids_no_tracker:
-            columns.append(f"null AS {tile_id}")
+        for agg_id in agg_ids_no_tracker:
+            columns.append(f"CAST(null AS TIMESTAMP) AS {agg_id}")
 
         table_expr = table_expr.select("REQ.*", *columns)
         table_sql = sql_to_string(table_expr, source_type=self.source_type)
 
         tile_cache_working_table_name = (
             f"{InternalName.TILE_CACHE_WORKING_TABLE.value}_{request_id}"
         )
         await self.session.register_table_with_query(tile_cache_working_table_name, table_sql)
         self._materialized_temp_table_names.add(tile_cache_working_table_name)
 
     async def _get_tile_cache_validity_from_working_table(
-        self, request_id: str, tile_ids: list[str]
+        self,
+        request_id: str,
+        agg_ids: list[str],
+        unique_tile_infos: dict[str, TileGenSql],
     ) -> dict[str, bool]:
         """Get a dictionary indicating whether each tile table has updated enough tiles
 
         Parameters
         ----------
         request_id : str
             Request ID
-        tile_ids : list[str]
-            List of tile ids
+        agg_ids : list[str]
+            List of aggregation ids
+        unique_tile_infos : dict[str, TileGenSql]
+            Mapping from tile id to TileGenSql
 
         Returns
         -------
         dict[str, bool]
             Mapping from tile id to bool (True means the tile id has valid cache)
         """
         # A tile table has valid cache if there is no null value in corresponding column in the
         # working table
         validity_exprs = []
-        for tile_id in tile_ids:
-            expr = f"(COUNT({tile_id}) = COUNT(*)) AS {tile_id}"
+        for agg_id in agg_ids:
+            tile_info = unique_tile_infos[agg_id]
+            point_in_time_epoch_expr = self._get_point_in_time_epoch_expr(in_groupby_context=False)
+            last_tile_start_date_expr = self._get_last_tile_start_date_expr(
+                point_in_time_epoch_expr, tile_info
+            )
+            is_tile_updated = expressions.Sum(
+                this=expressions.Cast(
+                    this=expressions.Case(
+                        ifs=[
+                            expressions.If(
+                                this=expressions.Is(this=agg_id, expression=expressions.Null()),
+                                true=expressions.false(),
+                            ),
+                        ],
+                        default=expressions.LTE(
+                            this=last_tile_start_date_expr,
+                            expression=expressions.Identifier(this=agg_id),
+                        ),
+                    ),
+                    to=expressions.DataType.build("BIGINT"),
+                )
+            )
+            expr = expressions.alias_(
+                expressions.EQ(
+                    this=is_tile_updated, expression=expressions.Count(this=expressions.Star())
+                ),
+                alias=agg_id,
+                quoted=False,
+            )
             validity_exprs.append(expr)
 
         tile_cache_working_table_name = (
             f"{InternalName.TILE_CACHE_WORKING_TABLE.value}_{request_id}"
         )
         tile_cache_validity_sql = (
             select(*validity_exprs).from_(tile_cache_working_table_name)
@@ -463,19 +489,33 @@
         tile_info : TileGenSql
             Tile table information
 
         Returns
         -------
         OnDemandTileComputeRequest
         """
-        tile_id = tile_info.tile_table_id
         aggregation_id = tile_info.aggregation_id
 
         # Filter for rows where tile cache are outdated
-        working_table_filter = f"{aggregation_id} IS NULL"
+        point_in_time_epoch_expr = self._get_point_in_time_epoch_expr(in_groupby_context=False)
+        last_tile_start_date_expr = self._get_last_tile_start_date_expr(
+            point_in_time_epoch_expr, tile_info
+        )
+        working_table_filter = expressions.Case(
+            ifs=[
+                expressions.If(
+                    this=expressions.Is(this=aggregation_id, expression=expressions.Null()),
+                    true=expressions.true(),
+                ),
+            ],
+            default=expressions.GT(
+                this=last_tile_start_date_expr,
+                expression=expressions.Identifier(this=aggregation_id),
+            ),
+        )
 
         # Expressions to inform the date range for tile building
         point_in_time_epoch_expr = self._get_point_in_time_epoch_expr(in_groupby_context=True)
         last_tile_start_date_expr = self._get_last_tile_start_date_expr(
             point_in_time_epoch_expr, tile_info
         )
         start_date_expr, end_date_expr = self._get_tile_start_end_date_expr(
@@ -497,31 +537,31 @@
         entity_table_expr = (
             select(
                 *serving_names_to_keys,
                 expressions.alias_(
                     last_tile_start_date_expr, InternalName.TILE_LAST_START_DATE.value
                 ),
                 expressions.alias_(end_date_expr, InternalName.ENTITY_TABLE_END_DATE.value),
+                expressions.alias_(start_date_expr, InternalName.ENTITY_TABLE_START_DATE.value),
             )
             .from_(tile_cache_working_table_name)
             .where(working_table_filter)
             .group_by(*serving_names)
         )
 
         tile_compute_sql = cast(
             str,
             tile_info.sql_template.render(
                 {
                     InternalName.ENTITY_TABLE_SQL_PLACEHOLDER: entity_table_expr.subquery(),
-                    InternalName.TILE_START_DATE_SQL_PLACEHOLDER: start_date_expr,
                 }
             ),
         )
         request = OnDemandTileComputeRequest(
-            tile_table_id=tile_id,
+            tile_table_id=tile_info.tile_table_id,
             aggregation_id=aggregation_id,
             tracker_sql=sql_to_string(entity_table_expr, source_type=self.source_type),
             tile_compute_sql=tile_compute_sql,
             tile_gen_info=tile_info,
         )
         return request
 
@@ -644,14 +684,15 @@
         Returns
         -------
         Tuple[Expression, Expression]
         """
         previous_job_epoch_expr = self._get_previous_job_epoch_expr(
             point_in_time_epoch_expr, tile_info
         )
+        frequency = make_literal_value(tile_info.frequency)
         blind_spot = make_literal_value(tile_info.blind_spot)
         time_modulo_frequency = make_literal_value(tile_info.time_modulo_frequency)
 
         # TO_TIMESTAMP(PREVIOUS_JOB_EPOCH - BLIND_SPOT)
         end_date_expr = expressions.Anonymous(
             this="TO_TIMESTAMP",
             expressions=[expressions.Sub(this=previous_job_epoch_expr, expression=blind_spot)],
@@ -660,12 +701,35 @@
         # DATEADD(s, TIME_MODULO_FREQUENCY - BLIND_SPOT, CAST('1970-01-01' AS TIMESTAMP))
         tile_boundaries_offset = expressions.Paren(
             this=expressions.Sub(this=time_modulo_frequency, expression=blind_spot)
         )
         tile_boundaries_offset_microsecond = TimedeltaExtractNode.convert_timedelta_unit(
             tile_boundaries_offset, "second", "microsecond"
         )
-        start_date_expr = self.adapter.dateadd_microsecond(
+        frequency_microsecond = TimedeltaExtractNode.convert_timedelta_unit(
+            frequency, "second", "microsecond"
+        )
+        earliest_start_date_expr = self.adapter.dateadd_microsecond(
             tile_boundaries_offset_microsecond,
             cast(Expression, parse_one("CAST('1970-01-01' AS TIMESTAMP)")),
         )
+        # This expression will be evaluated in a group by statement with the entity value as the
+        # group by key. We can use ANY_VALUE because the recorded last tile start date is the same
+        # across all rows within the group.
+        recorded_last_tile_start_date_expr = self.adapter.any_value(
+            expressions.Identifier(this=tile_info.aggregation_id)
+        )
+        start_date_expr = expressions.Case(
+            ifs=[
+                expressions.If(
+                    this=expressions.Is(
+                        this=recorded_last_tile_start_date_expr, expression=expressions.Null()
+                    ),
+                    true=earliest_start_date_expr,
+                )
+            ],
+            default=self.adapter.dateadd_microsecond(
+                frequency_microsecond,
+                recorded_last_tile_start_date_expr,
+            ),
+        )
         return start_date_expr, end_date_expr
```

### Comparing `featurebyte-0.2.2/featurebyte/utils/credential.py` & `featurebyte-0.3.0/featurebyte/utils/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/utils/messaging.py` & `featurebyte-0.3.0/featurebyte/utils/messaging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/utils/persistent.py` & `featurebyte-0.3.0/featurebyte/utils/persistent.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,25 +4,21 @@
 from __future__ import annotations
 
 import os
 
 from featurebyte.persistent.base import Persistent
 from featurebyte.persistent.mongo import MongoDB
 
-PERSISTENT = None
 DATABASE_NAME = os.environ.get("MONGODB_DB", "featurebyte")
 MONGO_URI = os.environ.get("MONGODB_URI", "mongodb://localhost:27021")
 
 
 def get_persistent() -> Persistent:
     """
     Return global Persistent object
 
     Returns
     -------
     Persistent
         Persistent object
     """
-    global PERSISTENT  # pylint: disable=global-statement
-    if not PERSISTENT:
-        PERSISTENT = MongoDB(uri=MONGO_URI, database=DATABASE_NAME)
-    return PERSISTENT
+    return MongoDB(uri=MONGO_URI, database=DATABASE_NAME)
```

### Comparing `featurebyte-0.2.2/featurebyte/utils/storage.py` & `featurebyte-0.3.0/featurebyte/utils/storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/__init__.py` & `featurebyte-0.3.0/featurebyte/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/process_store.py` & `featurebyte-0.3.0/featurebyte/worker/process_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/progress.py` & `featurebyte-0.3.0/featurebyte/worker/progress.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/schedulers.py` & `featurebyte-0.3.0/featurebyte/worker/schedulers.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/base.py` & `featurebyte-0.3.0/featurebyte/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/batch_feature_table.py` & `featurebyte-0.3.0/featurebyte/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/batch_request_table.py` & `featurebyte-0.3.0/featurebyte/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/deployment_create_update.py` & `featurebyte-0.3.0/featurebyte/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.3.0/featurebyte/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/historical_feature_table.py` & `featurebyte-0.3.0/featurebyte/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/materialized_table_delete.py` & `featurebyte-0.3.0/featurebyte/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/observation_table.py` & `featurebyte-0.3.0/featurebyte/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/test_task.py` & `featurebyte-0.3.0/featurebyte/worker/task/test_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task/tile_task.py` & `featurebyte-0.3.0/featurebyte/worker/task/tile_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.2/featurebyte/worker/task_executor.py` & `featurebyte-0.3.0/featurebyte/worker/task_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 This module contains TaskExecutor class
 """
 from __future__ import annotations
 
-from typing import Any, Awaitable
+from typing import Any, Awaitable, Optional
 
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 from threading import Thread
 from uuid import UUID
 
 import gevent
+from celery.exceptions import SoftTimeLimitExceeded
 
+from featurebyte.config import get_home_path
 from featurebyte.enum import WorkerCommand
 from featurebyte.logging import get_logger
 from featurebyte.models.base import User
 from featurebyte.utils.credential import MongoBackedCredentialProvider
 from featurebyte.utils.messaging import Progress
 from featurebyte.utils.persistent import get_persistent
 from featurebyte.utils.storage import get_storage, get_temp_storage
@@ -34,44 +36,58 @@
     loop: AbstractEventLoop
         Event loop to run
     """
     asyncio.set_event_loop(loop)
     loop.run_forever()
 
 
-def run_async(coro: Awaitable[Any]) -> Any:
+def run_async(coro: Awaitable[Any], timeout: Optional[int] = None) -> Any:
     """
     Run async function in both async and non-async context
     Parameters
     ----------
     coro: Coroutine
         Coroutine to run
+    timeout: Optional[int]
+        Timeout in seconds, default to None (no timeout)
 
     Returns
     -------
     Any
         result from function call
+
+    Raises
+    ------
+    SoftTimeLimitExceeded
+        timeout is exceeded
     """
     try:
-        loop = asyncio.get_event_loop()
+        loop = asyncio.get_running_loop()
         logger.debug("Use existing async loop", extra={"loop": loop})
     except RuntimeError:
         loop = asyncio.new_event_loop()
         loop.set_default_executor(ThreadPoolExecutor(max_workers=1000))
         logger.debug("Create new async loop", extra={"loop": loop})
         thread = Thread(target=start_background_loop, args=(loop,), daemon=True)
         thread.start()
 
-    tasks = asyncio.all_tasks()
-    logger.debug("Asyncio tasks", extra={"num_tasks": len(tasks)})
+    logger.debug("Asyncio tasks", extra={"num_tasks": len(asyncio.all_tasks(loop=loop))})
+
+    logger.info("Start task", extra={"timeout": timeout})
     future = asyncio.run_coroutine_threadsafe(coro, loop)
-    event = gevent.event.Event()
-    future.add_done_callback(lambda _: event.set())
-    event.wait()
-    return future.result()
+    try:
+        with gevent.Timeout(seconds=timeout, exception=TimeoutError):
+            event = gevent.event.Event()
+            future.add_done_callback(lambda _: event.set())
+            event.wait()
+            return future.result()
+    except TimeoutError as exc:
+        # try to cancel the job if it has not started
+        future.cancel()
+        raise SoftTimeLimitExceeded(f"Task timed out after {timeout}s") from exc
 
 
 class TaskExecutor:
     """
     TaskExecutor class
     """
 
@@ -86,14 +102,27 @@
             progress=progress,
             get_persistent=get_persistent,
             get_credential=credential_provider.get_credential,
             get_storage=get_storage,
             get_temp_storage=get_temp_storage,
         )
 
+        home_path = get_home_path()
+        if not home_path.exists():
+            home_path.mkdir(parents=True)
+
+        # override config file of the featurebyte-worker
+        config_path = home_path.joinpath("config.yaml")
+        config_path.write_text(
+            "# featurebyte-worker config file\n"
+            "profile:\n"
+            "  - name: worker\n"
+            "    api_url: http://featurebyte-server:8088\n\n"
+        )
+
     async def execute(self) -> Any:
         """
         Execute the task
         """
         await self.task.execute()
 
 
@@ -138,15 +167,17 @@
     payload: Any
         Task payload
 
     Returns
     -------
     Any
     """
-    return run_async(execute_task(self.request.id, **payload))
+    # gevent celery worker pool does not support soft time limit,
+    # so we let "run_async" handle the timeout enforcement
+    return run_async(execute_task(self.request.id, **payload), timeout=self.request.timelimit[1])
 
 
 @celery.task(bind=True)
 def execute_cpu_task(self: Any, **payload: Any) -> Any:
     """
     Execute Celery task
```

### Comparing `featurebyte-0.2.2/pyproject.toml` & `featurebyte-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     "featurebyte/sql/spark/*.jar",
 ]
 keywords = []
 license = "Elastic License 2.0"
 name = "featurebyte"
 readme = "README.md"
 repository = "https://github.com/featurebyte/featurebyte"
-version = "0.2.2"
+version = "0.3.0"
 
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 aiofiles = "^22.1.0"
 aioredis = { version = "^2.0.1", optional = true }
 alive-progress = "^3.1.1"
 asyncache = "^0.3.1"
@@ -108,15 +108,15 @@
 cryptography = "^40.0.2"
 databricks-cli = { version = "^0.17.3", optional = true }
 databricks-sql-connector = { version = "^2.5.0", optional = true }
 fastapi = { version =  "^0.95.1", optional = true }
 featurebyte-freeware = { version = "^0.2.14", optional = true }
 gevent = {version = "^22.10.2", optional = true}
 humanize = "^4.4.0"
-importlib_metadata = { version = "^4.5.0", python = "^3.8"}
+importlib_metadata = { version = "*", python = "^3.8"}
 jinja2 = "^3.1.2"
 lazy-object-proxy = "^1.7.1"
 motor = { version = "^3.0.0", optional = true }
 orjson = "^3.8.3"
 pandas = "^1.5.3"
 pdfkit = { version = "^1.0.0", optional = true }
 pyarrow = "^10"
@@ -126,16 +126,16 @@
 python = ">=3.8,<4.0"
 python-multipart = "^0.0.6"
 python-on-whales = "^0.60.0"
 redis = {version = "^5.0.0b1", optional = true, allow-prereleases = true}
 requests = "^2.27.1"
 rich = "^13.3.4"
 sasl = { version = "^0.3.1", optional = true }
-smart-open = { version = "^6.3.0", optional = true }
-snowflake-connector-python = { version = "^3.0.3", optional = true }
+smart-open = { version = "^6.3.0", extras = ["azure", "gcs"], optional = true }
+snowflake-connector-python = { version = "^3.0.3,!=3.0.4", optional = true }
 sqlglot = "^10.1.3,<10.4"  # SQL generation doesn't match as >10.4 double quotes are missing
 thrift-sasl = { version = "^0.4.3", optional = true }
 typeguard = "^2.13.3"
 typer = "^0.7.0"
 uvicorn = { version = "^0.21.1", extras = ["standard"], optional = true }
 websocket-client = "^1.5.1"
 wheel = "0.40.0"
@@ -160,15 +160,15 @@
 toml-sort = "^0.20.0"
 
 [tool.poetry.group.docs.dependencies]
 docstring-parser = "^0.15"
 humanize = "^4.5.0"
 mkautodoc = "^0.2.0"
 mkdocs = "^1.4.1"
-mkdocs-awesome-pages-plugin = "^2.8.0"
+mkdocs-awesome-pages-plugin = "^2.9.0"
 mkdocs-enumerate-headings-plugin = "^0.5.0"
 mkdocs-gen-files = "^0.4.0"
 mkdocs-git-authors-plugin = "^0.6.5"
 mkdocs-git-revision-date-localized-plugin = "^1.1.0"
 mkdocs-literate-nav = "^0.5.0"
 mkdocs-material = "^8.5.7"
 mkdocs-minify-plugin = "^0.6.1"
```

### Comparing `featurebyte-0.2.2/setup.py` & `featurebyte-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,148 +1,453 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: featurebyte
+Version: 0.3.0
+Summary: Python Library for FeatureOps
+Home-page: https://featurebyte.com
+License: Elastic License 2.0
+Author: FeatureByte
+Author-email: it-admin@featurebyte.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: server
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
+Requires-Dist: aioredis (>=2.0.1,<3.0.0) ; extra == "server"
+Requires-Dist: alive-progress (>=3.1.1,<4.0.0)
+Requires-Dist: asyncache (>=0.3.1,<0.4.0)
+Requires-Dist: black (>=23.3.0,<24.0.0)
+Requires-Dist: boto3 (==1.24.59) ; extra == "server"
+Requires-Dist: cachetools (>=5.2.0,<6.0.0) ; extra == "server"
+Requires-Dist: celery[redis] (>=5.2.6,<6.0.0) ; extra == "server"
+Requires-Dist: celerybeat-mongo (>=0.2.0,<0.3.0) ; extra == "server"
+Requires-Dist: cryptography (>=40.0.2,<41.0.0)
+Requires-Dist: databricks-cli (>=0.17.3,<0.18.0) ; extra == "server"
+Requires-Dist: databricks-sql-connector (>=2.5.0,<3.0.0) ; extra == "server"
+Requires-Dist: fastapi (>=0.95.1,<0.96.0) ; extra == "server"
+Requires-Dist: featurebyte-freeware (>=0.2.14,<0.3.0) ; extra == "server"
+Requires-Dist: gevent (>=22.10.2,<23.0.0) ; extra == "server"
+Requires-Dist: humanize (>=4.4.0,<5.0.0)
+Requires-Dist: importlib_metadata ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: lazy-object-proxy (>=1.7.1,<2.0.0)
+Requires-Dist: motor (>=3.0.0,<4.0.0) ; extra == "server"
+Requires-Dist: orjson (>=3.8.3,<4.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pdfkit (>=1.0.0,<2.0.0) ; extra == "server"
+Requires-Dist: pyarrow (>=10,<11)
+Requires-Dist: pydantic (>=1.9.6,<2.0.0)
+Requires-Dist: pyhive (>=0.6.5,<0.7.0) ; extra == "server"
+Requires-Dist: pymongo (>=4.1.1,<5.0.0)
+Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
+Requires-Dist: python-on-whales (>=0.60.0,<0.61.0)
+Requires-Dist: redis (>=5.0.0b1,<6.0.0) ; extra == "server"
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: sasl (>=0.3.1,<0.4.0) ; extra == "server"
+Requires-Dist: smart-open[azure,gcs] (>=6.3.0,<7.0.0) ; extra == "server"
+Requires-Dist: snowflake-connector-python (>=3.0.3,<4.0.0,!=3.0.4) ; extra == "server"
+Requires-Dist: sqlglot (>=10.1.3,<10.4)
+Requires-Dist: thrift-sasl (>=0.4.3,<0.5.0) ; extra == "server"
+Requires-Dist: typeguard (>=2.13.3,<3.0.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "server"
+Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
+Requires-Dist: wheel (==0.40.0)
+Project-URL: Documentation, https://docs.featurebyte.com
+Project-URL: Repository, https://github.com/featurebyte/featurebyte
+Description-Content-Type: text/markdown
 
-packages = \
-['featurebyte',
- 'featurebyte.api',
- 'featurebyte.api.templates',
- 'featurebyte.api.templates.online_serving',
- 'featurebyte.common',
- 'featurebyte.common.documentation',
- 'featurebyte.common.documentation.markdown_extension',
- 'featurebyte.core',
- 'featurebyte.core.accessor',
- 'featurebyte.datasets',
- 'featurebyte.docker',
- 'featurebyte.feature_manager',
- 'featurebyte.migration',
- 'featurebyte.migration.service',
- 'featurebyte.models',
- 'featurebyte.persistent',
- 'featurebyte.query_graph',
- 'featurebyte.query_graph.graph_node',
- 'featurebyte.query_graph.model',
- 'featurebyte.query_graph.node',
- 'featurebyte.query_graph.node.metadata',
- 'featurebyte.query_graph.sql',
- 'featurebyte.query_graph.sql.aggregator',
- 'featurebyte.query_graph.sql.ast',
- 'featurebyte.query_graph.sql.interpreter',
- 'featurebyte.query_graph.transform',
- 'featurebyte.routes',
- 'featurebyte.routes.batch_feature_table',
- 'featurebyte.routes.batch_request_table',
- 'featurebyte.routes.catalog',
- 'featurebyte.routes.common',
- 'featurebyte.routes.context',
- 'featurebyte.routes.credential',
- 'featurebyte.routes.deployment',
- 'featurebyte.routes.dimension_table',
- 'featurebyte.routes.entity',
- 'featurebyte.routes.event_table',
- 'featurebyte.routes.feature',
- 'featurebyte.routes.feature_job_setting_analysis',
- 'featurebyte.routes.feature_list',
- 'featurebyte.routes.feature_list_namespace',
- 'featurebyte.routes.feature_namespace',
- 'featurebyte.routes.feature_store',
- 'featurebyte.routes.historical_feature_table',
- 'featurebyte.routes.item_table',
- 'featurebyte.routes.observation_table',
- 'featurebyte.routes.periodic_tasks',
- 'featurebyte.routes.relationship_info',
- 'featurebyte.routes.scd_table',
- 'featurebyte.routes.semantic',
- 'featurebyte.routes.table',
- 'featurebyte.routes.task',
- 'featurebyte.routes.temp_data',
- 'featurebyte.schema',
- 'featurebyte.schema.common',
- 'featurebyte.schema.worker',
- 'featurebyte.schema.worker.task',
- 'featurebyte.service',
- 'featurebyte.service.validator',
- 'featurebyte.session',
- 'featurebyte.sql',
- 'featurebyte.sql.spark',
- 'featurebyte.storage',
- 'featurebyte.tile',
- 'featurebyte.utils',
- 'featurebyte.utils.snowflake',
- 'featurebyte.worker',
- 'featurebyte.worker.task']
-
-package_data = \
-{'': ['*'],
- 'featurebyte.query_graph.node.metadata': ['templates/*'],
- 'featurebyte.sql': ['databricks/*', 'snowflake/*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'aiofiles>=22.1.0,<23.0.0',
- 'alive-progress>=3.1.1,<4.0.0',
- 'asyncache>=0.3.1,<0.4.0',
- 'black>=23.3.0,<24.0.0',
- 'cryptography>=40.0.2,<41.0.0',
- 'humanize>=4.4.0,<5.0.0',
- 'jinja2>=3.1.2,<4.0.0',
- 'lazy-object-proxy>=1.7.1,<2.0.0',
- 'orjson>=3.8.3,<4.0.0',
- 'pandas>=1.5.3,<2.0.0',
- 'pyarrow>=10,<11',
- 'pydantic>=1.9.6,<2.0.0',
- 'pymongo>=4.1.1,<5.0.0',
- 'python-multipart>=0.0.6,<0.0.7',
- 'python-on-whales>=0.60.0,<0.61.0',
- 'requests>=2.27.1,<3.0.0',
- 'rich>=13.3.4,<14.0.0',
- 'sqlglot>=10.1.3,<10.4',
- 'typeguard>=2.13.3,<3.0.0',
- 'typer>=0.7.0,<0.8.0',
- 'websocket-client>=1.5.1,<2.0.0',
- 'wheel==0.40.0']
-
-extras_require = \
-{':python_version >= "3.8" and python_version < "4.0"': ['importlib_metadata>=4.5.0,<5.0.0'],
- 'server': ['aioredis>=2.0.1,<3.0.0',
-            'boto3==1.24.59',
-            'cachetools>=5.2.0,<6.0.0',
-            'celery[redis]>=5.2.6,<6.0.0',
-            'celerybeat-mongo>=0.2.0,<0.3.0',
-            'databricks-cli>=0.17.3,<0.18.0',
-            'databricks-sql-connector>=2.5.0,<3.0.0',
-            'fastapi>=0.95.1,<0.96.0',
-            'featurebyte-freeware>=0.2.14,<0.3.0',
-            'gevent>=22.10.2,<23.0.0',
-            'motor>=3.0.0,<4.0.0',
-            'pdfkit>=1.0.0,<2.0.0',
-            'pyhive>=0.6.5,<0.7.0',
-            'redis>=5.0.0b1,<6.0.0',
-            'sasl>=0.3.1,<0.4.0',
-            'smart-open>=6.3.0,<7.0.0',
-            'snowflake-connector-python>=3.0.3,<4.0.0',
-            'thrift-sasl>=0.4.3,<0.5.0',
-            'uvicorn[standard]>=0.21.1,<0.22.0']}
-
-entry_points = \
-{'console_scripts': ['featurebyte = featurebyte.__main__:app']}
-
-setup_kwargs = {
-    'name': 'featurebyte',
-    'version': '0.2.2',
-    'description': 'Python Library for FeatureOps',
-    'long_description': '<h1 align="center"> The modern Feature Engineering & Management platform</h1>\n<div align="center">\n\n[![Build status](https://github.com/featurebyte/featurebyte/workflows/build/badge.svg?branch=main&event=push)](https://github.com/featurebyte/featurebyte/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/featurebyte.svg)](https://pypi.org/project/featurebyte/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/featurebyte/featurebyte/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/featurebyte/featurebyte/blob/main/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/featurebyte/featurebyte/releases)\n[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)\n![Coverage Report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/kchua78/773e2960183c0a6fe24c644d95d71fdb/raw/coverage.json)\n\n</div>\n\nFeatureByte is a **free and source available feature platform** designed to:\n\n* **Create state-of-the-art features, not data pipelines:** Create features for Machine Learning with just a few lines of code. Leave the plumbing and pipelining to FeatureByte. We take care of orchestrating the data ops - whether it’s time-window aggs or backfilling, so you can deliver more value from data.\n* **Improve Accuracy through data:** Use the intuitive feature declaration framework to transform creative ideas into training data in minutes. Ditch the limitations of ad-hoc pipelines for features with much more scale, complexity and freshness.\n* **Streamline machine learning data pipelines:** Get more value from AI. Faster. Deploy and serve features in minutes, instead of weeks or months. Declare features in Python and automatically generate optimized data pipelines — all using tools you love like Jupyter Notebooks.\n\n\n\n\n## Take charge of the entire ML feature lifecycle\n\nFeature Engineering and management doesn’t have to be complicated. Take charge of the entire ML feature lifecycle. With FeatureByte, you can **create, experiment, serve and manage your features in one tool**.\n\n### Create\n- Create and share state-of-the-art ML features effortlessly\n- Search and reuse features to create feature lists tailored to your use case\n\n``` python\n# Get view from catalog\ninvoices = catalog.get_view("INVOICES")\n# Customer average spend over past 5 weeks\nfeatures = invoices.groupby(\n    "CustomerId"\n).aggregate_over(\n    "Amount",\n    method="avg",\n    feature_names=["AvgSpend5w"],\n    fill_value=0,\n    windows=["5w"]\n)\n# Save feature\nfeatures["AvgSpend5w"].save()\n```\n\n### Experiment\n- Immediately access historical features through automated backfilling - let FeatureByte handle the complexity of time-aware SQL\n- Experiment on live data at scale, innovating faster\n- Iterate rapidly with different feature lists to create more accurate models\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Get an observation set from the catalog\nobservation_set = catalog.get_observation_table(\n    "5M rows of active Customers in 2021-2022"\n)\n# Compute training data and\n# store it in the feature store for reuse and audit\ntraining = \\\n    feature_list.compute_historical_feature_table(\n      observation_set,\n      name="Training set to predict purchases next 2w"\n    )\n```\n\n### Serve\n- Deploy AI data pipelines and serve features in minutes\n- Access features with low latency\n- Reduce costs and security risk by performing computations in your existing data platform\n- Ensure data consistency between model training and inferencing\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Create deployment\ndeployment = feature_list.deploy(\n    name="Features for customer purchases next 2w",\n)\n# Activate deployment\ndeployment.enable()\n# Get shell script template for online serving\ndeployment.get_online_serving_code(language="sh")\n```\n\n### Manage\n- Organize feature engineering assets with domain-specific catalogs\n- Centralize cleaning operations and feature job configurations\n- Differentiate features that are prototype versus production ready\n- Create new versions of your features to handle changes in data\n- Keep full lineage of your training data and features in production\n- Monitor the health of feature pipelines centrally\n\n``` python\n# Get table from catalog\nitems_table = catalog.get_table("GROCERYITEMS")\n\n# Discount must not be negative\nitems_table.Discount.update_critical_data_info(\n    cleaning_operations=[\n        fb.MissingValueImputation(\n            imputed_value=0\n        ),\n        fb.ValueBeyondEndpointImputation(\n            type="less_than",\n            end_point=0,\n            imputed_value=0\n        ),\n    ]\n)\n```\n\nGet an [overview of the typical workflow](https://docs.featurebyte.com/latest/about/workflow/) in FeatureByte.\n\n## Get started with Quick-Start and Deep-Dive Tutorials\nDiscover FeatureByte via its tutorials. All you need is to install the FeatureByte SDK.\n\nInstall FeatureByte SDK with pip:\n```shell\npip install featurebyte\n```\n**Note**: To avoid potential conflicts with other packages it is strongly recommended to use a [virtual environment](https://docs.python.org/3/tutorial/venv.html) or a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).\n\nRun the following python code to start the FeatureByte services locally with [Docker](https://docs.docker.com/engine/install/).\n``` python\nimport featurebyte as fb\nfb.playground()\n```\nThis will create a local Spark data warehouse with pre-populated data. Once the environment is ready, you can [download](https://docs.featurebyte.com/latest/get_started/tutorials/overview/#download-tutorials) and run notebooks from the [tutorials](https://docs.featurebyte.com/latest/get_started/tutorials/overview/) section.\n\n## Leverage your data warehouse\n\nFeatureByte is developed to integrate seamlessly with your **Snowflake, Databricks, or Spark** data warehouses, enhancing security and efficiency by bypassing large-scale outbound data transfers. This integration allows feature calculations to be performed within the data warehouse, leveraging scalability, stability, and efficiency.\n\n<div align="center">\n  <img src="https://github.com/featurebyte/featurebyte/blob/main/assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">\n</div>\n\nFeatureByte utilizes your data warehouse as a:\n\n* data source.\n* compute engine to leverage its scalability, stability, and efficiency.\n* storage of partial aggregates (tiles) and precomputed feature values to support feature serving.\n\nMore data warehouses will be supported soon!\n\n## Architecture\n\n![FeatureByte Architecture](https://github.com/featurebyte/featurebyte/blob/main/assets/images/system_architecture.png)\nThe FeatureByte platform comprises the following components:\n- **FeatureByte SDK** (Python Package): Connects to the API service to provide feature authoring and management functionality through python classes and functions.\n- **FeatureByte Service** (Docker Containers):\n  - **API Service**: REST-API service that validates and executes requests, queries data warehouses, and stores data.\n  - **Worker**: Executes asynchronous or scheduled tasks.\n  - **MongoDB**: Store metadata for created assets.\n  - **Redis**: Broker and queue for workers, messenger service for publishing progress updates.\n- **Query Graph Transpiler** (Python Package): Construct data transformation steps as a query graph, which can be transpiled to platform-specific SQL.\n- **Source Tables** (Data Warehouse): Tables used as data sources for feature engineering.\n- **Feature Store** (Data Warehouse): Database that store data used to support feature serving.\n\n## FeatureByte Service Deployment Options\nThe **FeatureByte Service** can be installed in three different modes:\n\n* **Local installation:** The easiest way to get started with the FeatureByte SDK. It is a single-user installation that can be used to prototype features locally with your data warehouse.\n\n\n* **Hosted on a single server:** A light-weight option to support collaboration and job scheduling with limited scalability and availability. Multiple users can connect to the service using the FeatureByte SDK, and deploy features for production.\n\n\n* **High availability installation (coming soon):** The recommended way to run the service in production. Scale to a large number of users and deployed features, and provide highly available services.\n\nThe FeatureByte Service runs on **Docker** for the first two installation modes, and is deployed on a **Kubernetes Cluster** for the high availability installation mode.\n\nRefer to the [installation](https://docs.featurebyte.com/latest/get_started/installation/) section of the documentation for more details.\n\n## FeatureByte SDK\n\nThe FeatureByte Python SDK offers a comprehensive set of objects for feature engineering, simplifying the management and manipulation of tables, entities, views, features, feature lists and other necessary objects for feature serving.\n\n* [**Catalog**](https://docs.featurebyte.com/latest/reference/core/catalog/) objects help you organize your feature engineering assets per domain and maintain clarity and easy access to these assets.\n* [**Entity**](https://docs.featurebyte.com/latest/reference/core/entity/) objects contain metadata on entity types represented or referenced by tables within your data warehouse.\n* [**Table**](https://docs.featurebyte.com/latest/reference/core/table/) objects centralize key metadata about the table type, important columns, default cleaning operations and default feature job configurations.\n* [**View**](https://docs.featurebyte.com/latest/reference/core/view/) objects work like SQL views and are local virtual tables that can be modified and joined to other views to prepare data before feature definition.\n* [**Feature**](https://docs.featurebyte.com/latest/reference/core/feature/) objects contain the logical plan to compute a feature in the form of a feature definition file.\n* [**FeatureList**](https://docs.featurebyte.com/latest/reference/core/feature_list/) objects are collection of Feature objects tailored to meet the needs of a particular use case.\n\nRefer to the [SDK overview](https://docs.featurebyte.com/latest/about/sdk_overview/) for a complete list of the objects supported by the SDK and the SDK reference for more information about each object.\n\n## Feature Creation\n\nThe SDK offers an intuitive declarative framework to create feature objects with different signal types, including timing, regularity, stability, diversity, and similarity in addition to the traditional recency, frequency and monetary types.\n\n### Examples\nFeatures can be as simple as an entity’s attribute:\n\n``` python\ncustomer_view = catalog.get_view("GROCERYCUSTOMER")\n# Extract operating system from BrowserUserAgent column\ncustomer_view["OperatingSystemIsWindows"] = \\\n    customer_view.BrowserUserAgent.str.contains("Windows")\n# Create a feature indicating whether the customer is using Windows\nuses_windows = customer_view.OperatingSystemIsWindows.as_feature("UsesWindows")\n```\n\nFeatures can be more complex such as aggregations over a window:\n\n``` python\ninvoice_view = catalog.get_view("GROCERYINVOICE")\n# Group invoices by the column GroceryCustomerGuid that references the customer entity\ninvoices_by_customer = invoice_view.groupby("GroceryCustomerGuid")\n# Declare features of total spent by customer over the past 7 days and 28 days\ncustomer_purchases = invoices_by_customer.aggregate_over(\n    "Amount",\n    method=fb.AggFunc.SUM,\n    feature_names=["CustomerTotalSpent_7d", "CustomerTotalSpent_28d"],\n    fill_value=0,\n    windows=[\'7d\', \'28d\']\n)\n```\n\nTo capture more complex signals, features can involve a series of joins and aggregates and be derived from multiple features:\n\n``` python\n# Get items and product view from the catalog\nitems_view = catalog.get_view("INVOICEITEMS")\nproduct_view = catalog.get_view("GROCERYPRODUCT")\n# Join product view to items view\nitems_view = items_view.join(product_view)\n# Get Customer purchases across product group over the past 4 weeks\ncustomer_inventory_28d = items_view.groupby(\n    by_keys = "GroceryCustomerGuid", category=”ProductGroup”\n).aggregate_over(\n   "TotalCost",\n    method=fb.AggFunc.SUM,\n    feature_names=["CustomerInventory_28d"],\n    windows=[\'28d\']\n)\n# Get customer view and join it to items view\ncustomer_view = catalog.get_view("GROCERYCUSTOMER")\nitems_view = items_view.join(customer_view)\n# Get Purchases of Customers living in the same state\n# across product group over the past 4 weeks\nstate_inventory_28d = items_view.groupby(\n    by_keys="State", category="ProductGroup"\n).aggregate_over(\n   "TotalCost",\n    method=fb.AggFunc.SUM,\n    feature_names=["StateInventory_28d"],\n    windows=[\'28d\']\n)\n# Create a feature that measures the similarity of a customer purchases\n# and purchases of customers living in the same state\ncustomer_state_similarity_28d = \\\n    customer_inventory_28d["CustomerInventory_28d"].cd.cosine_similarity(\n        state_inventory_28d["StateInventory_28d"]\n    )\n# save the new feature\ncustomer_state_similarity_28d.name = \\\n    "Customer Similarity with purchases in the same state over 28 days"\ncustomer_state_similarity_28d.save()\n```\n\n### Feature Definition\nOnce a feature is defined, you can obtain its feature definition file that is the source of truth and provides an explicit outline of the intended operations of the feature declaration, including those inherited but not explicitly declared by you.\n\n``` python\ncustomer_state_similarity_28d.definition\n```\n\nRefer to the SDK reference for the [Feature](https://docs.featurebyte.com/latest/reference/core/feature/) object for more information.\n\n## Time Travel\n\nGreat Machine Learning models require great training data. Great training data require great features (columns) and great observation data points (rows). Great observation data points are historical data points that replicate the production environment. If predictions are expected to be any time, observation points-in-time should also be any time during a period covering at least one seasonal cycle.\n\nObservation data points are in FeatureByte in the form of observation sets that combine entity values and any past points-in-time you want to learn from.\n\nYou can choose to get training data as a Pandas DataFrame or as a Table in the feature store that contains metadata on how the table was created for reuse or audit.\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Create a new feature list that includes a new feature\ncustomer_state_similarity_28d = catalog.get_feature(\n    "Customer Similarity with purchases in the same state over 28 days"\n)\nnew_feature_list = fb.FeatureList(\n    [feature_list, customer_state_similarity_28d],\n    name="Improved feature list with Customer State similarity"\n)\n# Get an observation set from the catalog\nobservation_set = catalog.get_observation_table(\n    "5M of active Customers in 2021-2022"\n)\n# Compute training data and store it in the feature store for reuse and audit\ntraining_table = new_feature_list.compute_historical_feature_table(\n    observation_set,\n    name="Improved Data to predict purchases next 2w with 2021-2022 history"\n)\n# Download training data as a Pandas DataFrame\ntraining_df = training_table.to_pandas()\n```\n\nRefer to the SDK reference for the [FeatureList](https://docs.featurebyte.com/latest/reference/core/feature_list/), [ObservationTable](https://docs.featurebyte.com/latest/reference/core/observation_table/) and [HistoricalFeatureTable](https://docs.featurebyte.com/latest/reference/core/historical_feature_table/) objects, for more information.\n\n## Deploy when needed\n\nOnce a feature list is deployed, the FeatureByte Service automatically orchestrates the pre-computation of feature values and stores them in an online feature store for online and batch serving.\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Check Feature objects are PRODUCTION_READY.\n# A readiness metric of 100% should be returned.\nprint(feature_list.production_ready_fraction)\n# Create deployment\nmy_deployment = feature_list.deploy(\n    name="Deployment of 200 Features to predict customers purchases amount next 2 weeks",\n)\n# Activate deployment\nmy_deployment.enable()\n```\n\nUse the REST API service to retrieve feature values from the online feature store for online serving or use the SDK to retrieve batch of feature values from the online feature store for batch serving.\n\n### Online Serving\nFor online serving, the Deployment object provides REST API service templates that can be used to serve features. Python or shell script templates for the REST API service are retrieved from the Deployment object.\n\nGet online scoring code as a Python script:\n``` python\ndeployment = catalog.get_deployment(\n    "Deployment of 200 Features to predict customers purchases amount next 2 weeks"\n)\ndeployment.get_online_serving_code(language="python")\n```\n\nGet online scoring code as a Shell script:\n``` python\ndeployment.get_online_serving_code(language="sh")\n```\n\n### Batch Serving\nFor batch serving, the Deployment object is used to retrieve feature values for a batch request table containing entities values.\n\n``` python\nfrom datetime import datetime\nbatch_features = deployment.compute_batch_feature_table(\n    batch_request_table=batch_request_table,\n    batch_feature_table_name=\n        "Data to predict customers purchases next 2 w as of " +\n        datetime.utcnow().strftime(\'%Y-%m-%dT%H:%M:%SZ\')\n)\n# Download batch feature values as a Pandas DataFrame\nbatch_features_df = batch_features.to_pandas()\n```\n\nRefer to the SDK reference for the [Deployment](https://docs.featurebyte.com/latest/reference/core/deployment/), [BatchRequestTable](https://docs.featurebyte.com/latest/reference/core/batch_request_table/) and [BatchFeatureTable](https://docs.featurebyte.com/latest/reference/core/batch_feature_table/) objects, for more information.\n\n\n## Releases\n\nYou can see the list of available releases on the [Change Log](https://github.com/featurebyte/featurebyte/blob/main/CHANGELOG.md) page.\nReleases are versioned using the [Semantic Versions](https://semver.org/) specification.\n\n## License\n\n[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)\n\nThis project is licensed under the terms of the `Elastic License 2.0` license. See [LICENSE](https://github.com/featurebyte/featurebyte/blob/main/LICENSE) for more details.\n\n## Contributing\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)\n\nAll contributions are welcomed. Please adhere to the [Code of Conduct](https://github.com/featurebyte/featurebyte/blob/main/CODE_OF_CONDUCT.md) and read the\n[Developer\'s Guide](https://github.com/featurebyte/featurebyte/blob/main/CONTRIBUTING.md) to get started.\n',
-    'author': 'FeatureByte',
-    'author_email': 'it-admin@featurebyte.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://featurebyte.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+<h1 align="center"> The modern Feature Engineering & Management platform</h1>
+<div align="center">
 
+[![Build status](https://github.com/featurebyte/featurebyte/workflows/build/badge.svg?branch=main&event=push)](https://github.com/featurebyte/featurebyte/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/featurebyte.svg)](https://pypi.org/project/featurebyte/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/featurebyte/featurebyte/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/featurebyte/featurebyte/blob/main/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/featurebyte/featurebyte/releases)
+[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
+![Coverage Report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/kchua78/773e2960183c0a6fe24c644d95d71fdb/raw/coverage.json)
+
+</div>
+
+FeatureByte is a **free and source available feature platform** designed to:
+
+* **Create state-of-the-art features, not data pipelines:** Create features for Machine Learning with just a few lines of code. Leave the plumbing and pipelining to FeatureByte. We take care of orchestrating the data ops - whether it’s time-window aggs or backfilling, so you can deliver more value from data.
+* **Improve Accuracy through data:** Use the intuitive feature declaration framework to transform creative ideas into training data in minutes. Ditch the limitations of ad-hoc pipelines for features with much more scale, complexity and freshness.
+* **Streamline machine learning data pipelines:** Get more value from AI. Faster. Deploy and serve features in minutes, instead of weeks or months. Declare features in Python and automatically generate optimized data pipelines — all using tools you love like Jupyter Notebooks.
+
+
+
+
+## Take charge of the entire ML feature lifecycle
+
+Feature Engineering and management doesn’t have to be complicated. Take charge of the entire ML feature lifecycle. With FeatureByte, you can **create, experiment, serve and manage your features in one tool**.
+
+### Create
+- Create and share state-of-the-art ML features effortlessly
+- Search and reuse features to create feature lists tailored to your use case
+
+``` python
+# Get view from catalog
+invoice_view = catalog.get_view("GROCERYINVOICE")
+# Declare features of total spent by customer in the past 7 and 28 days
+customer_purchases = invoice_view.groupby("GroceryCustomerGuid").aggregate_over(
+    "Amount",
+    method="sum",
+    feature_names=["CustomerTotalSpent_7d", "CustomerTotalSpent_28d"],
+    fill_value=0,
+    windows=['7d', '28d']
+)
+customer_purchases.save()
+```
+
+### Experiment
+- Immediately access historical features through automated backfilling - let FeatureByte handle the complexity of time-aware SQL
+- Experiment on live data at scale, innovating faster
+- Iterate rapidly with different feature lists to create more accurate models
+
+``` python
+# Get feature list from the catalog
+feature_list = catalog.get_feature_list(
+    "200 Features on Active Customers"
+)
+# Get an observation set from the catalog
+observation_set = catalog.get_observation_table(
+    "5M rows of active Customers in 2021-2022"
+)
+# Compute training data and
+# store it in the feature store for reuse and audit
+training = \
+    feature_list.compute_historical_feature_table(
+      observation_set,
+      name="Training set to predict purchases next 2w"
+    )
+```
+
+### Serve
+- Deploy AI data pipelines and serve features in minutes
+- Access features with low latency
+- Reduce costs and security risk by performing computations in your existing data platform
+- Ensure data consistency between model training and inferencing
+
+``` python
+# Get feature list from the catalog
+feature_list = catalog.get_feature_list(
+    "200 Features on Active Customers"
+)
+# Create deployment
+deployment = feature_list.deploy(
+    name="Features for customer purchases next 2w",
+)
+# Activate deployment
+deployment.enable()
+# Get shell script template for online serving
+deployment.get_online_serving_code(language="sh")
+```
+
+### Manage
+- Organize feature engineering assets with domain-specific catalogs
+- Centralize cleaning operations and feature job configurations
+- Differentiate features that are prototype versus production ready
+- Create new versions of your features to handle changes in data
+- Keep full lineage of your training data and features in production
+- Monitor the health of feature pipelines centrally
+
+``` python
+# Get table from catalog
+items_table = catalog.get_table("GROCERYITEMS")
+
+# Discount must not be negative
+items_table.Discount.update_critical_data_info(
+    cleaning_operations=[
+        fb.MissingValueImputation(
+            imputed_value=0
+        ),
+        fb.ValueBeyondEndpointImputation(
+            type="less_than",
+            end_point=0,
+            imputed_value=0
+        ),
+    ]
+)
+```
+
+Get an [overview of the typical workflow](https://docs.featurebyte.com/latest/about/workflow/) in FeatureByte.
+
+## Get started with Quick-Start and Deep-Dive Tutorials
+Discover FeatureByte via its tutorials. All you need is to install the FeatureByte SDK.
+
+Install FeatureByte SDK with pip:
+```shell
+pip install featurebyte
+```
+**Note**: To avoid potential conflicts with other packages it is strongly recommended to use a [virtual environment](https://docs.python.org/3/tutorial/venv.html) or a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).
+
+Run the following python code to start the FeatureByte services locally with [Docker](https://docs.docker.com/engine/install/).
+``` python
+import featurebyte as fb
+fb.playground()
+```
+This will create a local Spark data warehouse with pre-populated data. Once the environment is ready, you can [download](https://docs.featurebyte.com/latest/get_started/tutorials/overview/#download-tutorials) and run notebooks from the [tutorials](https://docs.featurebyte.com/latest/get_started/tutorials/overview/) section.
+
+## Leverage your data warehouse
+
+FeatureByte is developed to integrate seamlessly with your **Snowflake, Databricks, or Spark** data warehouses, enhancing security and efficiency by bypassing large-scale outbound data transfers. This integration allows feature calculations to be performed within the data warehouse, leveraging scalability, stability, and efficiency.
+
+<div align="center">
+  <img src="https://github.com/featurebyte/featurebyte/blob/main/assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">
+</div>
+
+FeatureByte utilizes your data warehouse as a:
+
+* data source.
+* compute engine to leverage its scalability, stability, and efficiency.
+* storage of partial aggregates (tiles) and precomputed feature values to support feature serving.
+
+More data warehouses will be supported soon!
+
+## Architecture
+
+![FeatureByte Architecture](https://github.com/featurebyte/featurebyte/blob/main/assets/images/system_architecture.png)
+The FeatureByte platform comprises the following components:
+- **FeatureByte SDK** (Python Package): Connects to the API service to provide feature authoring and management functionality through python classes and functions.
+- **FeatureByte Service** (Docker Containers):
+  - **API Service**: REST-API service that validates and executes requests, queries data warehouses, and stores data.
+  - **Worker**: Executes asynchronous or scheduled tasks.
+  - **MongoDB**: Store metadata for created assets.
+  - **Redis**: Broker and queue for workers, messenger service for publishing progress updates.
+- **Query Graph Transpiler** (Python Package): Construct data transformation steps as a query graph, which can be transpiled to platform-specific SQL.
+- **Source Tables** (Data Warehouse): Tables used as data sources for feature engineering.
+- **Feature Store** (Data Warehouse): Database that store data used to support feature serving.
+
+## FeatureByte Service Deployment Options
+The **FeatureByte Service** can be installed in three different modes:
+
+* **Local installation:** The easiest way to get started with the FeatureByte SDK. It is a single-user installation that can be used to prototype features locally with your data warehouse.
+
+
+* **Hosted on a single server:** A light-weight option to support collaboration and job scheduling with limited scalability and availability. Multiple users can connect to the service using the FeatureByte SDK, and deploy features for production.
+
+
+* **High availability installation (coming soon):** The recommended way to run the service in production. Scale to a large number of users and deployed features, and provide highly available services.
+
+The FeatureByte Service runs on **Docker** for the first two installation modes, and is deployed on a **Kubernetes Cluster** for the high availability installation mode.
+
+Refer to the [installation](https://docs.featurebyte.com/latest/get_started/installation/) section of the documentation for more details.
+
+## FeatureByte SDK
+
+The FeatureByte Python SDK offers a comprehensive set of objects for feature engineering, simplifying the management and manipulation of tables, entities, views, features, feature lists and other necessary objects for feature serving.
+
+* [**Catalog**](https://docs.featurebyte.com/latest/reference/core/catalog/) objects help you organize your feature engineering assets per domain and maintain clarity and easy access to these assets.
+* [**Entity**](https://docs.featurebyte.com/latest/reference/core/entity/) objects contain metadata on entity types represented or referenced by tables within your data warehouse.
+* [**Table**](https://docs.featurebyte.com/latest/reference/core/table/) objects centralize key metadata about the table type, important columns, default cleaning operations and default feature job configurations.
+* [**View**](https://docs.featurebyte.com/latest/reference/core/view/) objects work like SQL views and are local virtual tables that can be modified and joined to other views to prepare data before feature definition.
+* [**Feature**](https://docs.featurebyte.com/latest/reference/core/feature/) objects contain the logical plan to compute a feature in the form of a feature definition file.
+* [**FeatureList**](https://docs.featurebyte.com/latest/reference/core/feature_list/) objects are collection of Feature objects tailored to meet the needs of a particular use case.
+
+Refer to the [SDK overview](https://docs.featurebyte.com/latest/about/sdk_overview/) for a complete list of the objects supported by the SDK and the SDK reference for more information about each object.
+
+## Feature Creation
+
+The SDK offers an intuitive declarative framework to create feature objects with different signal types, including timing, regularity, stability, diversity, and similarity in addition to the traditional recency, frequency and monetary types.
+
+### Examples
+Features can be as simple as an entity’s attribute:
+
+``` python
+customer_view = catalog.get_view("GROCERYCUSTOMER")
+# Extract operating system from BrowserUserAgent column
+customer_view["OperatingSystemIsWindows"] = \
+    customer_view.BrowserUserAgent.str.contains("Windows")
+# Create a feature indicating whether the customer is using Windows
+uses_windows = customer_view.OperatingSystemIsWindows.as_feature("UsesWindows")
+```
+
+Features can be more complex such as aggregations over a window:
+
+``` python
+invoice_view = catalog.get_view("GROCERYINVOICE")
+# Group invoices by the column GroceryCustomerGuid that references the customer entity
+invoices_by_customer = invoice_view.groupby("GroceryCustomerGuid")
+# Declare features of total spent by customer over the past 7 days and 28 days
+customer_purchases = invoices_by_customer.aggregate_over(
+    "Amount",
+    method=fb.AggFunc.SUM,
+    feature_names=["CustomerTotalSpent_7d", "CustomerTotalSpent_28d"],
+    fill_value=0,
+    windows=['7d', '28d']
+)
+```
+
+To capture more complex signals, features can involve a series of joins and aggregates and be derived from multiple features:
+
+``` python
+# Get items and product view from the catalog
+items_view = catalog.get_view("INVOICEITEMS")
+product_view = catalog.get_view("GROCERYPRODUCT")
+# Join product view to items view
+items_view = items_view.join(product_view)
+# Get Customer purchases across product group in the past 4 weeks
+customer_basket_28d = items_view.groupby(
+    by_keys = "GroceryCustomerGuid", category=”ProductGroup”
+).aggregate_over(
+   "TotalCost",
+    method=fb.AggFunc.SUM,
+    feature_names=["CustomerBasket_28d"],
+    windows=['28d']
+)
+# Get customer view and join it to items view
+customer_view = catalog.get_view("GROCERYCUSTOMER")
+items_view = items_view.join(customer_view)
+# Get Purchases of Customers living in the same state
+# across product group in the past 4 weeks
+state_basket_28d = items_view.groupby(
+    by_keys="State", category="ProductGroup"
+).aggregate_over(
+   "TotalCost",
+    method=fb.AggFunc.SUM,
+    feature_names=["StateBasket_28d"],
+    windows=['28d']
+)
+# Create a feature that measures the similarity of a customer purchases
+# and purchases of customers living in the same state
+customer_state_similarity_28d = \
+    customer_basket_28d["CustomerBasket_28d"].cd.cosine_similarity(
+        state_basket_28d["StateBasket_28d"]
+    )
+# save the new feature
+customer_state_similarity_28d.name = \
+    "Customer Similarity with purchases in the same state over 28 days"
+customer_state_similarity_28d.save()
+```
+
+### Feature Definition
+Once a feature is defined, you can obtain its feature definition file that is the source of truth and provides an explicit outline of the intended operations of the feature declaration, including those inherited but not explicitly declared by you.
+
+``` python
+customer_state_similarity_28d.definition
+```
+
+Refer to the SDK reference for the [Feature](https://docs.featurebyte.com/latest/reference/core/feature/) object for more information.
+
+## Time Travel
+
+Great Machine Learning models require great training data. Great training data require great features (columns) and great observation data points (rows). Great observation data points are historical data points that replicate the production environment. If predictions are expected to be any time, observation points-in-time should also be any time during a period covering at least one seasonal cycle.
+
+Observation data points are in FeatureByte in the form of observation sets that combine entity values and any past points-in-time you want to learn from.
+
+You can choose to get training data as a Pandas DataFrame or as a Table in the feature store that contains metadata on how the table was created for reuse or audit.
+
+``` python
+# Get feature list from the catalog
+feature_list = catalog.get_feature_list(
+    "200 Features on Active Customers"
+)
+# Create a new feature list that includes a new feature
+customer_state_similarity_28d = catalog.get_feature(
+    "Customer Similarity with purchases in the same state over 28 days"
+)
+new_feature_list = fb.FeatureList(
+    [feature_list, customer_state_similarity_28d],
+    name="Improved feature list with Customer State similarity"
+)
+# Get an observation set from the catalog
+observation_set = catalog.get_observation_table(
+    "5M of active Customers in 2021-2022"
+)
+# Compute training data and store it in the feature store for reuse and audit
+training_table = new_feature_list.compute_historical_feature_table(
+    observation_set,
+    name="Improved Data to predict purchases next 2w with 2021-2022 history"
+)
+# Download training data as a Pandas DataFrame
+training_df = training_table.to_pandas()
+```
+
+Refer to the SDK reference for the [FeatureList](https://docs.featurebyte.com/latest/reference/core/feature_list/), [ObservationTable](https://docs.featurebyte.com/latest/reference/core/observation_table/) and [HistoricalFeatureTable](https://docs.featurebyte.com/latest/reference/core/historical_feature_table/) objects, for more information.
+
+## Deploy when needed
+
+Once a feature list is deployed, the FeatureByte Service automatically orchestrates the pre-computation of feature values and stores them in an online feature store for online and batch serving.
+
+``` python
+# Get feature list from the catalog
+feature_list = catalog.get_feature_list(
+    "200 Features on Active Customers"
+)
+# Check Feature objects are PRODUCTION_READY.
+# A readiness metric of 100% should be returned.
+print(feature_list.production_ready_fraction)
+# Create deployment
+my_deployment = feature_list.deploy(
+    name="Deployment of 200 Features to predict customers purchases amount next 2 weeks",
+)
+# Activate deployment
+my_deployment.enable()
+```
+
+Use the REST API service to retrieve feature values from the online feature store for online serving or use the SDK to retrieve batch of feature values from the online feature store for batch serving.
+
+### Online Serving
+For online serving, the Deployment object provides REST API service templates that can be used to serve features. Python or shell script templates for the REST API service are retrieved from the Deployment object.
+
+Get online scoring code as a Python script:
+``` python
+deployment = catalog.get_deployment(
+    "Deployment of 200 Features to predict customers purchases amount next 2 weeks"
+)
+deployment.get_online_serving_code(language="python")
+```
+
+Get online scoring code as a Shell script:
+``` python
+deployment.get_online_serving_code(language="sh")
+```
+
+### Batch Serving
+For batch serving, the Deployment object is used to retrieve feature values for a batch request table containing entities values.
+
+``` python
+from datetime import datetime
+batch_features = deployment.compute_batch_feature_table(
+    batch_request_table=batch_request_table,
+    batch_feature_table_name=
+        "Data to predict customers purchases next 2 w as of " +
+        datetime.utcnow().strftime('%Y-%m-%dT%H:%M:%SZ')
+)
+# Download batch feature values as a Pandas DataFrame
+batch_features_df = batch_features.to_pandas()
+```
+
+Refer to the SDK reference for the [Deployment](https://docs.featurebyte.com/latest/reference/core/deployment/), [BatchRequestTable](https://docs.featurebyte.com/latest/reference/core/batch_request_table/) and [BatchFeatureTable](https://docs.featurebyte.com/latest/reference/core/batch_feature_table/) objects, for more information.
+
+
+## Releases
+
+You can see the list of available releases on the [Change Log](https://github.com/featurebyte/featurebyte/blob/main/CHANGELOG.md) page.
+Releases are versioned using the [Semantic Versions](https://semver.org/) specification.
+
+## License
+
+[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
+
+This project is licensed under the terms of the `Elastic License 2.0` license. See [LICENSE](https://github.com/featurebyte/featurebyte/blob/main/LICENSE) for more details.
+
+## Contributing
+[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
+
+All contributions are welcomed. Please adhere to the [Code of Conduct](https://github.com/featurebyte/featurebyte/blob/main/CODE_OF_CONDUCT.md) and read the
+[Developer's Guide](https://github.com/featurebyte/featurebyte/blob/main/CONTRIBUTING.md) to get started.
 
-setup(**setup_kwargs)
```

