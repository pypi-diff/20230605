# Comparing `tmp/debater_python_api-4.3.2.tar.gz` & `tmp/debater_python_api-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debater_python_api-4.3.2.tar", last modified: Sun Apr 30 13:43:43 2023, max compression
+gzip compressed data, was "debater_python_api-5.0.0.tar", last modified: Mon Jun  5 12:57:00 2023, max compression
```

## Comparing `debater_python_api-4.3.2.tar` & `debater_python_api-5.0.0.tar`

### file list

```diff
@@ -1,96 +1,94 @@
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.831185 debater_python_api-4.3.2/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    11358 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/LICENSE
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-04-30 13:43:43.831010 debater_python_api-4.3.2/PKG-INFO
--rw-r--r--   0 yoavkantor   (501) staff       (20)      169 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/README.md
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.820064 debater_python_api-4.3.2/debater_python_api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.821190 debater_python_api-4.3.2/debater_python_api/api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.824154 debater_python_api-4.3.2/debater_python_api/api/clients/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4503 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/abstract_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1147 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/argument_quality_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1548 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      934 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/claim_boundaries_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6203 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/clustering_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3034 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/embedding_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1999 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/index_searcher_client.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.825239 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    28620 2023-04-18 08:38:46.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      136 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpaExceptions.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    17249 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/KpaResult.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    12256 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/docx_generator.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2121 2023-01-23 14:28:56.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/try_things.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1711 2023-01-18 11:06:06.000000 debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/utils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6234 2022-12-27 12:16:15.000000 debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_admin_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    28126 2023-04-30 13:39:08.000000 debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1894 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13830 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/narrative_generation_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1230 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/pro_con_client.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.825508 debater_python_api-4.3.2/debater_python_api/api/clients/response_data/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/response_data/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1597 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/response_data/speech_response.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1790 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/term_relater_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1563 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/term_wikifier_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3394 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/clients/theme_extraction_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3270 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/debater_api.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.825641 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.826556 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      142 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     5079 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_client.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1001 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1314 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     3576 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1516 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.828623 debater_python_api-4.3.2/debater_python_api/examples/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      803 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/argument_quality_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      854 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/claim_boundaries_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1002 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/claim_detection_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      932 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/clustering_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      860 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/embedding_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1014 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/evidence_detection_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    85859 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/example_of_sc_args.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1480 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/index_searcher_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1173 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/examples/keypoints_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1428 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/pro_con_example.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.828987 debater_python_api-4.3.2/debater_python_api/examples/resources/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    23817 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/arguments.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829122 debater_python_api-4.3.2/debater_python_api/examples/resources/filters_output/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/filters_output/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2530 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/resources/pro_con_scores.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     9581 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/run_all_services.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      870 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/speech_construction_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      480 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/term_relater_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      907 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/term_wikifier_example.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1154 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/theme_extraction_example.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829476 debater_python_api-4.3.2/debater_python_api/examples/usecases/
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4943 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/usecases/kp_based_survey.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     6036 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/usecases/mining_to_narrative.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    10191 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/examples/usecases/survey.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829611 debater_python_api-4.3.2/debater_python_api/integration_tests/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.829718 debater_python_api-4.3.2/debater_python_api/integration_tests/api/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.830205 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/
--rw-r--r--   0 yoavkantor   (501) staff       (20)     2708 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)    11539 2023-04-18 07:19:29.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesIT.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4630 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/__init__.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.830793 debater_python_api-4.3.2/debater_python_api/utils/
--rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/__init__.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      992 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/clusters_refiner.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1574 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/general_utils.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)      604 2022-12-21 08:56:59.000000 debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_conf.py
--rw-r--r--   0 yoavkantor   (501) staff       (20)     1816 2023-01-18 09:21:46.000000 debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_utils.py
-drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-04-30 13:43:43.820855 debater_python_api-4.3.2/debater_python_api.egg-info/
--rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yoavkantor   (501) staff       (20)     4126 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)        1 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)       87 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/requires.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)       19 2023-04-30 13:43:43.000000 debater_python_api-4.3.2/debater_python_api.egg-info/top_level.txt
--rw-r--r--   0 yoavkantor   (501) staff       (20)      879 2023-04-30 13:43:21.000000 debater_python_api-4.3.2/pyproject.toml
--rw-r--r--   0 yoavkantor   (501) staff       (20)       38 2023-04-30 13:43:43.831222 debater_python_api-4.3.2/setup.cfg
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.259941 debater_python_api-5.0.0/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    11358 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/LICENSE
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-05 12:57:00.259727 debater_python_api-5.0.0/PKG-INFO
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      169 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/README.md
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.246186 debater_python_api-5.0.0/debater_python_api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.247191 debater_python_api-5.0.0/debater_python_api/api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.251223 debater_python_api-5.0.0/debater_python_api/api/clients/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4503 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/abstract_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1147 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/argument_quality_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1548 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/claim_and_evidence_detection_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      934 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/claim_boundaries_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6203 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/clustering_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3034 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/embedding_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1999 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/index_searcher_client.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.252076 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      478 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    35911 2023-06-05 12:56:29.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/KpsResult.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13092 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/docx_generator.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    14916 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/graph_generator.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3923 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/utils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6969 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_admin_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    39177 2023-06-05 12:50:31.000000 debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1894 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_pairs_infer_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13830 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/narrative_generation_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1230 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/pro_con_client.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.252351 debater_python_api-5.0.0/debater_python_api/api/clients/response_data/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/response_data/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1597 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/response_data/speech_response.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1790 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/term_relater_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1563 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/term_wikifier_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3394 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/clients/theme_extraction_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3263 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/api/debater_api.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.252597 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.253750 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      142 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     5079 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_client.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1001 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1314 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     3576 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_base.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1516 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_request.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.256659 debater_python_api-5.0.0/debater_python_api/examples/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      803 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/argument_quality_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      854 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/claim_boundaries_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1002 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/claim_detection_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      932 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/clustering_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      860 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/embedding_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1014 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/evidence_detection_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    85859 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/example_of_sc_args.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1480 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/index_searcher_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1204 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/examples/keypoints_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1428 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/pro_con_example.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257144 debater_python_api-5.0.0/debater_python_api/examples/resources/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    23817 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/arguments.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257313 debater_python_api-5.0.0/debater_python_api/examples/resources/filters_output/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/filters_output/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2530 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/resources/pro_con_scores.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     9581 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/run_all_services.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      870 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/speech_construction_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      480 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/term_relater_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      907 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/term_wikifier_example.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1154 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/theme_extraction_example.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257753 debater_python_api-5.0.0/debater_python_api/examples/usecases/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4943 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/usecases/kp_based_survey.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     6036 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/usecases/mining_to_narrative.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    10191 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/examples/usecases/survey.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.257910 debater_python_api-5.0.0/debater_python_api/integration_tests/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.258032 debater_python_api-5.0.0/debater_python_api/integration_tests/api/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.258635 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     2708 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    11791 2023-06-04 13:58:49.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesIT.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4630 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesLoad.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/__init__.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.259448 debater_python_api-5.0.0/debater_python_api/utils/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        0 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/__init__.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      992 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/clusters_refiner.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     1574 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/general_utils.py
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      604 2022-12-21 08:56:59.000000 debater_python_api-5.0.0/debater_python_api/utils/kp_analysis_conf.py
+drwxr-xr-x   0 yoavkantor   (501) staff       (20)        0 2023-06-05 12:57:00.246908 debater_python_api-5.0.0/debater_python_api.egg-info/
+-rw-r--r--   0 yoavkantor   (501) staff       (20)    13508 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yoavkantor   (501) staff       (20)     4041 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)        1 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       87 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/requires.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       19 2023-06-05 12:57:00.000000 debater_python_api-5.0.0/debater_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yoavkantor   (501) staff       (20)      879 2023-06-05 12:56:29.000000 debater_python_api-5.0.0/pyproject.toml
+-rw-r--r--   0 yoavkantor   (501) staff       (20)       38 2023-06-05 12:57:00.259987 debater_python_api-5.0.0/setup.cfg
```

### Comparing `debater_python_api-4.3.2/LICENSE` & `debater_python_api-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/PKG-INFO` & `debater_python_api-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater_python_api
-Version: 4.3.2
+Version: 5.0.0
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/abstract_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/abstract_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/argument_quality_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/argument_quality_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/claim_and_evidence_detection_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/claim_and_evidence_detection_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/claim_boundaries_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/claim_boundaries_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/clustering_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/clustering_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/embedding_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/embedding_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/index_searcher_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/index_searcher_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/key_point_analysis/docx_generator.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/key_point_summarization/docx_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,40 @@
 import logging
+import random
 
 import docx
 from docx.enum.dml import MSO_THEME_COLOR_INDEX
 from docx.shared import Inches, Pt, RGBColor
 from docx import Document
 
-from debater_python_api.api.clients.key_point_analysis.KpaResult import KpaResult
-from debater_python_api.api.clients.key_point_analysis.utils import create_dict_to_list, \
-    trunc_float, read_dicts_from_df
+from debater_python_api.api.clients.key_point_summarization.KpsExceptions import KpsIllegalInputException
+from debater_python_api.api.clients.key_point_summarization.utils import create_dict_to_list, \
+    trunc_float, read_dicts_from_df, get_unique_sent_id
 
 from docx.oxml.shared import OxmlElement
 from docx.oxml.ns import qn
 
