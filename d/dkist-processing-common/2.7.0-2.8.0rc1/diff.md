# Comparing `tmp/dkist-processing-common-2.7.0.tar.gz` & `tmp/dkist-processing-common-2.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.7.0.tar", last modified: Wed May 17 17:05:51 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.8.0rc1.tar", last modified: Mon Jun  5 16:22:54 2023, max compression
```

## Comparing `dkist-processing-common-2.7.0.tar` & `dkist-processing-common-2.8.0rc1.tar`

### file list

```diff
@@ -1,115 +1,122 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.048798 dkist-processing-common-2.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-17 17:05:51.048798 dkist-processing-common-2.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.036798 dkist-processing-common-2.7.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.036798 dkist-processing-common-2.7.0/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.036798 dkist-processing-common-2.7.0/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.040798 dkist-processing-common-2.7.0/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.040798 dkist-processing-common-2.7.0/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.040798 dkist-processing-common-2.7.0/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.040798 dkist-processing-common-2.7.0/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.044798 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.044798 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.044798 dkist-processing-common-2.7.0/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.036798 dkist-processing-common-2.7.0/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-17 17:05:50.000000 dkist-processing-common-2.7.0/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-05-17 17:05:51.000000 dkist-processing-common-2.7.0/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-17 17:05:50.000000 dkist-processing-common-2.7.0/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-05-17 17:05:50.000000 dkist-processing-common-2.7.0/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-05-17 17:05:50.000000 dkist-processing-common-2.7.0/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.048798 dkist-processing-common-2.7.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:05:51.048798 dkist-processing-common-2.7.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-05-17 17:05:51.048798 dkist-processing-common-2.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-17 17:05:43.000000 dkist-processing-common-2.7.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/changelog/139.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6382 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/dev_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10709 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.120769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3450 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     7417 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_dev_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     5380 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.116769 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4489 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-05 16:22:54.000000 dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-05 16:22:54.124769 dkist-processing-common-2.8.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-05 16:22:54.128769 dkist-processing-common-2.8.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-05 16:22:47.000000 dkist-processing-common-2.8.0rc1/setup.py
```

### Comparing `dkist-processing-common-2.7.0/.gitignore` & `dkist-processing-common-2.8.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/.pre-commit-config.yaml` & `dkist-processing-common-2.8.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/CHANGELOG.rst` & `dkist-processing-common-2.8.0rc1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/PKG-INFO` & `dkist-processing-common-2.8.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.7.0
+Version: 2.8.0rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.7.0/README.rst` & `dkist-processing-common-2.8.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/bitbucket-pipelines.yml` & `dkist-processing-common-2.8.0rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/check_changelog_updated.sh` & `dkist-processing-common-2.8.0rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/manual.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/message.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     modstate = "MODSTATE"
     dsps_repeat = "DSPS_REPEAT"
     calibrated = "CALIBRATED"  # A flag to indicate the data has been calibrated but not yet output
     quality = "QUALITY"
     exposure_time = "EXP_TIME"
     quality_task = "QUALITY_TASK"
     parameter = "PARAMETER"
+    debug = "DEBUG"
 
 
 class Tag:
     """Controlled methods for creating tags from stems + optional suffixes."""
 
     @staticmethod
     def format_tag(stem: StemName | str, *parts):
@@ -157,14 +158,19 @@
 
         Returns
         -------
         A movie tag
         """
         return cls.format_tag(StemName.movie)
 
+    @classmethod
+    def debug(cls) -> str:
+        """Return a debug tag."""
+        return cls.format_tag(StemName.debug)
+
     # Dynamic Tags
     @classmethod
     def task(cls, ip_task_type: str):
         """
         Return a task tag for the given task type.
 
         Parameters
```

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Task(s) for the transfer out of data from a processing pipeline."""
+"""Task(s) for the transfer and publishing of L1 data from a production run of a processing pipeline."""
 import logging
 from abc import ABC
 from functools import cached_property
 from pathlib import Path
 from typing import Iterable
 
 from dkist_processing_common.models.message import CatalogFrameMessage
```

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/fits.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 class FitsDataMixin:
     """Mixin for the WorkflowDataTaskBase to support fits r/w operations."""
 
     def fits_data_read(
         self, tags: tag_type_hint
     ) -> Generator[tuple[Path, fits.HDUList], None, None]:
-        """Return a generator of paths and fits objects for input data matching the given tags."""
+        """Return a generator of paths and fits HDU lists for input data matching the given tags."""
         for path in self.read(tags=tags):
             yield path, self.fits_data_open(path)
 
     def fits_data_read_hdu(
         self, tags: tag_type_hint
     ) -> Generator[tuple[Path, fits.PrimaryHDU | fits.CompImageHDU], None, None]:
-        """Return a generator of paths and hdu lists for the input data matching the given tags."""
+        """Return a generator of paths and hdus for the input data matching the given tags."""
         for path, hdul in self.fits_data_read(tags=tags):
             yield path, self.fits_data_extract_hdu(hdul=hdul)
 
     def fits_data_read_fits_access(
         self,
         tags: tag_type_hint,
         cls: Type[FitsAccessBase],
@@ -52,13 +52,16 @@
         return fits.open(path)
 
     def fits_data_write(
         self,
         hdu_list: fits.HDUList,
         tags: tag_type_hint,
         relative_path: Path | str | None = None,
+        overwrite: bool = False,
     ) -> Path:
         """Write the fits object to a file with the given path and tag with the given tags."""
         file_obj = BytesIO()
         hdu_list.writeto(file_obj, checksum=True)
         file_obj.seek(0)
-        return self.write(file_obj=file_obj, tags=tags, relative_path=relative_path)
+        return self.write(
+            file_obj=file_obj, tags=tags, relative_path=relative_path, overwrite=overwrite
+        )
```

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.8.0rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.7.0
+Version: 2.8.0rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/139.feature.2.rst
+changelog/139.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
@@ -47,21 +49,23 @@
 dkist_processing_common/parsers/quality.py
 dkist_processing_common/parsers/single_value_single_key_flower.py
 dkist_processing_common/parsers/time.py
 dkist_processing_common/parsers/unique_bud.py
 dkist_processing_common/tasks/__init__.py
 dkist_processing_common/tasks/assemble_movie.py
 dkist_processing_common/tasks/base.py
+dkist_processing_common/tasks/dev_output_data.py
 dkist_processing_common/tasks/l1_output_data.py
 dkist_processing_common/tasks/parse_l0_input_data.py
 dkist_processing_common/tasks/quality_metrics.py
 dkist_processing_common/tasks/teardown.py
 dkist_processing_common/tasks/transfer_input_data.py
 dkist_processing_common/tasks/write_l1.py
 dkist_processing_common/tasks/mixin/__init__.py
+dkist_processing_common/tasks/mixin/debug_frame.py
 dkist_processing_common/tasks/mixin/fits.py
 dkist_processing_common/tasks/mixin/globus.py
 dkist_processing_common/tasks/mixin/input_dataset.py
 dkist_processing_common/tasks/mixin/interservice_bus.py
 dkist_processing_common/tasks/mixin/metadata_store.py
 dkist_processing_common/tasks/mixin/object_store.py
 dkist_processing_common/tasks/mixin/quality/__init__.py
@@ -69,15 +73,18 @@
 dkist_processing_common/tasks/mixin/quality/_metrics.py
 dkist_processing_common/tests/__init__.py
 dkist_processing_common/tests/conftest.py
 dkist_processing_common/tests/test_assemble_movie.py
 dkist_processing_common/tests/test_base.py
 dkist_processing_common/tests/test_constants.py
 dkist_processing_common/tests/test_cs_step.py
+dkist_processing_common/tests/test_debug_frame.py
+dkist_processing_common/tests/test_dev_output_data.py
 dkist_processing_common/tests/test_dkist_location.py
+dkist_processing_common/tests/test_fits.py
 dkist_processing_common/tests/test_fits_access.py
 dkist_processing_common/tests/test_fits_flowers.py
 dkist_processing_common/tests/test_flower_pot.py
 dkist_processing_common/tests/test_input_dataset.py
 dkist_processing_common/tests/test_l1_output_data_base.py
 dkist_processing_common/tests/test_parameters.py
 dkist_processing_common/tests/test_parse_l0_input_data.py
```

### Comparing `dkist-processing-common-2.7.0/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.8.0rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/docs/Makefile` & `dkist-processing-common-2.8.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/docs/conf.py` & `dkist-processing-common-2.8.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/docs/make.bat` & `dkist-processing-common-2.8.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/licenses/LICENSE.rst` & `dkist-processing-common-2.8.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/pyproject.toml` & `dkist-processing-common-2.8.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.7.0/setup.cfg` & `dkist-processing-common-2.8.0rc1/setup.cfg`

 * *Files identical despite different names*