+stance_to_stance_str = {"con": "Negative", "pro":"Positive", "":""}
+
+def get_stance_to_stance_str(stances):
+    if not stances:
+        return ""
+    if isinstance(stances, str):
+        stances = [stances]
+    if set(stances) == set(["no-stance"]):
+        return ""
+    if len(stances) == 1:
+        return stance_to_stance_str[list(stances)[0]]
+    if set(stances) == set(["pro","con"]):
+        return "Positive and Negative"
+    raise KpsIllegalInputException(f"unsupported stances {stances}")
+
+def get_kp_stance_if_needed(id_data, stances):
+    return id_data["kp_stance"].capitalize() + ", " if stances == {"pro", "con"} else ""
+
 def insertHR(paragraph):
     p = paragraph._p  # p is the <w:p> XML element
     pPr = p.get_or_add_pPr()
     pBdr = OxmlElement('w:pBdr')
     pPr.insert_element_before(pBdr,
         'w:shd', 'w:tabs', 'w:suppressAutoHyphens', 'w:kinsoku', 'w:wordWrap',
         'w:overflowPunct', 'w:topLinePunct', 'w:autoSpaceDE', 'w:autoSpaceDN',
@@ -74,177 +93,154 @@
 
 def set_heading(heading):
     paragraph_format = heading.paragraph_format
     paragraph_format.page_break_before = False
     paragraph_format.keep_with_next = False
     paragraph_format.keep_together = False
 
-
-def get_unique_matches_subtree(node_id, id_to_node, id_to_kids, id_to_n_unique_matches_subtree, kp_to_dicts, by_sentence = True):
-    kp = id_to_node[node_id]['data']['kp']
-    if by_sentence:
-        kp_unique_sentences = set([KpaResult.get_unique_sent_id(d) for d in kp_to_dicts[kp]])
-    else: # by comments
-        kp_unique_sentences = set([d['comment_id'] for d in kp_to_dicts[kp]])
-    if node_id in id_to_kids:
-        for kid in id_to_kids[node_id]:
-            kp_unique_sentences = kp_unique_sentences.union(get_unique_matches_subtree(kid, id_to_node, id_to_kids, id_to_n_unique_matches_subtree, kp_to_dicts, by_sentence))
-    id_to_n_unique_matches_subtree[node_id] = len(kp_unique_sentences)
-    return kp_unique_sentences
-
-def add_data_stats(dicts, nodes_ids, document, stance, min_n_matches):
+def add_data_stats(meta_data, dicts, kp_id_to_data, document, stances, min_n_matches):
+    n_kps = len(kp_id_to_data)
+    n_total_sentences = meta_data["general"]["n_sentences"]
+    n_total_comments = meta_data["general"]["n_comments"]
     dicts_not_none = list(filter(lambda r: r["kp"] != "none", dicts))
-    n_sents = len(set([KpaResult.get_unique_sent_id(d) for d in dicts]))
-    rate_matched_sents = 100 *len(set([KpaResult.get_unique_sent_id(d) for d in dicts_not_none])) / n_sents
-    n_comments = len(set([d["comment_id"] for d in dicts]))
-    rate_matched_comments = 100 *len(set([d["comment_id"] for d in dicts_not_none])) / n_comments
-    n_kps = len(nodes_ids)
-    if stance == "pos":
-        stance_str = " with positive sentiment"
-    elif stance == "neg":
-        stance_str = " with negative sentiment"
-    else:
-        stance_str = ""
+    n_matches_sentences = len(set([get_unique_sent_id(d) for d in dicts_not_none]))
+    n_matches_comments = len(set([d["comment_id"] for d in dicts_not_none])) # Todo: this includes matches to smaller, filtered kps!
+    rate_matched_sents = 100*n_matches_sentences / n_total_sentences
+    rate_matched_comments = 100*n_matches_comments / n_total_comments
+
+    stances_str = get_stance_to_stance_str(stances).lower()
 
     heading = document.add_heading('Data Statistics', 1)
     set_heading(heading)
+    s = f'Analyzed {n_total_comments} comments ({n_total_sentences} sentences).\n' \
+        f'Identified {n_kps} {stances_str.lower()} key points with at least {min_n_matches or 1} matching sentences.\n' \
+        f'{int(rate_matched_comments)}% of the comments (and {int(rate_matched_sents)}%' \
+        f' of the sentences) were matched to at least one key point.\n'
+    for stance in ["pro","con"]:
+        if stance in stances:
+            stance_str = get_stance_to_stance_str(stance).lower()
+            n_kps_stance = len(list(filter(lambda kp_id:kp_id_to_data[kp_id].get("kp_stance")==stance, kp_id_to_data)))
+            kp_stance_str = f"of {n_kps_stance} {stance_str} key points." if len(stances) > 1 else "key point."
+
+            n_stance_sentences = meta_data["per_stance"][stance]["n_sentences_stance"]
+            n_stance_comments = meta_data["per_stance"][stance]["n_comments_stance"]
+            dicts_stance = list(filter(lambda r: r["kp_stance"] == stance, dicts_not_none))
+            n_matches_sentences_stance = len(set([get_unique_sent_id(d) for d in dicts_stance]))
+            n_matches_comments_stance = len(set([d["comment_id"] for d in dicts_stance]))
+            matched_sentences_stance_rate = 100*n_matches_sentences_stance/n_stance_sentences if n_stance_sentences > 0 else 0
+            matched_comments_stance_rate = 100*n_matches_comments_stance / n_stance_comments if n_stance_comments > 0 else 0
+            s += f'Identified {n_stance_comments} {stance_str} comments (and {n_stance_sentences} {stance_str} sentences).\n'\
+                 f'{int(matched_comments_stance_rate)}% of these comments (and {int(matched_sentences_stance_rate)}% of these sentences)' \
+                f' were matched to at least one {kp_stance_str}\n'
     p = document.add_paragraph()
-    run = p.add_run(
-         f'Analyzed {n_comments} comments ({n_sents} sentences){stance_str}.\n'
-        f'Identified {n_kps} key points with at least {min_n_matches or 1} matching sentences.\n'
-        f'{int(rate_matched_comments)}% of the comments (and {int(rate_matched_sents)}%'
-        f' of the sentences) were matched to at least one key point.'
-        )
-
+    run = p.add_run(s)
     run.font.size = Pt(12)
 
 
-def save_hierarchical_graph_data_to_docx(kpa_result: KpaResult, graph_data, result_filename, n_top_matches=None, sort_by_subtree=True, include_match_score=False, min_n_matches=5, file_suff=""):
-    def get_hierarchical_bullets_aux(document, id_to_kids, id_to_node, id, tab, id_to_paragraph, id_to_n_matches_subtree, sort_by_subtree=True, ids_order=[]):
+def sample_list_keep_order(list_to_sample, n_to_sample, seed=0):
+    rng = random.Random(seed)
+    return [list_to_sample[i] for i in sorted(rng.sample(range(len(list_to_sample)), n_to_sample))]
+
+
+def save_hierarchical_graph_data_to_docx(full_result_df, kp_id_to_data, result_filename, meta_data, n_matches=None, sort_by_subtree=True, include_match_score=False, min_n_matches=5, seed=0):
+
+    def get_hierarchical_bullets_aux(document, kp_id_to_data, id, tab, id_to_paragraph, sort_by_subtree=True, ids_order=[]):
         bullet = '\u25E6' if tab % 2 == 1 else '\u2022'
         msg = f'{("   " * tab)} {bullet} '
 
         heading = document.add_heading(msg, 9 if (tab + 1) > 9 else (tab+1))
         set_heading(heading)
 
         id_to_paragraph[id] = heading
         ids_order.append(id)
 
-        if id in id_to_kids:
-            kids = id_to_kids[id]
+        kids = kp_id_to_data[id].get('kids')
+        if kids and len(kids) > 0:
             if sort_by_subtree:
-                kids = sorted(kids, key=lambda n: int(id_to_n_matches_subtree[n]), reverse=True)
+                kids = sorted(kids, key=lambda n: int(kp_id_to_data[n].get('n_matching_sents_in_subtree')), reverse=True)
             else:
-                kids = sorted(kids, key=lambda n: int(id_to_node[n]['data']['n_matches']), reverse=True)
+                kids = sorted(kids, key=lambda n: int(kp_id_to_data[n]['n_matching_sentences']), reverse=True)
             for k in kids:
-                get_hierarchical_bullets_aux(document, id_to_kids, id_to_node, k, tab + 1, id_to_paragraph, id_to_n_matches_subtree, sort_by_subtree, ids_order)
+                get_hierarchical_bullets_aux(document, kp_id_to_data, k, tab + 1, id_to_paragraph, sort_by_subtree, ids_order)
 
 
-    def get_hierarchical_bullets(document, roots, id_to_kids, id_to_node, id_to_paragraph, id_to_n_matches_subtree, sort_by_subtree=True, ids_order=[]):
+    def get_hierarchical_bullets(document, roots, kp_id_to_data, id_to_paragraph, sort_by_subtree=True, ids_order=[]):
         tab = 0
         if sort_by_subtree:
-            roots = sorted(roots, key=lambda n: int(id_to_n_matches_subtree[n]), reverse=True)
+            roots = sorted(roots, key=lambda n: int(kp_id_to_data[n].get('n_matching_sents_in_subtree')), reverse=True)
         else:
-            roots = sorted(roots, key=lambda n: int(id_to_node[n]['data']['n_matches']), reverse=True)
+            roots = sorted(roots, key=lambda n: int(kp_id_to_data[n]['n_matching_sentences']), reverse=True)
         for root in roots:
-            get_hierarchical_bullets_aux(document, id_to_kids, id_to_node, root, tab, id_to_paragraph, id_to_n_matches_subtree, sort_by_subtree=True, ids_order=ids_order)
-
-    nodes = [d for d in graph_data if d['type'] == 'node']
-    edges = [d for d in graph_data if d['type'] == 'edge']
-
-    if min_n_matches is not None:
-        nodes = [n for n in nodes if int(n['data']['n_matches'])>=min_n_matches]
-
-    nodes_ids = [n['data']['id'] for n in nodes]
-    edges = [e for e in edges if (e['data']['target'] in nodes_ids and e['data']['source'] in nodes_ids)]
-
-    id_to_kids = create_dict_to_list([(e['data']['target'], e['data']['source']) for e in edges])
-    id_to_node = {d['data']['id']: d for d in nodes}
-
-    all_kids = set()
-    for id, kids in id_to_kids.items():
-        all_kids = all_kids.union(kids)
-
-    root_ids = set(nodes_ids).difference(all_kids)
+            get_hierarchical_bullets_aux(document, kp_id_to_data, root, tab, id_to_paragraph, sort_by_subtree=True, ids_order=ids_order)
 
     document = Document()
     style = document.styles['Normal']
     style.font.name = 'Calibri'
 
-    dicts, _ = read_dicts_from_df(kpa_result.result_df)
-    kp_to_dicts = create_dict_to_list([(d['kp'], d) for d in dicts])
-
-    id_to_n_matches_subtree = {}
-    for root in root_ids:
-        get_unique_matches_subtree(root, id_to_node, id_to_kids, id_to_n_matches_subtree, kp_to_dicts)
-
-    stances = set([d['stance'] for d in dicts if 'stance' in d])
-    stances = stances.union(set([d['selected_stance'] for d in dicts if 'selected_stance' in d]))
-
-    stance = None
-    if len(stances) == 1 and 'pos' in stances:
-        stance = 'pos'
-    elif (len(stances) == 1 and ('neg' in stances or 'sug' in stances)) \
-            or (len(stances) == 2 and 'neg' in stances and 'sug' in stances):
-        stance = 'neg'
 
-    heading = document.add_heading('Key Point Analysis Results', 1)
+    heading = document.add_heading('Key Point Summarization Results', 1)
     set_heading(heading)
 
-    if stance == 'pos':
-        p = document.add_paragraph('Positive Key Points')
-        p.style = document.styles['Subtitle']
-        set_heading(p)
-        insertHR(p)
-    elif stance == 'neg':
-        p = document.add_paragraph('Negative Key Points')
+    if min_n_matches is not None:
+        kp_id_to_data = {kp_id:kp_id_to_data[kp_id] for kp_id in kp_id_to_data if int(kp_id_to_data[kp_id]['n_matching_sentences'])>=min_n_matches}
+
+    stances = list(meta_data["per_stance"].keys())#set(data['kp_stance'] for id,data in kp_id_to_data.items() if data['kp_stance'])
+    stance_str = get_stance_to_stance_str(stances)
+    if stance_str:
+        p = document.add_paragraph(stance_str + " Key Points")
         p.style = document.styles['Subtitle']
         set_heading(p)
-        insertHR(p)
-    else:
-        insertHR(heading)
+    insertHR(heading)
 
-    add_data_stats(dicts, nodes_ids, document, stance, min_n_matches)
+    kps = [data["kp"] for data in kp_id_to_data.values()]
+    dicts, _ = read_dicts_from_df(full_result_df)
+    dicts = list(filter(lambda d: d["kp"] in kps, dicts))
+    kp_to_dicts = create_dict_to_list([(d['kp'], d) for d in dicts])
+
+    add_data_stats(meta_data, dicts, kp_id_to_data, document, stances, min_n_matches)
 
     heading = document.add_heading('Key Point Hierarchy', 1)
     set_heading(heading)
 
     p = document.add_paragraph()
     run = p.add_run('Click (Ctrl+Click on windows) on each key point to view top matching sentences.\nThen use back link (Alt+LeftArrow on windows) to go back.')
     run.font.size = Pt(10)
-    id_to_kids = create_dict_to_list([(e['data']['target'], e['data']['source']) for e in edges])
 
     logging.info('Creating key points hierarchy')
 
     id_to_paragraph1 = {}
     ids_order = []
-    get_hierarchical_bullets(document, root_ids, id_to_kids, id_to_node, id_to_paragraph1, id_to_n_matches_subtree, ids_order=ids_order)
+
+    root_ids = list(filter(lambda x:not kp_id_to_data[x].get('parent'), kp_id_to_data.keys()))
+    get_hierarchical_bullets(document, root_ids, kp_id_to_data, id_to_paragraph1, ids_order=ids_order)
 
     logging.info('Creating key points matches tables')
 
-    if n_top_matches is None:
+    if n_matches is None:
         heading = document.add_heading(f'\n\nAll matches per key point', 1)
     else:
-        heading = document.add_heading(f'\n\nTop {n_top_matches} matches per key point', 1)
+        heading = document.add_heading(f'\n\nTop {n_matches} matches per key point', 1)
     set_heading(heading)
 
     id_to_paragraph2 = {}
     for id in ids_order:
-        n = id_to_node[id]
-        kp = n["data"]["kp"]
+        id_data = kp_id_to_data[id]
+        kp = id_data['kp']
 
-        heading = document.add_heading(f'\nKey point: {kp}  ({n["data"]["n_matches"]} matches)', 2)
+        kp_stance_str = get_kp_stance_if_needed(id_data, stances)
+        heading = document.add_heading(f'\nKey point: {kp}  ({kp_stance_str}{id_data["n_matching_comments"]}'
+                                       f' matching comments, {id_data["n_matching_sentences"]} matching sentences)', 2)
         set_heading(heading)
         id_to_paragraph2[id] = heading
 
         matches_dicts = kp_to_dicts[kp]
-        if n_top_matches is not None and n_top_matches < len(kp_to_dicts[kp]):
-            matches_dicts = matches_dicts[:n_top_matches]
+        if n_matches is not None and n_matches < len(kp_to_dicts[kp]):
+            matches_dicts = sample_list_keep_order(matches_dicts, n_matches, seed=seed)
 
-        logging.info(f'creating table for KP: {kp}, n_matches: {len(matches_dicts)}')
+        #logging.info(f'creating table for KP: {kp}, {stance_str}, matching sentences: {len(matches_dicts)}')
 
         records = []
         for d in matches_dicts:
             records.append([d["sentence_text"], trunc_float(float(d["match_score"]), 4)])
 
         heading = document.add_heading(f'Matching Sentences', 3)
         set_heading(heading)
@@ -269,29 +265,29 @@
                 row_cells[1].width = Inches(0.5)
 
     # add a bookmark to every paragraph
     for id, paragraph in id_to_paragraph2.items():
         add_bookmark(paragraph=paragraph, bookmark_text="", bookmark_name=f'table_bookmark{id}')
 
     for id, paragraph in id_to_paragraph1.items():
-        node = id_to_node[id]
-        kp = node['data']['kp']
-        n_matches = int(node["data"]["n_matches"])
-        if n_matches == id_to_n_matches_subtree[id]:
+        id_data = kp_id_to_data[id]
+        kp = id_data['kp']
+        kp_stance_str = get_kp_stance_if_needed(id_data, stances)
+        n_matches = int(id_data["n_matching_sentences"])
+        if n_matches == id_data["n_matching_sents_in_subtree"]:
             msg = f'{kp} ({n_matches} matches)'
         else:
             if sort_by_subtree:
-                msg = f'{kp} ({id_to_n_matches_subtree[id]} matching sentences in subtree, {n_matches} matches)'
+                msg = f'{kp} ({kp_stance_str}{id_data["n_matching_sents_in_subtree"]} matching sentences in subtree, {n_matches} matches)'
             else:
-                msg = f'{kp} ({n_matches} matches, {id_to_n_matches_subtree[id]} in subtree)'
+                msg = f'{kp} ({kp_stance_str}{n_matches} matches, {id_data["n_matching_sents_in_subtree"]} in subtree)'
         add_link(paragraph=paragraph, link_to=f'table_bookmark{id}', text=msg, tool_tip="Click to view top matching sentences")
 
     for id, paragraph in id_to_paragraph1.items():
         add_bookmark(paragraph=paragraph, bookmark_text="", bookmark_name=f'hierarchy_bookmark{id}')
 
     for id, paragraph in id_to_paragraph2.items():
         msg = ' - back'
         add_link(paragraph=paragraph, link_to=f'hierarchy_bookmark{id}', text=msg, tool_tip="Click to view hierarchy", set_color=True)
 
-    out_file = result_filename.replace('.csv', f'{file_suff}_hierarchical.docx')
-    logging.info(f'saving docx summary in file: {out_file}')
-    document.save(out_file)
+    logging.info(f'saving docx summary in file: {result_filename}')
+    document.save(result_filename)
```

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_admin_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_admin_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import datetime
 import logging
 
 from typing import Optional, List
-from debater_python_api.api.clients.keypoints_client import KpAnalysisClient
+from debater_python_api.api.clients.keypoints_client import KpsClient
 
 admin_reports_endpoint = '/admin_report'
 admin_actions_endpoint = '/admin_action'
 
-class KpAnalysisAdminClient(KpAnalysisClient):
-    def __init__(self, admin_password, apikey: str, host: Optional[str]=None):
-        super().__init__(apikey, host)
+class KpsAdminClient(KpsClient):
+    def __init__(self, admin_password, apikey: str, host: Optional[str]=None, verify_certificate: bool = True):
+        super().__init__(apikey, host, verify_certificate)
         self.admin_password = admin_password
 
     def get_admin_password_header(self, admin_password):
         return {'admin-password': self.admin_password}
 
     def admin_report_get_domain_statuses(self):
         res = self._get(self.host + admin_reports_endpoint, {'report': 'domain_statuses'},
@@ -55,14 +55,28 @@
     def admin_report_get_not_finished_comment_batches(self):
         res = self._get(self.host + admin_reports_endpoint,
                         {'report': 'comment_batches_statuses'},
                         headers=self.get_admin_password_header(self.admin_password))
         logging.info(f'not_done_comment_batches: {len(res)}')
         return res
 
+    def admin_report_get_comments_stats(self, user_id=None, since_date=None, till_date=None):
+        params = {'admin_password': self.admin_password, 'report': 'comments_stats'}
+        if user_id is not None:
+            params['user_id'] = str(user_id)
+        if since_date is not None:
+            params['since_date'] = since_date.strftime("%m/%d/%Y, %H:%M:%S")
+        if till_date is not None:
+            params['till_date'] = till_date.strftime("%m/%d/%Y, %H:%M:%S")
+
+        res = self._get(self.host + admin_reports_endpoint, params,
+                        headers=self.get_admin_password_header(self.admin_password))
+        logging.info(f'comments_stats: {len(res)}')
+        return res
+
     def admin_action_delete_user(self, user_id: str):
         res = self._get(self.host + admin_actions_endpoint,
                         {'action': 'delete_user', 'user_id': user_id},
                         headers=self.get_admin_password_header(self.admin_password))
         logging.info(f'delete_users: {res}')
         return res
```

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,169 @@
+import json
 import logging
 import time
 import calendar
 import traceback
+from enum import Enum
 
+import pandas as pd
 import requests
-from debater_python_api.api.clients.abstract_client import AbstractClient
-from debater_python_api.utils.general_utils import get_default_request_header
-from typing import List, Optional, Dict
-from debater_python_api.utils.kp_analysis_utils import print_progress_bar
-from debater_python_api.api.clients.key_point_analysis.KpaExceptions import KpaIllegalInputException
+
+from debater_python_api.api.clients.key_point_summarization.KpsResult import KpsResult
+from debater_python_api.api.clients.key_point_summarization.utils import get_default_request_header, \
+    update_row_with_stance_data, validate_api_key_or_throw_exception, print_progress_bar, is_list_of_strings
+
+from typing import List, Optional, Dict, Union, Any
+from debater_python_api.api.clients.key_point_summarization.KpsExceptions import KpsIllegalInputException, \
+    KpsNoPrivilegesException, KpsInvalidOperationException
 
 domains_endpoint = '/domains'
 comments_endpoint = '/comments'
 kp_extraction_endpoint = '/kp_extraction'
 data_endpoint = '/data'
 report_endpoint = '/report'
 comments_limit_endpoint = '/comments_limit'
 self_check_endpoint = '/self_check'
 
+class Stance(Enum):
+    PRO = "pro"
+    CON = "con"
+    NO_STANCE = "no-stance"
+    EACH_STANCE = "each-stance"
 
-class KpAnalysisClient(AbstractClient):
+class KpsClient():
     '''
-    A client for the Key Point Analysis (KPA) service.
+    A client for the Key Point Summarization (KPS) service.
     '''
     def __init__(self, apikey: str, host: Optional[str] = None, verify_certificate: bool = True):
         '''
-        :param apikey: user's api-key, should be retreived from the early-access-program site.
-        :param host: optional, enable switching to alternative services.
-        '''
-        AbstractClient.__init__(self, apikey)
+        :param apikey: User's api-key, should be retreived from the early-access-program site.
+        :param host: Optional, enable switching to alternative services.
+        :param verify_certificate: Optional, will not verify the server's certificate when set to False. Useful when using a self-signed certificate.
+        '''
+        validate_api_key_or_throw_exception(apikey)
+        self.apikey = apikey
+        self.show_process = True
         self.host = host if host is not None else 'https://keypoint-matching-backend.debater.res.ibm.com'
         self.verify_certificate = verify_certificate
+        self.api_version = "2"
 
-    def _delete(self, url, params, use_cache=True, timeout=300, retries=10, headers=None):
-        return self._run_request_with_retry(requests.delete, url, params, use_cache, timeout, retries, headers)
+    def _delete(self, url, params, timeout=300, retries=10, headers=None):
+        return self._run_request_with_retry(requests.delete, url, params, timeout, retries, headers)
 
-    def _get(self, url, params, use_cache=True, timeout=300, retries=10, headers=None):
-        return self._run_request_with_retry(requests.get, url, params, use_cache, timeout, retries, headers)
+    def _get(self, url, params, timeout=300, retries=10, headers=None):
+        return self._run_request_with_retry(requests.get, url, params, timeout, retries, headers)
 
-    def _post(self, url, body, use_cache=True, timeout=300, retries=10, headers=None):
-        return self._run_request_with_retry(requests.post, url, body, use_cache, timeout, retries, headers)
+    def _post(self, url, body, timeout=300, retries=10, headers=None):
+        return self._run_request_with_retry(requests.post, url, body, timeout, retries, headers)
 
-    def _run_request_with_retry(self, func, url, params, use_cache=True, timeout=20, retries=10, headers_input=None):
+    def _run_request_with_retry(self, func, url, params, timeout=20, retries=10, headers_input=None):
         headers = get_default_request_header(self.apikey)
         if headers_input is not None:
             headers.update(headers_input)
 
+        KpsClient._validate_request(params)
+        params["api_version"] = self.api_version
         logging.info('client calls service (%s): %s' % (func.__name__, url))
-        if not use_cache:
-            headers['cache-control'] = 'no-cache'
-
         while True:
             try:
                 if func.__name__ == 'post':
                     resp = func(url, json=params, headers=headers, timeout=timeout, verify=self.verify_certificate)
                 else:
                     resp = func(url, params=params, headers=headers, timeout=timeout, verify=self.verify_certificate)
                 if resp.status_code == 200:
                     return resp.json()
                 if resp.status_code == 422:
                     msg = 'There is a problem with the request (%d): %s' % (resp.status_code, resp.reason)
                     logging.error(msg)
-                    raise KpaIllegalInputException(msg)
+                    raise KpsIllegalInputException(msg)
+                if resp.status_code == 403:
+                    msg = 'User is not authorized to perform the requested operation (%d): %s' % (resp.status_code, resp.reason)
+                    logging.error(msg)
+                    raise KpsNoPrivilegesException(msg)
                 msg = 'Failed calling server at %s: (%d) %s' % (url, resp.status_code, resp.reason)
-            except KpaIllegalInputException as e:
+            except (KpsIllegalInputException, KpsNoPrivilegesException) as e:
                 raise e
             except Exception as e:
                 track = traceback.format_exc()
                 msg = "Can't access server at {}. Exception: {}".format(url, track)
 
             retries -= 1
             if retries < 0:
                 raise ConnectionError(msg)
             else:
                 logging.warning('%s, retries left: %d' % (msg, retries))
                 time.sleep(10)
 
-    def _is_list_of_strings(self, lst):
-        return isinstance(lst, list) and len([a for a in lst if not isinstance(a, str)]) == 0
-
-    def create_domain(self, domain, domain_params=None):
-        '''
+    def create_domain(self, domain:str, domain_params:Optional[Dict[str, Union[str, int, bool]]] = None, ignore_exists:Optional[bool] = False) -> None:
+        """
         Create a new domain and customize domain's parameters.
-        By default, comments that are uploaded into a domain are over go minor cleansing and then split into sentences.
-        However, sometimes users have better domain-knowledge and prefer to handle their data themselves.
-        Therefore, users that want to clean their comments and split them into sentences can use the dont_split parameter and set it to True,
-        and the uploaded comments will be kept as is.
         :param domain: the name of the new domain (must not exist already)
-        :param domain_params: a dictionary with various parameters for the domain. Supported values:
-        * dont_split: (Boolean, set to False by default), when set to True, the comments uploaded to the domain will not be cleaned and not be split into sentences.
-        * do_stance_analysis: (Boolean, set to False by default), when set to True, stance (positive, negative, neutral, suggestion) is calculated for all sentences (needed when we want to run on each stance seperatly).
-        * do_kp_quality: (Boolean, set to False by default), When set to true, keypoint quality is calculated for all sentences (needed when we want to use the kp_quality model for key point selection).
-        '''
-        body = {'domain': domain}
-        if domain_params is not None:
-            body['domain_params'] = domain_params
-
-        self._post(url=self.host + domains_endpoint, body=body)
-        logging.info('created domain: %s with domain_params: %s' % (domain, str(domain_params)))
-
+        :param domain_params: optional, a dictionary with various parameters for the domain.
+        For full documentation of the domain
+        params see https://github.com/IBM/debater-eap-tutorial/blob/main/survey_usecase/kps_parameters.pdf
+        :param ignore_exists: optional, default False. When the domain already exists - if True, keeps existing domain.
+        If False, raises an exception.
+        """
+        try:
+            body = {'domain': domain}
+            if domain_params is not None:
+                KpsClient._validate_params_dict(domain_params, "domain")
+                body['domain_params'] = domain_params
+            self._post(url=self.host + domains_endpoint, body=body)
+            logging.info('created domain: %s with domain_params: %s' % (domain, str(domain_params)))
+        except KpsIllegalInputException as e:
+            if 'already exist' not in str(e):
+                raise e
+            if not ignore_exists:
+                raise KpsIllegalInputException(f'domain: {domain} already exists. To run on a new domain, please either select another '
+                             f'domain name or delete this domain first by running client.delete_domain_cannot_be_undone({domain}).'
+                             f'To allow running on an existing domain set ignore_exists=True ')
+
+            logging.info(f'domain: {domain} already exists, domain_params are NOT updated.')
+
+    def upload_comments(self, domain: str, comments_ids: List[str], comments_texts: List[str]) -> None:
+        """
+        Uploads comments into a domain. It is mandatory to create a domain before uploading comments into it.
+        Re-uploading the same comments (same domain + comment_id + text) is relatively quick.
+        Uploading an the same comment_id with a different text will raise an exception.
+        Processing comments (cleaning + sentence splitting + calculating scores) takes some time. The progress will
+        be displayed on screen and the method will return only when all comments are processed.
+        :param domain: the name of the domain to upload the comments into. (usually one  per data-set).
+        :param comments_ids: a list of comment ids (strings), comment ids must be unique, and composed of alphanumeric characters,
+        spaces and underscores only.
+        :param comments_texts: a list of comments (strings), this list must be the same length as comments_ids and the comment_id and comment_text should match by position in the list.
+        """
+        self.upload_comments_async(domain, comments_ids, comments_texts)
+        logging.info('waiting for the comments to be processed')
+        self.wait_till_all_comments_are_processed(domain)
 
-    def upload_comments(self, domain: str, comments_ids: List[str], comments_texts: List[str], batch_size: int = 2000) -> None:
+    def upload_comments_async(self, domain: str, comments_ids: List[str], comments_texts: List[str]) -> None:
         '''
-        Uploads comments into a domain. It is not mandatory to create a domain before uploading comments into it.
-        If the domain doesn't exist, a domain with default parameters will be created.
-        When we need to change domain's parameters, we must create it first via create_domain method.
-        Re-uploading the same comments (same domain + comment_id, text is ignored) is not problematic (and relativly quick).
-        Processing comments (cleaning + sentence splitting + calculating quality etc.) takes some time,
-        please wait for it to finish before starting a key point analysis job (using method wait_till_all_comments_are_processed).
+        Uploads comments into a domain in an async manner.
+        It is mandatory to create a domain before uploading comments into it.
+        Re-uploading the same comments (same domain + comment_id + text) is relatively quick.
+        Uploading an the same comment_id with a different text will raise an exception.
+        Processing comments (cleaning + sentence splitting + calculating scores) takes some time,
+        please wait for it to finish before starting a key point summarization job, using get_comments_status or are_all_comments_processed.
         :param domain: the name of the domain to upload the comments into. (usually one  per data-set).
         :param comments_ids: a list of comment ids (strings), comment ids must be unique.
         :param comments_texts: a list of comments (strings), this list must be the same length as comments_ids and the comment_id and comment_text should match by position in the list.
-        :param batch_size: the number of comments that will be uploaded in every REST-API call.
         '''
         assert len(comments_ids) == len(comments_texts), 'comments_texts and comments_ids must be the same length'
-        assert len(comments_ids) == len(set(comments_ids)), 'comment_ids must be unique'
-        assert self._is_list_of_strings(comments_texts), 'comment_texts must be a list of strings'
-        assert self._is_list_of_strings(comments_ids), 'comment_ids must be a list of strings'
+        assert len(comments_ids) == len(set(comments_ids)), 'comments_ids must be unique'
+        assert is_list_of_strings(comments_texts), 'comment_texts must be a list of strings'
+        assert is_list_of_strings(comments_ids), 'comments_ids must be a list of strings'
         assert len([c for c in comments_texts if c is None or c == '' or len(c) == 0 or c.isspace()]) == 0, 'comment_texts must not have an empty string in it'
-        assert len([c for c in comments_texts if len(c) > 3000]) == 0, 'comment_texts must be shorter than 3000 charachters'
+        assert len([c for c in comments_texts if len(c)>3000]) == 0, 'comment_texts must be shorter than 3000 characters'
         logging.info('uploading %d comments in batches' % len(comments_ids))
 
         ids_texts = list(zip(comments_ids, comments_texts))
+        ids_texts.sort(key=lambda t: len(t[1]))
+        batch_size = 2000
         uploaded = 0
         batches = [ids_texts[i:i + batch_size] for i in range(0, len(ids_texts), batch_size)]
         for batch in batches:
             comments_ids = [t[0] for t in batch]
             comments_texts = [t[1] for t in batch]
             body = {'domain': domain,
                     'comments_ids': comments_ids,
@@ -134,91 +172,190 @@
             self._post(url=self.host + comments_endpoint, body=body, retries=10)
             uploaded += len(batch)
             logging.info('uploaded %d comments, out of %d' % (uploaded, len(ids_texts)))
 
     def get_comments_status(self, domain: str) -> Dict[str, int]:
         '''
         Get the status of the comments in a domain.
+        All comments are processed and a kps job can start when there are no more pending comments.
         :param domain: the name of the domain
         :return: a dictionary with the status:
         * processed_comments: number of comments that where already processed
         * pending_comments: number of comments that still need to be processed
         * processed_sentences: number of sentences after sentence-splitting the processed comments
         '''
         res = self._get(self.host + comments_endpoint, {'domain': domain})
         logging.info('domain: %s, comments status: %s' % (domain, str(res)))
         return res
 
-    def wait_till_all_comments_are_processed(self, domain: str, polling_timout_secs: Optional[int] = None) -> None:
+    def are_all_comments_processed(self, domain: str) -> bool:
+        """
+        Check if all comments in the domain are processed.
+        :param domain: the name of the domain
+        :return: True if all comments uploaded to the domain are processed.
+        """
+        res = self.get_comments_status(domain)
+        return res['pending_comments'] == 0
+
+    def wait_till_all_comments_are_processed(self, domain: str, polling_timeout_secs: Optional[int] = None) -> None:
         '''
         Waits for all comments in a domain to be processed.
         :param domain: the name of the domain
+        :param polling_timeout_secs: optional, polling time in seconds
         '''
         while True:
             res = self.get_comments_status(domain)
             if res['pending_comments'] == 0:
                 break
-            time.sleep(polling_timout_secs if polling_timout_secs is not None else 10)
+            time.sleep(polling_timeout_secs if polling_timeout_secs is not None else 10)
 
-    def start_kp_analysis_job(self, domain: str, comments_ids: Optional[List[str]] = None,
-                              run_params = None, description: Optional[str] = None, use_cache: bool = True) -> 'KpAnalysisTaskFuture':
+    @staticmethod
+    def _get_run_params_with_stance(run_params, stance):
+        if stance == Stance.NO_STANCE.value or not stance:
+            return run_params
+        if not run_params:
+            run_params = {}
+        else:
+            assert "stances_to_run" not in run_params, "run_param 'stances_to_run' is no longer supported, please use the 'stance' method parameter instead."
+            assert "stance" not in run_params, "run_param 'stance' is set interanlly by the client, please use the 'stance' method parameter instead."
+            run_params = run_params.copy()
+
+        if stance == Stance.PRO.value:
+            run_params['stance'] = "PRO"
+        elif stance == Stance.CON.value:
+            run_params['stance'] = "CON"
+        else:
+            raise KpsIllegalInputException(f"Unsupported stance: *{stance}*, supported: no-stance, pro, con.")
+        return run_params
+
+    def run_full_kps_flow(self, domain: str, comments_texts: List[str],
+                          stance: Optional[str] = Stance.EACH_STANCE.value):
+        '''
+        This is the simplest way to use the Key Point Summarization system.
+        This method uploads the comments into a temporary domain, waits for them to be processed,
+        starts a Key Point Summarization job using all comments, and waits for the results. Eventually, the domain is deleted.
+        It is possible to use this method for up to 10000 comments. For longer jobs, please run the system in a staged
+        manner (upload the comments yourself, start a job etc').
+        If execution stopped before this method returned, please run client.delete_domain_cannot_be_undone(<domain>)
+        to free resources and avoid longer waiting in future calls.  TODO Remove comment?
+        :param domain: name of the temporary domain to store the comments. must not be a name of an existing domain, or
+        an error will be raised. The domain must be composed of alphanumeric characters, spaces and underscores only.
+        :param comments_texts: a list of comments (strings).
+        :param stance: Optional, If "no-stance" - run on all the data disregarding the stance.
+        If "pro", run on positive sentences only, if "con", run on con sentences (negative and suggestions).
+        If "each-stance", starts two kps jobs, one for each stance, and returns the merged result object.
+        :return: a KpsResult object with the result
         '''
-        Starts a Key Point Analysis (KPA) job in an async manner. Please make sure all comments had already been uploaded into a domain and processed before starting a new job (using the wait_till_all_comments_are_processed method).
-          * By default it runs over all comments in the domain. In order to run only on a subset of the comments in the domain, pass their ids in the comment_ids param.
-          * It is also possible to add a job description. This description will later be visible in the user-report.
-          * Every domain has a cache. When running a new job, only the delta from previous jobs in the same domain is calculated.
-          * Different parameters that affect the job and its result can be passed in the run_params parameter:
-              * keypoints (List of strings, empty by default): When keypoints are provided the service matches the sentences to the given keypoints instead of extracting them automatically.
-              This enables a human-in-the-loop scenario, where the automatically extracted key points are reviewed by the user, and the sentences are then remapped to the revised keypoints.
-              * keypoints_by_job_id (String, empty by default): It is also possible to use key points from a previous job by suppling the job_id in the keypoints_by_job_id param.
-              Note that only one of the keypoints and keypoints_by_job_id params can be used, not both.
-              * arg_min_len (Integer, set to 4 by default): Filter shorter sentences (by number of tokens).
-              * arg_max_len (Integer, set to 36 by default): Filter longer sentences (by number of tokens).
-              * arg_relative_aq_threshold (Float in [0.0,1.0], set to 1.0 by default): Filter sentences having a quality score below this precentile (useful to filter out low quality data in the data-set).
-              * mapping_policy (String in ["STRICT","NORMAL","LOOSE"], "NORMAL" by default): Policy for determining if an argument is matched to a key point: for “STRICT”, only pairs with high matching
-              scores are considered matched, leading to a higher precision and a lower coverage, and vice versa for "LOOSE".
-              * sentence_to_multiple_kps (Boolean, False by default): When True, a sentence is matched to all key points with score above threshold. Otherwise only to one key point with highest match score above threshold.
-              * n_top_kps (Integer, default is set by an internal algorithm): Number of key points to generate. Lower value will make the job finish faster. All sentences are re-mapped to these key point.
-              * kp_relative_aq_threshold (Float in [0.0,1.0], set to 0.65 by default): Sentences having AQ score below this precentile will not be selected as key point candidates.
-              * invalid_kps_comment_ids (String list, empty by default): A list of comment_ids who’s sentences should not be selected as key point candidates.
+        if len(comments_texts) > 10000:
+            raise Exception(
+                'Please use the stagged mode (upload_comments, run_kps_job) for jobs with more then 10000 comments')
+        try:
+            self.create_domain(domain, ignore_exists=False)
+            comments_ids = [str(i) for i in range(len(comments_texts))]
+            self.upload_comments(domain, comments_ids, comments_texts)
+            if stance == Stance.EACH_STANCE.value:
+                keypoint_matching = self.run_kps_job_both_stances(domain)
+            else:
+                keypoint_matching = self.run_kps_job(domain, stance=stance)
+            return keypoint_matching
+        except KpsIllegalInputException as e:
+            if 'already exist' in str(e):
+                raise KpsIllegalInputException(f'Domain {domain} already exists. Please use a new domain name or delete the domain using '
+                                               f'delete_domain_cannot_be_undone() to run the full flow. If you wish to run kps on the existing domain, please'
+                                               f'use the methods run_kps_job or run_kps_job_both_stances')
+            else:
+                raise e
+        finally:
+            self.delete_domain_cannot_be_undone(domain)
+
+    def run_kps_job_both_stances(self, domain: str, comments_ids: Optional[List[str]]=None,
+                                 run_params_pro:Optional[Dict[str, Any]] = None,
+                                 run_params_con:Optional[Dict[str, Any]] = None,
+                                 description: Optional[str] = None):
+        """
+        Starts two kps jobs simultaneously, one for pro sentences and one for con sentences, and returns a merge KpsResult.
         :param domain: the name of the domain
-        :param comments_ids: when None is passed, it uses all comments in the domain (typical usage) otherwise it only uses the comments according to the provided list of comment_ids.
-        :param run_params: a dictionary with different parameters and their values (see description above). e.g. run_param={'arg_min_len': 5, 'arg_max_len': 40, 'mapping_threshold': 0.0}
-        :param description: add a description to a job so it will be easy to detecte it in the user-report.
-        :param use_cache: determines whether the cache is used (should be kept as True for faster more efficient runs).
-        :return: KpAnalysisTaskFuture: an object that enables the retrieval of the results in an async manner.
-        '''
+        :param comments_ids: optional, when None is passed, it uses all comments in the domain (typical usage) otherwise it only uses the comments according to the provided list of comments_ids.
+        :param run_params_pro: optional,a dictionary with different parameters and their values, to be sent to the pro kps job.
+        :param run_params_con: optional,a dictionary with different parameters and their values, to be sent to the con kps job.
+        For full documentation of supported run_params see https://github.com/IBM/debater-eap-tutorial/blob/main/survey_usecase/kpa_parameters.pdf
+        :param description: optional, add a textual description to a job so it will be easy to detect it in the user-report. for each job, the stance will be appended to the description.,
+        the stance of each job will be added to the description
+        :return: a KpsResult object with the merged pro and con result.
+        """
+        description_pro = (description + " (pro)") if description else None
+        description_con = (description + " (con)") if description else None
+        future_pro = self.run_kps_job_async(domain, comments_ids, stance=Stance.PRO.value, run_params=run_params_pro, description = description_pro)
+        future_con = self.run_kps_job_async(domain, comments_ids, stance=Stance.CON.value, run_params=run_params_con, description = description_con)
+        result_pro = future_pro.get_result()
+        result_con = future_con.get_result()
+        return KpsResult.get_merged_pro_con_results(pro_result=result_pro, con_result=result_con)
+
+    def run_kps_job(self, domain: str, comments_ids: Optional[List[str]]=None,
+                    run_params: Optional[Dict[str, Any]] = None,
+                    description: Optional[str] = None, stance: Optional[str]=Stance.NO_STANCE.value) -> 'KpsResult':
+        """
+        Runs Key Point Summarization (KPS) in a synchronous manner: starts the job, waits for the results and return them.
+        Please make sure all comments had already been uploaded into a domain and processed before starting a new job (using the get_comments_status or are_all_comments_processed methods).
+        :param domain: the name of the domain
+        :param comments_ids: optional, when None is passed, it uses all comments in the domain (typical usage) otherwise it only uses the comments according to the provided list of comments_ids.
+        :param run_params: optional,a dictionary with different parameters and their values. For full documentation of supported run_params see https://github.com/IBM/debater-eap-tutorial/blob/main/survey_usecase/kpa_parameters.pdf
+        :param description: optional, add a textual description to a job so it will be easy to detect it in the user-report.
+        :param stance: Optional, default to "no-stance". If "no-stance" - run on all the data disregarding the stance.
+        If "pro", run on positive sentences only, if "con", run on con sentences (negative and suggestions).
+        :return: a KpsResult object with the result.
+        """
+        future = self.run_kps_job_async(domain, run_params=run_params, comments_ids=comments_ids, stance=stance, description=description)
+        keypoint_matching = future.get_result(high_verbosity=True)
+        return keypoint_matching
 
-        # TODO validate run_params
+    def run_kps_job_async(self, domain: str, comments_ids: Optional[List[str]]=None,
+                          stance: Optional[str] = Stance.NO_STANCE.value,
+                          run_params: Optional[Dict[str, Any]] = None, description: Optional[str] = None) -> 'KpsJobFuture':
+        """
+        Starts a Key Point Summarization (KPS) job in an async manner. Please make sure all comments had already been
+        uploaded into a domain and processed before starting a new job (using the using get_comments_status or are_all_comments_processed methods).
+        :param domain: the name of the domain
+        :param comments_ids: optional, when None is passed, it uses all comments in the domain (typical usage) otherwise it only uses the comments according to the provided list of comments_ids.
+        :param run_params: optional, a dictionary with different parameters and their values. For full documentation of supported run_params see https://github.com/IBM/debater-eap-tutorial/blob/main/survey_usecase/kpa_parameters.pdf
+        :param stance: Optional, default to "no-stance". If "no-stance" - run on all the data disregarding the stance.
+        If "pro", run on positive sentences only, if "con", run on con sentences (negative and suggestions).
+        :param description: optional, add a textual description to a job so it will be easy to detect it in the user-report.
+        :return: KpsJobFuture: an object that enables the retrieval of the results in an async manner
+        """
+        if not self.are_all_comments_processed(domain):
+            raise KpsInvalidOperationException(f"Attempt to start a KPS job on domain {domain} when comments"
+                                               f" are still processing. Please wait until all comments are processed"
+                                               f" before starting a kps job. You can test the comments status using the"
+                                               f"methods are_all_comments_processed({domain}) or get_comments_status({domain})")
+        run_params = KpsClient._get_run_params_with_stance(run_params, stance)
         body = {'domain': domain}
 
         if comments_ids is not None:
+            assert is_list_of_strings(comments_ids), 'comments_ids must be a list of strings'
             body['comments_ids'] = comments_ids
 
         if run_params is not None:
+            KpsClient._validate_params_dict(run_params, 'run')
             body['run_params'] = run_params
 
         if description is not None:
             body['description'] = description
 
-        res = self._post(url=self.host + kp_extraction_endpoint, body=body, use_cache=use_cache)
-        logging.info(f'started a kp analysis job - domain: {domain}, run_params: {run_params}, {"" if description is None else f"description: {description}, "}job_id: {res["job_id"]}')
-        return KpAnalysisTaskFuture(self, res['job_id'])
+        res = self._post(url=self.host + kp_extraction_endpoint, body=body)
+        logging.info(f'started a kp summarization job - domain: {domain}, stance: {stance}, run_params: {run_params}, {"" if description is None else f"description: {description}, "}job_id: {res["job_id"]}')
+        return KpsJobFuture(self, res['job_id'])
 
-    def get_kp_extraction_job_status(self, job_id: str, top_k_kps: Optional[int] = None,
+    def get_kps_job_status(self, job_id: str, top_k_kps: Optional[int] = None,
                                      top_k_sentences_per_kp: Optional[int] = None):
         '''
-        Checks for the status of a key point analysis job. It returns a json with a 'status' key that can have one of the following values: PENDING, PROCESSING, DONE, CANCELED, ERROR
-        If the status is PROCESSING, it also have a 'progress' key that describes the calculation progress.
-        If the status is DONE, it also have a 'result' key that has the result json.
-        If the status is ERROR, it also have a 'error_msg' key that has the description of the error.
-        The result json have the following structure:
-            * 'keypoint_matchings': a list of keypoint_matching (key point and its matched sentences). Sorted descendingly according to number of matched sentences. each keypoint_matching have:
-                * 'keypoint': the key point (string).
-                * 'matching': a list of matches (sentences that match the key point). each match have the sentences details ('domain', 'comment_id', 'sentence_id', 'sents_in_comment', 'span_start', 'span_end', 'num_tokens', 'argument_quality', 'sentence_text') and a match score ('score') this is the match score between the sentence and the key point. The matchings are sorted descendingly according to their match score.
+        Checks for the status of a key point summarization job. It returns a json with a 'status' key that can have one of the following values: PENDING, PROCESSING, DONE, CANCELED, ERROR
+        If the status is PROCESSING, it also has a 'progress' key that describes the calculation progress.
+        If the status is DONE, it also has a 'result' key that has the result_json, that can be converted into KpsResults using KpsResult.create_from_result_json(result_json)
+        If the status is ERROR, it also has a 'error_msg' key that has the description of the error.
         :param job_id: the job_id (can be found in the future returned when the job was started or in the user-report)
         :param top_k_kps: use this parameter to truncate the result json to have only the top K key points.
         :param top_k_sentences_per_kp: use this parameter to truncate the result json to have only the top K matched sentences per key point.
         :return: see description above.
         '''
         params = {'job_id': job_id}
 
@@ -226,197 +363,307 @@
             params['top_k_kps'] = top_k_kps
 
         if top_k_sentences_per_kp is not None:
             params['top_k_sentences_per_kp'] = top_k_sentences_per_kp
 
         return self._get(self.host + kp_extraction_endpoint, params, timeout=180)
 
-    def run(self, comments_texts: List[str], comments_ids: Optional[List[str]]=None):
+    def cancel_kps_job(self, job_id: str):
         '''
-        This is the simplest way to use the Key Point Analysis system.
-        This method uploads the comments into a temporary domain, waits for them to be processed, starts a Key Point Analysis job using all comments (auto key points extraction with default parameters), and waits for the results. Eventually, the domain is deleted.
-        It is possible to use this method for up to 1000 comments. For longer jobs, please run the system in a stagged manner (upload the comments yourself, start a job etc').
-        :param comments_texts: a list of comments (strings).
-        :param comments_ids: (optional) a list of comment ids (a list of strings). When not provided, dummy comment_ids will be generated (1, 2, 3,...). When provided, comment_ids must be unique, must be the same length as comments_texts and the comment_id and comment_text should match by position in the list.
-        :return: a json with the result
-        '''
-        if len(comments_texts) > 10000:
-            raise Exception('Please use the stagged mode (upload_comments, start_kp_analysis_job) for jobs with more then 10000 comments')
-
-        if comments_ids is None:
-            comments_ids = [str(i) for i in range(len(comments_texts))]
-        domain = 'run_temp_domain_' + str(calendar.timegm(time.gmtime()))
-        logging.info('uploading comments')
-        self.upload_comments(domain, comments_ids, comments_texts)
-        logging.info('waiting for the comments to be processed')
-        self.wait_till_all_comments_are_processed(domain)
-        logging.info('starting the key point analysis job')
-        future = self.start_kp_analysis_job(domain)
-        logging.info('waiting for the key point analysis job to finish')
-        keypoint_matching = future.get_result(high_verbosity=True)
-        self.delete_domain_cannot_be_undone(domain)
-        return keypoint_matching
-
-    def cancel_kp_extraction_job(self, job_id: str):
-        '''
-        Stops a running key point analysis job.
+        Stops a running key point summarization job.
         :param job_id: the job_id
         :return: the request's response
         '''
-        return self._delete(self.host + kp_extraction_endpoint, {'job_id': job_id})
+        logging.info(f"Canceling job {job_id}")
+        try:
+            return self._delete(self.host + kp_extraction_endpoint, {'job_id': job_id})
+        except KpsIllegalInputException as e:
+            return
 
-    def cancel_all_extraction_jobs_for_domain(self, domain: str, clear_kp_analysis_jobs_log: bool = False):
+    def cancel_all_kps_jobs_for_domain(self, domain: str):
         '''
         Stops all running jobs and cancels all pending jobs in a domain.
         :param domain: the name of the domain.
-        :param clear_kp_analysis_jobs_log: When set to True, clears all jobs in this domain from the jobs-history in the user-report (useful when the report becomes too long).
         :return: the request's response
         '''
-        return self._delete(self.host + data_endpoint, {'domain': domain, 'clear_kp_analysis_jobs_log': clear_kp_analysis_jobs_log, 'clear_db': False})
+        logging.info(f"Canceling all jobs for domain {domain}")
+        return self._delete(self.host + data_endpoint, {'domain': domain, 'clear_kp_analysis_jobs_log': False, 'clear_db': False})
 
-    def cancel_all_extraction_jobs_all_domains(self, clear_kp_analysis_jobs_log: bool = False):
+    def cancel_all_kps_jobs_all_domains(self):
         '''
         Stops all running jobs and cancels all pending jobs in all domains.
-        :param clear_kp_analysis_jobs_log: When set to True, also clears all jobs (in all domains) from the jobs-history in the user-report (useful when the repots becomes too long).
         :return: the request's response
         '''
-        return self._delete(self.host + data_endpoint, {'clear_kp_analysis_jobs_log': clear_kp_analysis_jobs_log, 'clear_db': False})
+        logging.info(f"Canceling all jobs for all domains.")
+        return self._delete(self.host + data_endpoint, {'clear_kp_analysis_jobs_log': False, 'clear_db': False})
 
-    def delete_domain_cannot_be_undone(self, domain: str, clear_kp_analysis_jobs_log: bool = False):
+    def delete_domain_cannot_be_undone(self, domain: str):
         '''
         Deletes a domain. Stops all running jobs and cancels all pending jobs in a domain. Erases the data (comments and sentences) in a domain and clears the domain's cache.
         When uploaded comments in a domain need to be replaced, first delete the domain and then upload the updated comments.
         :param domain: the name of the domain
-        :param clear_kp_analysis_jobs_log: When set to True, also clears all jobs in the domain from the jobs-history in the user-report (useful when the repots becomes too long).
         :return: the request's response
         '''
-        return self._delete(self.host + data_endpoint, {'domain': domain, 'clear_kp_analysis_jobs_log': clear_kp_analysis_jobs_log, 'clear_db': True})
+        try:
+            resp = self._delete(self.host + data_endpoint, {'domain': domain, 'clear_kp_analysis_jobs_log': False, 'clear_db': True})
+            logging.info(f'domain: {domain} was deleted')
+            return resp
+        except KpsIllegalInputException as e:
+            if 'doesn\'t have domain' not in str(e):
+                raise e
+            logging.info(f'domain: {domain} doesn\'t exist.')
 
-    def delete_all_domains_cannot_be_undone(self, clear_kp_analysis_jobs_log: bool = False):
+    def delete_all_domains_cannot_be_undone(self):
         '''
         Deletes all user's domains. Stops all running jobs and cancels all pending jobs in all domains. Erases the data (comments and sentences) in all domains and clears all domains' caches.
-        :param clear_kp_analysis_jobs_log: When set to True, also clears all jobs (in all domains) from the jobs-history in the user-report (useful when the repots becomes too long).
         :return: the request's response
         '''
-        return self._delete(self.host + data_endpoint, {'clear_kp_analysis_jobs_log': clear_kp_analysis_jobs_log, 'clear_db': True})
+        return self._delete(self.host + data_endpoint, {'clear_kp_analysis_jobs_log': False, 'clear_db': True})
 
     def get_full_report(self, days_ago=30):
         '''
         Retreives a json with the user's report.
-        :param days_ago: key point analysis jobs older then this parameter will be filtered out
+        :param days_ago: key point summarization jobs older then this parameter will be filtered out
         returns: The report which consists:
           * 'comments_status': all the domains that the user have and the current status of each domain (number of processed comments, sentences and comments that still need to be processed, similar to get_comments_status method).
-          * 'kp_analysis_status': a list of all key point analysis jobs that the user have/had with all the relevant details and parameters for each job.
+          * 'kp_summarization_status': a list of all key point summarization jobs that the user have/had with all the relevant details and parameters for each job.
         '''
         return self._get(self.host + report_endpoint, {'days_ago': days_ago}, timeout=180)
 
-    def get_comments_limit(self):
+    def get_comments_limit(self) -> int:
         '''
-        Retreives a json with the permitted number of comments per KPA job.
+        Retreives a json with the permitted number of comments per KPS job.
         returns:
-          * 'n_comments_limit': The maximal number of comments permitted per KPA job (None if there is no limit).
+          * 'n_comments_limit': The maximal number of comments permitted per KPS job (None if there is no limit).
         '''
         return self._get(self.host + comments_limit_endpoint, {}, timeout=180)
 
     def run_self_check(self):
         '''
         Checks the connection to the service and if the service is UP and running.
         :return: a json with 'status': that have the value UP if all is well and DOWN otherwise.
         '''
         return self._get(self.host + self_check_endpoint, None, timeout=180)
 
+    def get_unmapped_sentences_for_kps_result(self, kps_result: KpsResult):
+        '''
+        Retrieve all unmapped sentences associated with the kps_result.
+        :param kps_result: KpsResult object storing the results.
+        :return: a dataframe with all unmapped sentences and their data, or None if domain
+        '''
+        domain = kps_result.get_domain()
+        job_ids = list(kps_result.get_stance_to_job_id().values())
+        sentences_dfs = []
+
+        if len(job_ids) == 1:
+            sents_df = self.get_sentences_for_domain(domain, job_ids[0])
+        elif len(job_ids) == 2:
+            for job_id in job_ids:
+                sents_df = self.get_sentences_for_domain(domain, job_id)
+                sentences_dfs.append(sents_df)
+            sents_df = pd.concat(sentences_dfs).drop_duplicates(subset=["comment_id","sent_id"])
+
+        if len(sents_df) == 0:
+            logging.info("No sentences found for result, maybe the domain was deleted?")
+            return None
+
+        mapped_sents_df = kps_result.result_df.rename(columns={"sentence_id":"sent_id"})
+        unmapped_sents_df = pd.concat([sents_df,mapped_sents_df]).drop_duplicates(subset=["sent_id","comment_id"], keep=False)
+        unmapped_sents_df = unmapped_sents_df[sents_df.columns]
+        return unmapped_sents_df
+
     def get_sentences_for_domain(self, domain: str, job_id: Optional[str] = None):
         '''
         Uploaded comments are cleaned and split into sentences. This method retrieves the sentences in a domain.
         :param domain: the name of the domain.
-        :param job_id: when provided, it will only return the sentences used in a specific key point analysis job.
-        :return: a dictionary with all the sentences' details.
+        :param job_id: when provided, it will only return the sentences used in a specific key point summarization job.
+        :return: a dataframe with all the sentences' data.
         '''
-        res = self._get(self.host + data_endpoint, {'domain': domain, 'get_sentences': True, 'job_id': job_id})
+        params = {'domain': domain, 'get_sentences': True}
+        if job_id:
+            params['job_id'] = job_id
+
+        res = self._get(self.host + data_endpoint, params=params)
         logging.info(res['msg'])
-        return res['sentences_results']
+        sentences = res['sentences_results']
+        if len(sentences) == 0:
+            logging.info(f"No sentences found, returning empty dataframe.")
+            return pd.DataFrame()
+
+        cols = list(sentences[0].keys())
+        rows = [[s[col] for col in cols] for s in sentences]
+        df = pd.DataFrame(rows, columns=cols)
+        if "stance_dict" in cols and sentences[0]["stance_dict"]:
+            df = df.apply(lambda r: update_row_with_stance_data(r), axis=1)
+        return df
+
+    @staticmethod
+    def init_logger():
+        '''
+        Inits the logger for more informative console prints.
+        '''
+        from logging import getLogger, getLevelName, Formatter, StreamHandler
+        log = getLogger()
+        log.setLevel(getLevelName('INFO'))
+        log_formatter = Formatter("%(asctime)s [%(levelname)s] %(filename)s %(lineno)d: %(message)s")
+
+        console_handler = StreamHandler()
+        console_handler.setFormatter(log_formatter)
+        log.handlers = []
+        log.addHandler(console_handler)
+
+    @staticmethod
+    def print_report(user_report, job_statuses: Optional[List[str]] = None, active_domains_only: Optional[bool] = True,
+                     domains_to_show: Optional[List[str]] = None):
+        '''
+        Prints the user_report to console.
+        :param user_report: the user report, returned by method get_full_report
+        :param job_statuses: optional, print only jobs with the listed statuses. possible statuses:
+        'PENDING','PROCESSING','CANCELED','ERROR','DONE'
+        :param active_domains_only: optional, print only jobs from domains that were not deleted. default: true.
+        :param domains_to_show: optional, print only these domain and jobs from these domains (if they exist).
+        '''
+        logging.info('User Report:')
+        comments_statuses = user_report['domains_status']
+        logging.info('  Comments status by domain (%d domains):' % len(comments_statuses))
+        active_domains = []
+        if len(comments_statuses) == 0:
+            logging.info('    User has no domains')
+        else:
+            for status in comments_statuses:
+                domain = status["domain"]
+                if domains_to_show and domain not in domains_to_show:
+                    continue
+                active_domains.append(domain)
+                logging.info(
+                    f'    Domain: {domain}, Domain Params: {status["domain_params"]}, Status: {status["data_status"]}')
+        kp_summarization_statuses = user_report['kp_analysis_status']
+        logging.info(f'  Key point summarization - jobs status:')
+        if len(kp_summarization_statuses) == 0:
+            logging.info('    User has no key point summarization jobs history')
+        else:
+            n_total_jobs = len(kp_summarization_statuses)
+            if active_domains_only:
+                kp_summarization_statuses = list(filter(lambda x: x["domain"] in active_domains, kp_summarization_statuses))
+            if job_statuses and len(job_statuses) > 0:
+                kp_summarization_statuses = list(filter(lambda x: x["status"] in job_statuses, kp_summarization_statuses))
+            if domains_to_show and len(domains_to_show) > 0:
+                kp_summarization_statuses = list(filter(lambda x: x["domain"] in domains_to_show, kp_summarization_statuses))
+            n_displayed_jobs = len(kp_summarization_statuses)
+            logging.info(
+                f'  Displaying {n_displayed_jobs} jobs out of {n_total_jobs}: {"only active" if active_domains_only else "all"} domains, '
+                f'{"all" if not job_statuses else job_statuses} jobs statuses, {"all" if not domains_to_show else domains_to_show} domain names')
+
+            for kp_summarization_status in kp_summarization_statuses:
+                logging.info(f'    Job: {str(kp_summarization_status)}')
+
+    def get_results_from_job_id(self, job_id:str):
+        kps_future = KpsJobFuture(self, job_id)
+        kps_result = kps_future.get_result(high_verbosity=True)
+        return kps_result
+
+    @staticmethod
+    def _validate_params_dict(params_dict, params_type:str):
+        if params_dict is None:
+            return
+        if not isinstance(params_dict, dict):
+            raise KpsIllegalInputException(f'{params_type}_params must be a dictionary, given: {type(params_dict)}')
+
+        for k,v in params_dict.items():
+            if not isinstance(k, str):
+                raise KpsIllegalInputException(f'{params_type}_params keys must be a strings, given: {type(k)}:{k}')
+            if type(v) not in [list, str, int, float, bool]:
+                raise KpsIllegalInputException(f'unsupported {params_type}_params value type: {type(v)}:{v}')
+
+    @staticmethod
+    def _validate_request(params):
+        for param_name,val in params.items():
+            if param_name in ["domain","job_id","description"]:
+                assert isinstance(val, str), f"{param_name} should be a string, given {type(val)} : {val}"
+            try:
+                json.dumps(val)
+            except TypeError as e:
+                raise TypeError(f"Request could not be sent to server due to invalid parameters: {param_name}:{val}:\n{e}")
+
 
 
-class KpAnalysisTaskFuture:
+class KpsJobFuture:
     '''
-    A future for an async key point analysis job. Wraps the job_id and uses a provided client for retrieving the job's result.
-    Usually created when starting a key point analysis job but can also be created by a user, by suppling the client and the job_id.
+    A future for an async key point summarization job. Wraps the job_id and uses a provided client for retrieving the job's result.
+    Usually created when starting a key point summarization job but can also be created by a user, by suppling the client and the job_id.
     The job_id can be retrieved from the console (it is printed to console when a job is started) or from the user-report.
     '''
-    def __init__(self, client: KpAnalysisClient, job_id: str):
+    def __init__(self, client: KpsClient, job_id: str):
         '''
-        Create a KpAnalysisTaskFuture over a job_id for results retrieval.
+        Create a KpsJobFuture over a job_id for results retrieval.
         :param client: a client for communicating with the service.
         :param job_id: the job_id. The job_id can be retrieved from the console (it is printed to console when a job is started) or from the user-report.
         '''
         self.client = client
         self.job_id = job_id
-        self.polling_timout_secs = 60
+        self.polling_timeout_secs = 30
 
     def get_job_id(self) -> str:
         '''
         :return: the job_id
         '''
         return self.job_id
 
     def get_result(self, top_k_kps: Optional[int] = None, top_k_sentences_per_kp: Optional[int] = None,
-                   dont_wait: bool = False, wait_secs: Optional[int] = None, polling_timout_secs: Optional[int] = None,
-                   high_verbosity: bool = True):
+                   dont_wait: bool = False, wait_secs: Optional[int] = None, polling_timeout_secs: Optional[int] = None,
+                   high_verbosity: bool = True) -> KpsResult:
         '''
         Retreives the job's result. This method polls and waits till the job is done and the result is available.
-        The result-json consists:
-            * 'keypoint_matchings': a list of keypoint_matching (key point and its matched sentences). Sorted descendingly according to number of matched sentences. each keypoint_matching have:
-                * 'keypoint': the key point string.
-                * 'matching': a list of matched sentences. each match have the sentences details ('domain', 'comment_id', 'sentence_id', 'sents_in_comment', 'span_start', 'span_end', 'num_tokens', 'argument_quality', 'sentence_text') and a match score ('score') this is the match score between the sentence and the key point. The matchings are sorted descendingly according to their match score.
         :param top_k_kps: use this parameter to truncate the result json to have only the top K key points.
         :param top_k_sentences_per_kp: use this parameter to truncate the result json to have only the top K matched sentences per key point.
         :param dont_wait: when True, tries to get the result once and returns it if it's available, otherwise returns None.
         :param wait_secs: limit the waiting time (in seconds).
-        :param polling_timout_secs: sets the time to wait before polling again (in seconds). The default is 60 seconds.
+        :param polling_timeout_secs: sets the time to wait before polling again (in seconds). The default is 30 seconds.
         :param high_verbosity: set to False to reduce the number of messages printed to the logger.
-        :return: the key point analysis job result or throws an exception if an error occurs.
+        :return: the KpsResult object or throws an exception if an error occurs or if the job was canceled.
         '''
         start_time = time.time()
 
         do_again = True
         while do_again:
-            result = self.client.get_kp_extraction_job_status(self.job_id, top_k_kps=top_k_kps, top_k_sentences_per_kp=top_k_sentences_per_kp)
+            result = self.client.get_kps_job_status(self.job_id, top_k_kps=top_k_kps, top_k_sentences_per_kp=top_k_sentences_per_kp)
             if result['status'] == 'PENDING':
                 if high_verbosity:
                     logging.info('job_id %s is pending' % self.job_id)
             elif result['status'] == 'PROCESSING':
                 if high_verbosity:
                     progress = result['progress']
                     logging.info('job_id %s is running, progress: %s' % (self.job_id, progress))
                     self._print_progress_bar(progress)
             elif result['status'] == 'DONE':
                 logging.info('job_id %s is done, returning result' % self.job_id)
-                return result['result']
+                json_results = result['result']
+                return KpsResult.create_from_result_json(json_results)
             elif result['status'] == 'ERROR':
                 error_msg = 'job_id %s has error, error_msg: %s' % (self.job_id, str(result['error_msg']))
                 logging.error(error_msg)
                 raise Exception(error_msg)
             elif result['status'] == 'CANCELED':
                 logging.info('job_id %s was canceled!' % self.job_id)
                 raise Exception('waiting for result on a job that was canceled')
             else:
                 raise Exception('unsupported status: %s, result: %s' % (result['status'], str(result)))
 
             do_again = False if dont_wait else True if wait_secs is None else time.time() - start_time < wait_secs
-            time.sleep(polling_timout_secs if polling_timout_secs is not None else self.polling_timout_secs)
+            time.sleep(polling_timeout_secs if polling_timeout_secs is not None else self.polling_timeout_secs)
         return None
 
     def cancel(self):
         '''
         Cancels (stops) the running job. Please stop unneeded jobs since they use a lot of resources.
         '''
-        self.client.cancel_kp_extraction_job(self.job_id)
+        self.client.cancel_kps_job(self.job_id)
 
     def _print_progress_bar(self, progress):
         if 'total_stages' in progress:
             total_stages = progress['total_stages']
             for i in reversed(range(total_stages)):
                 stage = str(i + 1)
                 stage_i = 'stage_' + stage
                 if stage_i in progress and 'inferred_batches' in progress[stage_i] and 'total_batches' in progress[stage_i]:
                     print_progress_bar(progress[stage_i]['inferred_batches'], progress[stage_i]['total_batches'], prefix='Stage %s/%s:' % (stage, str(total_stages)), suffix='Complete', length=50)
-                    break
+                    break
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/keypoints_pairs_infer_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/keypoints_pairs_infer_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/narrative_generation_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/narrative_generation_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/pro_con_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/pro_con_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/response_data/speech_response.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/response_data/speech_response.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/term_relater_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/term_relater_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/term_wikifier_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/term_wikifier_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/clients/theme_extraction_client.py` & `debater_python_api-5.0.0/debater_python_api/api/clients/theme_extraction_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/debater_api.py` & `debater_python_api-5.0.0/debater_python_api/api/debater_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,13 +62,13 @@
     def get_index_searcher_client(self):
         return index_searcher_client.IndexServiceClient(self.get_apikey())
 
     def get_narrative_generation_client(self):
         return narrative_generation_client.NarrativeGenerationClient(self.get_apikey())
 
     def get_keypoints_client(self):
-        return keypoints_client.KpAnalysisClient(self.get_apikey(), 'https://keypoint-matching-backend.debater.res.ibm.com')
+        return keypoints_client.KpsClient(self.get_apikey(), 'https://keypoint-matching-backend.debater.res.ibm.com')
 
     def get_keypoints_pairs_infer_client(self):
         return keypoints_pairs_infer_client.KpPairsInferClient(self.get_apikey(), 'https://keypoint-matching.debater.res.ibm.com')
```

### Comparing `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_client.py` & `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_client.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py` & `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py` & `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/elastic_search_sentence_res.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_base.py` & `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_base.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/api/sentence_level_index/client/sentence_query_request.py` & `debater_python_api-5.0.0/debater_python_api/api/sentence_level_index/client/sentence_query_request.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/argument_quality_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/argument_quality_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/claim_boundaries_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/claim_boundaries_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/claim_detection_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/claim_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/clustering_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/clustering_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/embedding_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/embedding_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/evidence_detection_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/evidence_detection_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/example_of_sc_args.py` & `debater_python_api-5.0.0/debater_python_api/examples/example_of_sc_args.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/index_searcher_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/index_searcher_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/keypoints_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/keypoints_example.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from debater_python_api.api.clients.key_point_analysis.KpAnalysisUtils import KpAnalysisUtils
+from debater_python_api.api.clients.keypoints_client import KpsClient
 from debater_python_api.api.debater_api import DebaterApi
 
 debater_api = DebaterApi('PUT_YOUR_API_KEY_HERE')
 keypoints_client = debater_api.get_keypoints_client()
 
 comments_texts = [
     'Cannabis has detrimental effects on cognition and memory, some of which are irreversible.',
@@ -13,10 +13,10 @@
     'Frequent marijuana use can seriously affect short-term memory.',
     'Marijuana is very addictive, and therefore very dangerous'
     'Cannabis is addictive and very dangerous for use.',
     'Cannabis can be very harmful and addictive, especially for young people',
     'Cannabis is very addictive.'
                   ]
 
-KpAnalysisUtils.init_logger()
-keypoint_matchings = keypoints_client.run(comments_texts)
-KpAnalysisUtils.print_result(keypoint_matchings, n_sentences_per_kp=10, title="KPA Example")
+KpsClient.init_logger()
+keypoint_matchings_result = keypoints_client.run_full_kps_flow(domain="keypoints_example_domain", comments_texts=comments_texts)
+keypoint_matchings_result.print_result(n_sentences_per_kp=10, title="KPS Example")
```

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/pro_con_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/pro_con_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/resources/arguments.py` & `debater_python_api-5.0.0/debater_python_api/examples/resources/arguments.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/resources/pro_con_scores.py` & `debater_python_api-5.0.0/debater_python_api/examples/resources/pro_con_scores.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/run_all_services.py` & `debater_python_api-5.0.0/debater_python_api/examples/run_all_services.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/speech_construction_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/speech_construction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/term_wikifier_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/term_wikifier_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/theme_extraction_example.py` & `debater_python_api-5.0.0/debater_python_api/examples/theme_extraction_example.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/usecases/kp_based_survey.py` & `debater_python_api-5.0.0/debater_python_api/examples/usecases/kp_based_survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/usecases/mining_to_narrative.py` & `debater_python_api-5.0.0/debater_python_api/examples/usecases/mining_to_narrative.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/examples/usecases/survey.py` & `debater_python_api-5.0.0/debater_python_api/examples/usecases/survey.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py` & `debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesIT.py` & `debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesIT.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # (C) Copyright IBM Corp. 2020.
 import math
 import sys
 import unittest
 
 from hamcrest import assert_that
 
-from debater_python_api.api.clients.key_point_analysis.KpAnalysisUtils import KpAnalysisUtils
+from debater_python_api.api.clients.keypoints_client import KpsClient
 from debater_python_api.api.clients.narrative_generation_client import Polarity
 from debater_python_api.api.sentence_level_index.client.sentence_query_base import SimpleQuery
 from debater_python_api.api.sentence_level_index.client.sentence_query_request import SentenceQueryRequest
 from debater_python_api.examples.resources.arguments import arguments_list
 from debater_python_api.examples.resources.pro_con_scores import pro_con_scores
 from debater_python_api.integration_tests.api.clients.DebaterApiWithAdjustedUrl import DebaterApiWithAdjustedUrl
 from debater_python_api.integration_tests.api.clients.DebaterApiWithAdjustedUrl import Domains
@@ -189,32 +189,35 @@
                 if annotation['concept']['title'] is not None:
                     titles.append(annotation['concept']['title'])
 
         assert_that(len(titles) > 0)
 
     def test_keypoints_service (self):
         comments_texts = [
-            "Using cannabis can lead to more dangerous drug use",
-            "Prolonged use of cannabis increases the risk of developing psychosis.",
-            "Cannabis is a gateway drug to more dangerous drugs",
-            "The use of cannabis can be addictive for some people",
-            "Legalizing illicit drugs will kill the black market",
-            "When cannabis is consumed over a long period of time it has impact on memory and decision making of people.",
-            "Early studies suggested cognitive declines associated with marijuana ; these declines persisted long after the period of acute cannabis intoxication."
+                'Cannabis has detrimental effects on cognition and memory, some of which are irreversible.',
+                'Cannabis can severely impact memory and productivity in its consumers.',
+                'Cannabis harms the memory and learning capabilities of its consumers.',
+                'Frequent use can impair cognitive ability.',
+                'Cannabis harms memory, which in the long term hurts progress and can hurt people',
+                'Frequent marijuana use can seriously affect short-term memory.',
+                'Marijuana is very addictive, and therefore very dangerous'
+                'Cannabis is addictive and very dangerous for use.',
+                'Cannabis can be very harmful and addictive, especially for young people',
+                'Cannabis is very addictive.'
         ]
-        KpAnalysisUtils.init_logger()
+        KpsClient.init_logger()
         keypoints_client = self.debater_api.get_keypoints_client()
-
-        keypoint_matchings = keypoints_client.run(comments_texts)
-        KpAnalysisUtils.print_result(keypoint_matchings)
-        assert_that(len(keypoint_matchings['keypoint_matchings']) > 1)
-        for keypoint_matching in keypoint_matchings['keypoint_matchings']:
+        keypoint_matchings_res = keypoints_client.run_full_kps_flow("serviceit_test" ,comments_texts)
+        keypoint_matchings_res.print_result(n_sentences_per_kp=10, title="KPS Result")
+        keypoint_matchings = keypoint_matchings_res.result_json['keypoint_matchings']
+        assert_that(len(keypoint_matchings) > 1)
+        for keypoint_matching in keypoint_matchings:
             if keypoint_matching['keypoint'] != 'none':
                 for matching in keypoint_matching['matching']:
-                    assert_that(0.98 <= matching['score'] <= 1.0)
+                    assert_that(0.95 <= matching['score'] <= 1.0)
 
 
     def test_theme_extraction_service(self):
 
         theme_extraction_client = self.debater_api.get_theme_extraction_client()
 
         dominant_concept = 'Animal'
```

### Comparing `debater_python_api-4.3.2/debater_python_api/integration_tests/api/clients/ServicesLoad.py` & `debater_python_api-5.0.0/debater_python_api/integration_tests/api/clients/ServicesLoad.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/utils/clusters_refiner.py` & `debater_python_api-5.0.0/debater_python_api/utils/clusters_refiner.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/utils/general_utils.py` & `debater_python_api-5.0.0/debater_python_api/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api/utils/kp_analysis_conf.py` & `debater_python_api-5.0.0/debater_python_api/utils/kp_analysis_conf.py`

 * *Files identical despite different names*

### Comparing `debater_python_api-4.3.2/debater_python_api.egg-info/PKG-INFO` & `debater_python_api-5.0.0/debater_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debater-python-api
-Version: 4.3.2
+Version: 5.0.0
 Summary: Project Debater Early Access Program API sdk for python
 Author-email: Elad Venezian <eladv@il.ibm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `debater_python_api-4.3.2/debater_python_api.egg-info/SOURCES.txt` & `debater_python_api-5.0.0/debater_python_api.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 debater_python_api/api/clients/keypoints_client.py
 debater_python_api/api/clients/keypoints_pairs_infer_client.py
 debater_python_api/api/clients/narrative_generation_client.py
 debater_python_api/api/clients/pro_con_client.py
 debater_python_api/api/clients/term_relater_client.py
 debater_python_api/api/clients/term_wikifier_client.py
 debater_python_api/api/clients/theme_extraction_client.py
-debater_python_api/api/clients/key_point_analysis/KpAnalysisUtils.py
-debater_python_api/api/clients/key_point_analysis/KpaExceptions.py
-debater_python_api/api/clients/key_point_analysis/KpaResult.py
-debater_python_api/api/clients/key_point_analysis/docx_generator.py
-debater_python_api/api/clients/key_point_analysis/try_things.py
-debater_python_api/api/clients/key_point_analysis/utils.py
+debater_python_api/api/clients/key_point_summarization/KpsExceptions.py
+debater_python_api/api/clients/key_point_summarization/KpsResult.py
+debater_python_api/api/clients/key_point_summarization/docx_generator.py
+debater_python_api/api/clients/key_point_summarization/graph_generator.py
+debater_python_api/api/clients/key_point_summarization/utils.py
 debater_python_api/api/clients/response_data/__init__.py
 debater_python_api/api/clients/response_data/speech_response.py
 debater_python_api/api/sentence_level_index/__init__.py
 debater_python_api/api/sentence_level_index/client/__init__.py
 debater_python_api/api/sentence_level_index/client/article_retrieval_request.py
 debater_python_api/api/sentence_level_index/client/elastic_client.py
 debater_python_api/api/sentence_level_index/client/elastic_search_article_res.py
@@ -69,9 +68,8 @@
 debater_python_api/integration_tests/api/clients/DebaterApiWithAdjustedUrl.py
 debater_python_api/integration_tests/api/clients/ServicesIT.py
 debater_python_api/integration_tests/api/clients/ServicesLoad.py
 debater_python_api/integration_tests/api/clients/__init__.py
 debater_python_api/utils/__init__.py
 debater_python_api/utils/clusters_refiner.py
 debater_python_api/utils/general_utils.py
-debater_python_api/utils/kp_analysis_conf.py
-debater_python_api/utils/kp_analysis_utils.py
+debater_python_api/utils/kp_analysis_conf.py
```

### Comparing `debater_python_api-4.3.2/pyproject.toml` & `debater_python_api-5.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debater_python_api"
-version = "4.3.2"
+version = "5.0.0"
 description = "Project Debater Early Access Program API sdk for python"
 readme = "README.md"
 authors = [{ name = "Elad Venezian", email = "eladv@il.ibm.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

