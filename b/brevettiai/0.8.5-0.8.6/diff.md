# Comparing `tmp/brevettiai-0.8.5.tar.gz` & `tmp/brevettiai-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brevettiai-0.8.5.tar", max compression
+gzip compressed data, was "brevettiai-0.8.6.tar", max compression
```

## Comparing `brevettiai-0.8.5.tar` & `brevettiai-0.8.6.tar`

### file list

```diff
@@ -1,136 +1,138 @@
--rw-r--r--   0        0        0    11358 2023-03-24 10:35:44.741143 brevettiai-0.8.5/LICENSE
--rw-r--r--   0        0        0      678 2023-03-24 10:35:44.741143 brevettiai-0.8.5/README.md
--rw-r--r--   0        0        0      306 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/__init__.py
--rw-r--r--   0        0        0      156 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/__init__.py
--rw-r--r--   0        0        0    21427 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/data_generator.py
--rw-r--r--   0        0        0      374 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/__init__.py
--rw-r--r--   0        0        0       86 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/annotation.py
--rw-r--r--   0        0        0     4805 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/annotation_loader.py
--rw-r--r--   0        0        0    10337 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/annotation_parser.py
--rw-r--r--   0        0        0     1683 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/annotation_pooling.py
--rw-r--r--   0        0        0      872 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/bayer_demosaic.py
--rw-r--r--   0        0        0    14400 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/bcimg_dataset.py
--rw-r--r--   0        0        0    26860 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/image_augmenter.py
--rw-r--r--   0        0        0    11743 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/image_loader.py
--rw-r--r--   0        0        0    10337 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/image_pipeline.py
--rw-r--r--   0        0        0      877 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/image_processor.py
--rw-r--r--   0        0        0     1271 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/image_region.py
--rw-r--r--   0        0        0      223 2023-03-24 10:35:44.741143 brevettiai-0.8.5/brevettiai/data/image/modules.py
--rw-r--r--   0        0        0     4612 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/image/multi_frame_imager.py
--rw-r--r--   0        0        0     4254 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/image/segmentation_loader.py
--rw-r--r--   0        0        0     3733 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/image/sequence_loader.py
--rw-r--r--   0        0        0    15180 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/image/utils.py
--rw-r--r--   0        0        0     1481 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/inspection_info.py
--rw-r--r--   0        0        0    10164 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/sample_integrity.py
--rw-r--r--   0        0        0     9711 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/sample_tools.py
--rw-r--r--   0        0        0     4617 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/tf_types.py
--rw-r--r--   0        0        0     6422 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/data/tf_utils.py
--rw-r--r--   0        0        0      374 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/__init__.py
--rw-r--r--   0        0        0      348 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/camelmodel.py
--rw-r--r--   0        0        0      987 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/color.py
--rw-r--r--   0        0        0     3243 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/dataset.py
--rw-r--r--   0        0        0     4448 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/image.py
--rw-r--r--   0        0        0     5656 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/image_annotation.py
--rw-r--r--   0        0        0     1140 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/tag.py
--rw-r--r--   0        0        0     7570 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/datamodel/web_api_types.py
--rw-r--r--   0        0        0     3819 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/examples/explore_application.py
--rw-r--r--   0        0        0      465 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/examples/plot_annotation.py
--rw-r--r--   0        0        0     1439 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/examples/run_experiment.py
--rw-r--r--   0        0        0       71 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/__init__.py
--rw-r--r--   0        0        0     3101 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/aws.py
--rw-r--r--   0        0        0     4862 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/facets_atlas.py
--rw-r--r--   0        0        0     2357 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/git_state.py
--rw-r--r--   0        0        0     2558 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/package_validation.py
--rw-r--r--   0        0        0     3559 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/pivot.py
--rw-r--r--   0        0        0     2268 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/raygun.py
--rw-r--r--   0        0        0     2311 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/remote_monitor.py
--rw-r--r--   0        0        0     1783 2023-03-24 10:35:44.745143 brevettiai-0.8.5/brevettiai/interfaces/sagemaker.py
--rw-r--r--   0        0        0    21985 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/interfaces/vue_schema_utils.py
--rw-r--r--   0        0        0      451 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/__init__.py
--rw-r--r--   0        0        0    15551 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/cloudpath.py
--rw-r--r--   0        0        0     1344 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/credentials.py
--rw-r--r--   0        0        0     4160 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/file_cache.py
--rw-r--r--   0        0        0     2071 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/files.py
--rw-r--r--   0        0        0      743 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/h5_metadata.py
--rw-r--r--   0        0        0     4677 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/local_io.py
--rw-r--r--   0        0        0     8813 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/minio_io.py
--rw-r--r--   0        0        0     4923 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/onnx.py
--rw-r--r--   0        0        0     2325 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/path.py
--rw-r--r--   0        0        0     1184 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/serialization.py
--rw-r--r--   0        0        0     2790 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/smart_open_patch.py
--rw-r--r--   0        0        0     3577 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/tf_recorder.py
--rw-r--r--   0        0        0     1365 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/url_io.py
--rw-r--r--   0        0        0     6825 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/io/utils.py
--rw-r--r--   0        0        0        0 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/ml/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/ml/tensorflow/__init__.py
--rw-r--r--   0        0        0     5839 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/ml/tensorflow/annotation_loader.py
--rw-r--r--   0        0        0      111 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/__init__.py
--rw-r--r--   0        0        0     2692 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/catalogue.py
--rw-r--r--   0        0        0      534 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/factory/__init__.py
--rw-r--r--   0        0        0     2191 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/factory/lenet_backbone.py
--rw-r--r--   0        0        0     8746 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/factory/lraspp.py
--rw-r--r--   0        0        0     3690 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/factory/mobilenetv2_backbone.py
--rw-r--r--   0        0        0     2652 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/factory/segmentation.py
--rw-r--r--   0        0        0     2510 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/factory/unet.py
--rw-r--r--   0        0        0     2972 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/losses.py
--rw-r--r--   0        0        0      137 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/metadata/__init__.py
--rw-r--r--   0        0        0     1465 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/metadata/history.py
--rw-r--r--   0        0        0     2805 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/metadata/image_segmentation.py
--rw-r--r--   0        0        0      538 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/metadata/inference.py
--rw-r--r--   0        0        0     2903 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/model/metadata/metadata.py
--rw-r--r--   0        0        0      332 2023-03-24 10:35:44.749143 brevettiai-0.8.5/brevettiai/platform/__init__.py
--rw-r--r--   0        0        0     8568 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/aipackage.py
--rw-r--r--   0        0        0     2758 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/annotations.py
--rw-r--r--   0        0        0     1274 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/dataset.py
--rw-r--r--   0        0        0     8145 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/model_archive.py
--rw-r--r--   0        0        0      368 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/models/__init__.py
--rw-r--r--   0        0        0    21202 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/models/annotation.py
--rw-r--r--   0        0        0    12476 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/models/dataset.py
--rw-r--r--   0        0        0      370 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/models/iomodel.py
--rw-r--r--   0        0        0    21112 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/models/job.py
--rw-r--r--   0        0        0     4851 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/models/platform_backend.py
--rw-r--r--   0        0        0     3720 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/platform_credentials.py
--rw-r--r--   0        0        0    28968 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/platform/web_api.py
--rw-r--r--   0        0        0   150582 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/bin/0_1543413266626.bmp
--rw-r--r--   0        0        0     6796 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/bin/1651574629796.json
--rw-r--r--   0        0        0      249 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/get_resources.py
--rw-r--r--   0        0        0     1767 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/test_aipackage.py
--rw-r--r--   0        0        0     5045 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/test_annotation_loader.py
--rw-r--r--   0        0        0     5858 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/test_annotation_tooling.py
--rw-r--r--   0        0        0    14997 2023-03-24 10:35:44.753143 brevettiai-0.8.5/brevettiai/tests/test_data.py
--rw-r--r--   0        0        0     5048 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_data_image.py
--rw-r--r--   0        0        0      882 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_data_manipulation.py
--rw-r--r--   0        0        0     3923 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_image_loader.py
--rw-r--r--   0        0        0     1329 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_model_archive.py
--rw-r--r--   0        0        0      577 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_model_catalogue.py
--rw-r--r--   0        0        0     1139 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_model_loss.py
--rw-r--r--   0        0        0     3500 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_model_metadata.py
--rw-r--r--   0        0        0     1574 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_pivot.py
--rw-r--r--   0        0        0     1249 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_platform_annotation.py
--rw-r--r--   0        0        0     1263 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_platform_job.py
--rw-r--r--   0        0        0     3732 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_polygon_extraction.py
--rw-r--r--   0        0        0     1795 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_schema.py
--rw-r--r--   0        0        0     1200 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_tags.py
--rw-r--r--   0        0        0      667 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tests/test_web_api.py
--rw-r--r--   0        0        0        0 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tooling/__init__.py
--rw-r--r--   0        0        0     5288 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tooling/annotation_tools.py
--rw-r--r--   0        0        0     7134 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tooling/experiments.py
--rw-r--r--   0        0        0     1633 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/tooling/plot.py
--rw-r--r--   0        0        0       67 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/__init__.py
--rw-r--r--   0        0        0     1117 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/argparse_utils.py
--rw-r--r--   0        0        0      614 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/dict_utils.py
--rw-r--r--   0        0        0      536 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/env_variables.py
--rw-r--r--   0        0        0     2651 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/model_version.py
--rw-r--r--   0        0        0     2589 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/module.py
--rw-r--r--   0        0        0      292 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/numpy_json_encoder.py
--rw-r--r--   0        0        0     5823 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/onnx_benchmark.py
--rw-r--r--   0        0        0     1491 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/pandas_utils.py
--rw-r--r--   0        0        0      850 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/polygon_utils.py
--rw-r--r--   0        0        0     1707 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/profiling.py
--rw-r--r--   0        0        0      433 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/singleton.py
--rw-r--r--   0        0        0     5961 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/tensorboard_collector.py
--rw-r--r--   0        0        0     3914 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/tf_serving_request.py
--rw-r--r--   0        0        0     4171 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/upload_data.py
--rw-r--r--   0        0        0      843 2023-03-24 10:35:44.757143 brevettiai-0.8.5/brevettiai/utils/validate_args.py
--rw-r--r--   0        0        0     2383 2023-03-24 10:35:44.761143 brevettiai-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 brevettiai-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-05 11:23:09.518812 brevettiai-0.8.6/LICENSE
+-rw-r--r--   0        0        0      678 2023-06-05 11:23:09.518812 brevettiai-0.8.6/README.md
+-rw-r--r--   0        0        0      306 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/__init__.py
+-rw-r--r--   0        0        0      156 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/__init__.py
+-rw-r--r--   0        0        0    21427 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/data_generator.py
+-rw-r--r--   0        0        0      374 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/__init__.py
+-rw-r--r--   0        0        0       86 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation.py
+-rw-r--r--   0        0        0     4805 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation_loader.py
+-rw-r--r--   0        0        0    10337 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation_parser.py
+-rw-r--r--   0        0        0     1683 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/annotation_pooling.py
+-rw-r--r--   0        0        0      872 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/bayer_demosaic.py
+-rw-r--r--   0        0        0    14429 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/bcimg_dataset.py
+-rw-r--r--   0        0        0    26860 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_augmenter.py
+-rw-r--r--   0        0        0    11743 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_loader.py
+-rw-r--r--   0        0        0    10337 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_pipeline.py
+-rw-r--r--   0        0        0      877 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_processor.py
+-rw-r--r--   0        0        0     1271 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/image_region.py
+-rw-r--r--   0        0        0      223 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/modules.py
+-rw-r--r--   0        0        0     4612 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/multi_frame_imager.py
+-rw-r--r--   0        0        0     4254 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/segmentation_loader.py
+-rw-r--r--   0        0        0     3733 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/sequence_loader.py
+-rw-r--r--   0        0        0    15180 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/image/utils.py
+-rw-r--r--   0        0        0     1481 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/inspection_info.py
+-rw-r--r--   0        0        0    10164 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/sample_integrity.py
+-rw-r--r--   0        0        0     9711 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/sample_tools.py
+-rw-r--r--   0        0        0     1075 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/serialization.py
+-rw-r--r--   0        0        0     1292 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/tf_serialization.py
+-rw-r--r--   0        0        0     4617 2023-06-05 11:23:09.518812 brevettiai-0.8.6/brevettiai/data/tf_types.py
+-rw-r--r--   0        0        0     6422 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/data/tf_utils.py
+-rw-r--r--   0        0        0      374 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/camelmodel.py
+-rw-r--r--   0        0        0      987 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/color.py
+-rw-r--r--   0        0        0     3243 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/dataset.py
+-rw-r--r--   0        0        0     4672 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/image.py
+-rw-r--r--   0        0        0     5656 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/image_annotation.py
+-rw-r--r--   0        0        0     1140 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/tag.py
+-rw-r--r--   0        0        0     7570 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/datamodel/web_api_types.py
+-rw-r--r--   0        0        0     3819 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/examples/explore_application.py
+-rw-r--r--   0        0        0      465 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/examples/plot_annotation.py
+-rw-r--r--   0        0        0     1439 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/examples/run_experiment.py
+-rw-r--r--   0        0        0       71 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/__init__.py
+-rw-r--r--   0        0        0     3101 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/aws.py
+-rw-r--r--   0        0        0     4862 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/facets_atlas.py
+-rw-r--r--   0        0        0     2357 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/git_state.py
+-rw-r--r--   0        0        0     2558 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/package_validation.py
+-rw-r--r--   0        0        0     3559 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/pivot.py
+-rw-r--r--   0        0        0     2268 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/raygun.py
+-rw-r--r--   0        0        0     2311 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/remote_monitor.py
+-rw-r--r--   0        0        0     1783 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/sagemaker.py
+-rw-r--r--   0        0        0    21985 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/interfaces/vue_schema_utils.py
+-rw-r--r--   0        0        0      451 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/__init__.py
+-rw-r--r--   0        0        0    15551 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/cloudpath.py
+-rw-r--r--   0        0        0     1344 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/credentials.py
+-rw-r--r--   0        0        0     4160 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/file_cache.py
+-rw-r--r--   0        0        0     2071 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/files.py
+-rw-r--r--   0        0        0      743 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/h5_metadata.py
+-rw-r--r--   0        0        0     4677 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/local_io.py
+-rw-r--r--   0        0        0     8813 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/minio_io.py
+-rw-r--r--   0        0        0     4923 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/onnx.py
+-rw-r--r--   0        0        0     2325 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/path.py
+-rw-r--r--   0        0        0     1184 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/serialization.py
+-rw-r--r--   0        0        0     2790 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/smart_open_patch.py
+-rw-r--r--   0        0        0     3577 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/tf_recorder.py
+-rw-r--r--   0        0        0     1365 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/url_io.py
+-rw-r--r--   0        0        0     6825 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/io/utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/ml/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/ml/tensorflow/__init__.py
+-rw-r--r--   0        0        0     5839 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/ml/tensorflow/annotation_loader.py
+-rw-r--r--   0        0        0      111 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/model/__init__.py
+-rw-r--r--   0        0        0     2692 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/model/catalogue.py
+-rw-r--r--   0        0        0      534 2023-06-05 11:23:09.522812 brevettiai-0.8.6/brevettiai/model/factory/__init__.py
+-rw-r--r--   0        0        0     2191 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/lenet_backbone.py
+-rw-r--r--   0        0        0     8746 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/lraspp.py
+-rw-r--r--   0        0        0     3690 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/mobilenetv2_backbone.py
+-rw-r--r--   0        0        0     2652 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/segmentation.py
+-rw-r--r--   0        0        0     2510 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/factory/unet.py
+-rw-r--r--   0        0        0     2972 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/losses.py
+-rw-r--r--   0        0        0      137 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/__init__.py
+-rw-r--r--   0        0        0     1465 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/history.py
+-rw-r--r--   0        0        0     2805 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/image_segmentation.py
+-rw-r--r--   0        0        0      538 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/inference.py
+-rw-r--r--   0        0        0     2903 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/model/metadata/metadata.py
+-rw-r--r--   0        0        0      346 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/__init__.py
+-rw-r--r--   0        0        0     8568 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/aipackage.py
+-rw-r--r--   0        0        0     2758 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/annotations.py
+-rw-r--r--   0        0        0     1274 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/dataset.py
+-rw-r--r--   0        0        0     8145 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/model_archive.py
+-rw-r--r--   0        0        0      368 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/__init__.py
+-rw-r--r--   0        0        0    21202 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/annotation.py
+-rw-r--r--   0        0        0    12476 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/dataset.py
+-rw-r--r--   0        0        0      370 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/iomodel.py
+-rw-r--r--   0        0        0    21112 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/job.py
+-rw-r--r--   0        0        0     5142 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/models/platform_backend.py
+-rw-r--r--   0        0        0     3720 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/platform_credentials.py
+-rw-r--r--   0        0        0    29359 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/platform/web_api.py
+-rw-r--r--   0        0        0   150582 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/bin/0_1543413266626.bmp
+-rw-r--r--   0        0        0     6796 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/bin/1651574629796.json
+-rw-r--r--   0        0        0      249 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/get_resources.py
+-rw-r--r--   0        0        0     1767 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/test_aipackage.py
+-rw-r--r--   0        0        0     5045 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/test_annotation_loader.py
+-rw-r--r--   0        0        0     5858 2023-06-05 11:23:09.526812 brevettiai-0.8.6/brevettiai/tests/test_annotation_tooling.py
+-rw-r--r--   0        0        0    15003 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_data.py
+-rw-r--r--   0        0        0     5048 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_data_image.py
+-rw-r--r--   0        0        0      882 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_data_manipulation.py
+-rw-r--r--   0        0        0     3923 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_image_loader.py
+-rw-r--r--   0        0        0     1329 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_archive.py
+-rw-r--r--   0        0        0      577 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_catalogue.py
+-rw-r--r--   0        0        0     1139 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_loss.py
+-rw-r--r--   0        0        0     3500 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_model_metadata.py
+-rw-r--r--   0        0        0     1574 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_pivot.py
+-rw-r--r--   0        0        0     1249 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_platform_annotation.py
+-rw-r--r--   0        0        0     1263 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_platform_job.py
+-rw-r--r--   0        0        0     3732 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_polygon_extraction.py
+-rw-r--r--   0        0        0     1795 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_schema.py
+-rw-r--r--   0        0        0     1200 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_tags.py
+-rw-r--r--   0        0        0      667 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tests/test_web_api.py
+-rw-r--r--   0        0        0        0 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/__init__.py
+-rw-r--r--   0        0        0     5288 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/annotation_tools.py
+-rw-r--r--   0        0        0     7247 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/experiments.py
+-rw-r--r--   0        0        0     1633 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/tooling/plot.py
+-rw-r--r--   0        0        0       67 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/__init__.py
+-rw-r--r--   0        0        0     1117 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/argparse_utils.py
+-rw-r--r--   0        0        0      614 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/dict_utils.py
+-rw-r--r--   0        0        0      536 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/env_variables.py
+-rw-r--r--   0        0        0     2651 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/model_version.py
+-rw-r--r--   0        0        0     2589 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/module.py
+-rw-r--r--   0        0        0      292 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/numpy_json_encoder.py
+-rw-r--r--   0        0        0     5823 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/onnx_benchmark.py
+-rw-r--r--   0        0        0     1491 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/pandas_utils.py
+-rw-r--r--   0        0        0      850 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/polygon_utils.py
+-rw-r--r--   0        0        0     1707 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/profiling.py
+-rw-r--r--   0        0        0      433 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/singleton.py
+-rw-r--r--   0        0        0     5961 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/tensorboard_collector.py
+-rw-r--r--   0        0        0     3914 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/tf_serving_request.py
+-rw-r--r--   0        0        0     4171 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/upload_data.py
+-rw-r--r--   0        0        0      843 2023-06-05 11:23:09.530812 brevettiai-0.8.6/brevettiai/utils/validate_args.py
+-rw-r--r--   0        0        0     2372 2023-06-05 11:23:09.534812 brevettiai-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     2903 1970-01-01 00:00:00.000000 brevettiai-0.8.6/PKG-INFO
```

### Comparing `brevettiai-0.8.5/LICENSE` & `brevettiai-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/README.md` & `brevettiai-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/data_generator.py` & `brevettiai-0.8.6/brevettiai/data/data_generator.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/annotation_loader.py` & `brevettiai-0.8.6/brevettiai/data/image/annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/annotation_parser.py` & `brevettiai-0.8.6/brevettiai/data/image/annotation_parser.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/annotation_pooling.py` & `brevettiai-0.8.6/brevettiai/data/image/annotation_pooling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/bayer_demosaic.py` & `brevettiai-0.8.6/brevettiai/data/image/bayer_demosaic.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/bcimg_dataset.py` & `brevettiai-0.8.6/brevettiai/data/image/bcimg_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,17 +209,17 @@
         samples = samples.reset_index(drop=False)
 
         # Explode annotations to dataframe with path as id
         index, data = zip(
             *((k, dict(
                 a.dict(include={"type", "label", "uuid", "visibility", "severity"}),
                 geometry=a.geometry,
-                bbox=BBOX(*a.geometry.bounds),
+                bbox=BBOX(*map(int, a.geometry.bounds)),
             ))
-              for k, ia in annotations.items() if len(ia.annotations) for a in ia.annotations))
+              for k, ia in annotations.items() if len(ia.annotations) for a in ia.annotations if type(a) != dict))
         ann = pd.DataFrame(data=data, index=index)
         out = pd.merge(samples, ann, left_on=samples.annotation_path.apply(str), right_index=True, how="inner")
         out["visibility"].fillna(-1, inplace=True)
         out["severity"].fillna(-1, inplace=True)
         out.set_index(out.columns[0], drop=True, inplace=True)
         return out
```

### Comparing `brevettiai-0.8.5/brevettiai/data/image/image_augmenter.py` & `brevettiai-0.8.6/brevettiai/data/image/image_augmenter.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/image_loader.py` & `brevettiai-0.8.6/brevettiai/data/image/image_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/image_pipeline.py` & `brevettiai-0.8.6/brevettiai/data/image/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/image_processor.py` & `brevettiai-0.8.6/brevettiai/data/image/image_processor.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/image_region.py` & `brevettiai-0.8.6/brevettiai/data/image/image_region.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/multi_frame_imager.py` & `brevettiai-0.8.6/brevettiai/data/image/multi_frame_imager.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/segmentation_loader.py` & `brevettiai-0.8.6/brevettiai/data/image/segmentation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/sequence_loader.py` & `brevettiai-0.8.6/brevettiai/data/image/sequence_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/image/utils.py` & `brevettiai-0.8.6/brevettiai/data/image/utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/inspection_info.py` & `brevettiai-0.8.6/brevettiai/data/inspection_info.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/sample_integrity.py` & `brevettiai-0.8.6/brevettiai/data/sample_integrity.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/sample_tools.py` & `brevettiai-0.8.6/brevettiai/data/sample_tools.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/tf_types.py` & `brevettiai-0.8.6/brevettiai/data/tf_types.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/data/tf_utils.py` & `brevettiai-0.8.6/brevettiai/data/tf_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/datamodel/color.py` & `brevettiai-0.8.6/brevettiai/datamodel/color.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/datamodel/dataset.py` & `brevettiai-0.8.6/brevettiai/datamodel/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/datamodel/image.py` & `brevettiai-0.8.6/brevettiai/datamodel/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 @dataclass(frozen=True, eq=True)
 class ImageRegion:
     y: int
     x: int
     height: int
     width: int
 
+    @classmethod
+    def from_bbox(cls, obj):
+        shape = obj.shape
+        return cls(
+            y=int(obj.y1),
+            x=int(obj.x1),
+            height=int(shape[0]),
+            width=int(shape[1]),
+        )
+
 
 @dataclass(frozen=True, eq=True, order=True)
 class SequenceShape:
     frames: int = 0
     height: int = 0
     width: int = 0
     channels: int = 0
```

### Comparing `brevettiai-0.8.5/brevettiai/datamodel/image_annotation.py` & `brevettiai-0.8.6/brevettiai/datamodel/image_annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/datamodel/tag.py` & `brevettiai-0.8.6/brevettiai/datamodel/tag.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/datamodel/web_api_types.py` & `brevettiai-0.8.6/brevettiai/datamodel/web_api_types.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/examples/explore_application.py` & `brevettiai-0.8.6/brevettiai/examples/explore_application.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/examples/run_experiment.py` & `brevettiai-0.8.6/brevettiai/examples/run_experiment.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/aws.py` & `brevettiai-0.8.6/brevettiai/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/facets_atlas.py` & `brevettiai-0.8.6/brevettiai/interfaces/facets_atlas.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/git_state.py` & `brevettiai-0.8.6/brevettiai/interfaces/git_state.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/package_validation.py` & `brevettiai-0.8.6/brevettiai/interfaces/package_validation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/pivot.py` & `brevettiai-0.8.6/brevettiai/interfaces/pivot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/raygun.py` & `brevettiai-0.8.6/brevettiai/interfaces/raygun.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/remote_monitor.py` & `brevettiai-0.8.6/brevettiai/interfaces/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/sagemaker.py` & `brevettiai-0.8.6/brevettiai/interfaces/sagemaker.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/interfaces/vue_schema_utils.py` & `brevettiai-0.8.6/brevettiai/interfaces/vue_schema_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/cloudpath.py` & `brevettiai-0.8.6/brevettiai/io/cloudpath.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/credentials.py` & `brevettiai-0.8.6/brevettiai/io/credentials.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/file_cache.py` & `brevettiai-0.8.6/brevettiai/io/file_cache.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/files.py` & `brevettiai-0.8.6/brevettiai/io/files.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/h5_metadata.py` & `brevettiai-0.8.6/brevettiai/io/h5_metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/local_io.py` & `brevettiai-0.8.6/brevettiai/io/local_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/minio_io.py` & `brevettiai-0.8.6/brevettiai/io/minio_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/onnx.py` & `brevettiai-0.8.6/brevettiai/io/onnx.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/path.py` & `brevettiai-0.8.6/brevettiai/io/path.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/serialization.py` & `brevettiai-0.8.6/brevettiai/io/serialization.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/smart_open_patch.py` & `brevettiai-0.8.6/brevettiai/io/smart_open_patch.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/tf_recorder.py` & `brevettiai-0.8.6/brevettiai/io/tf_recorder.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/url_io.py` & `brevettiai-0.8.6/brevettiai/io/url_io.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/io/utils.py` & `brevettiai-0.8.6/brevettiai/io/utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/ml/tensorflow/annotation_loader.py` & `brevettiai-0.8.6/brevettiai/ml/tensorflow/annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/catalogue.py` & `brevettiai-0.8.6/brevettiai/model/catalogue.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/factory/__init__.py` & `brevettiai-0.8.6/brevettiai/model/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/factory/lenet_backbone.py` & `brevettiai-0.8.6/brevettiai/model/factory/lenet_backbone.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/factory/lraspp.py` & `brevettiai-0.8.6/brevettiai/model/factory/lraspp.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/factory/mobilenetv2_backbone.py` & `brevettiai-0.8.6/brevettiai/model/factory/mobilenetv2_backbone.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/factory/segmentation.py` & `brevettiai-0.8.6/brevettiai/model/factory/segmentation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/factory/unet.py` & `brevettiai-0.8.6/brevettiai/model/factory/unet.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/losses.py` & `brevettiai-0.8.6/brevettiai/model/losses.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/metadata/history.py` & `brevettiai-0.8.6/brevettiai/model/metadata/history.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/metadata/image_segmentation.py` & `brevettiai-0.8.6/brevettiai/model/metadata/image_segmentation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/metadata/inference.py` & `brevettiai-0.8.6/brevettiai/model/metadata/inference.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/model/metadata/metadata.py` & `brevettiai-0.8.6/brevettiai/model/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/aipackage.py` & `brevettiai-0.8.6/brevettiai/platform/aipackage.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/annotations.py` & `brevettiai-0.8.6/brevettiai/platform/annotations.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/dataset.py` & `brevettiai-0.8.6/brevettiai/platform/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/model_archive.py` & `brevettiai-0.8.6/brevettiai/platform/model_archive.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/models/annotation.py` & `brevettiai-0.8.6/brevettiai/platform/models/annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/models/dataset.py` & `brevettiai-0.8.6/brevettiai/platform/models/dataset.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/models/job.py` & `brevettiai-0.8.6/brevettiai/platform/models/job.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/models/platform_backend.py` & `brevettiai-0.8.6/brevettiai/platform/models/platform_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,40 +53,42 @@
         r = requests.get(f"{self.host}/api/resources/roottags?key={api_key}&id={id}")
         if r.ok:
             return [Tag.parse_obj(x) for x in r.json()]
         else:
             log.warning("Could not get root tags")
             return []
 
-    def get_annotation_url(self, s3_image_path, annotation_name=None,
+    def get_annotation_url(self, s3_image_path=None, image_path=None, dataset_id=None, annotation_name=None,
                            bbox=None, zoom=None, screen_size=1024, test_report_id=None, model_id=None,
                            min_zoom=2, max_zoom=300):
         """
         Get url to annotation file
         :param s3_image_path: Name of image file
         :param annotation_name: Name of annotation file, if any
         :param bbox: Selects zoom and center for the bbox
         :param zoom: Zoom level [2-300] related to screen pixel size (if None zoom will be calculated from bbox)
         :param screen_size: default screen size in pixels
         :param test_report_id:
         :param model_id:
         :param min_zoom:
         :param max_zoom:
         """
-        s3_image_path = str(s3_image_path)
-        uri_length = 36
-        rm_keys = [self.data_bucket, ".tiles/", "/dzi.json"]
-        image_key = s3_image_path
-        for rm_key in rm_keys:
-            image_key = image_key.replace(rm_key, "")
-        image_key = image_key.lstrip("/")
-        dataset_id = image_key[:uri_length]
-        image_rel_path = "/".join(image_key.split("/")[1:])
+        if s3_image_path is not None:
+            s3_image_path = str(s3_image_path)
+            uri_length = 36
+            rm_keys = [self.data_bucket, ".tiles/", "/dzi.json"]
+            image_key = s3_image_path
+            for rm_key in rm_keys:
+                image_key = image_key.replace(rm_key, "")
+            image_key = image_key.lstrip("/")
+            dataset_id = image_key[:uri_length]
+            image_path = "/".join(image_key.split("/")[1:])
 
-        url_info = dict(file=image_rel_path)
+
+        url_info = dict(file=image_path)
 
         if annotation_name:
             url_info["annotationFile"] = annotation_name
 
         if test_report_id:
             url_info["testReportId"] = test_report_id
 
@@ -113,7 +115,13 @@
     def custom_report_type(self):
         from brevettiai.datamodel.web_api_types import ReportType
         return ReportType(id=self.custom_report_id, name="custom report", created="",status=1,
                           can_run_on_projects=False, can_run_on_applications=False, can_run_on_models=True,
                           max_runtime_in_seconds=1, instance_count=1, volume_size_in_gb=100, model_type_ids=[])
 
 backend = PlatformBackend()
+
+test_backend = PlatformBackend(
+    host="https://platformdev.brevetti.ai",
+    data_bucket="s3://platformdev.brevetti.ai",
+    custom_job_id="136610ed-65d2-4f78-bd11-cb8b5a1e3953",
+)
```

### Comparing `brevettiai-0.8.5/brevettiai/platform/platform_credentials.py` & `brevettiai-0.8.6/brevettiai/platform/platform_credentials.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/platform/web_api.py` & `brevettiai-0.8.6/brevettiai/platform/web_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,25 @@
         r = self.session.get(url, headers=headers, **kwargs)
         if not r.ok:
             if r.status_code == 401:
                 raise PermissionError("Not authorized")
             raise requests.HTTPError(r.reason)
         return r
 
+    def _http_put(self, url, headers=None, **kwargs):
+        if url.startswith(self.host):
+            headers = {**(headers or {}), **self.antiforgery_headers}
+
+        r = self.session.put(url, headers=headers, **kwargs)
+        if not r.ok:
+            if r.status_code == 401:
+                raise PermissionError("Not authorized")
+            raise requests.HTTPError(r.reason)
+        return r
+
     def _http_post(self, url, headers=None, **kwargs):
         if url.startswith(self.host):
             headers = {**(headers or {}), **self.antiforgery_headers}
 
         r = self.session.post(url, headers=headers, **kwargs)
         if not r.ok:
             if r.status_code == 401:
@@ -422,15 +433,15 @@
         self.update_annotation(dataset, image_path, annotation_name=new_annotation_name, annotation=annotation)
         self.delete_annotation(dataset, image_path, annotation_name=annotation_name)
 
     def create(self, obj: Union[Dataset, Tag, api.Model, api.Report], **kwargs):
         if isinstance(obj, Dataset):
             payload = obj.dict(include={"name", "reference", "notes", "locked"}, by_alias=True)
             payload["tagIds"] = [tag.id for tag in obj.tags]
-            r = self._http_post(f"{self.host}/api/data/", json=payload)
+            r = self._http_post(f"{self.host}/api/data/", )
             return self.get_dataset(r.json()["datasetId"], **kwargs)
         elif isinstance(obj, Tag):
             payload = obj.dict(include={"name", "parent_id"}, by_alias=True, exclude_none=True)
             self._http_post(f"{self.host}/api/resources/tags/", json=payload)
 
             # TODO: return tag id on api
             parent = self.get_tag(obj.parent_id)
```

### Comparing `brevettiai-0.8.5/brevettiai/tests/bin/0_1543413266626.bmp` & `brevettiai-0.8.6/brevettiai/tests/bin/0_1543413266626.bmp`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/bin/1651574629796.json` & `brevettiai-0.8.6/brevettiai/tests/bin/1651574629796.json`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_aipackage.py` & `brevettiai-0.8.6/brevettiai/tests/test_aipackage.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_annotation_loader.py` & `brevettiai-0.8.6/brevettiai/tests/test_annotation_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_annotation_tooling.py` & `brevettiai-0.8.6/brevettiai/tests/test_annotation_tooling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_data.py` & `brevettiai-0.8.6/brevettiai/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class TestDataGenerator(unittest.TestCase):
     n = 10
     samples = pd.DataFrame({
         "category": pd.Series(np.random.RandomState(20).randint(0, 3, size=n)).apply(lambda x: (x,)).astype("category"),
         "id": pd.Series(np.arange(n))
     })
-    samples.category.cat.categories = [("A",), ("B",), ("A", "B")]
+    samples.category.cat.rename_categories([("A",), ("B",), ("A", "B")])
     samples["path"] = samples.id.map(str)
 
     def test_unshuffled_unbatched(self):
         ds = DataGenerator(self.samples)
 
         df = pd.DataFrame(ds.get_samples_numpy(batch=False))
         self.assertTrue((self.samples.id.values == df.id).all())
```

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_data_image.py` & `brevettiai-0.8.6/brevettiai/tests/test_data_image.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_data_manipulation.py` & `brevettiai-0.8.6/brevettiai/tests/test_data_manipulation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_image_loader.py` & `brevettiai-0.8.6/brevettiai/tests/test_image_loader.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_model_archive.py` & `brevettiai-0.8.6/brevettiai/tests/test_model_archive.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_model_catalogue.py` & `brevettiai-0.8.6/brevettiai/tests/test_model_catalogue.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_model_loss.py` & `brevettiai-0.8.6/brevettiai/tests/test_model_loss.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_model_metadata.py` & `brevettiai-0.8.6/brevettiai/tests/test_model_metadata.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_pivot.py` & `brevettiai-0.8.6/brevettiai/tests/test_pivot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_platform_annotation.py` & `brevettiai-0.8.6/brevettiai/tests/test_platform_annotation.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_platform_job.py` & `brevettiai-0.8.6/brevettiai/tests/test_platform_job.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_polygon_extraction.py` & `brevettiai-0.8.6/brevettiai/tests/test_polygon_extraction.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_schema.py` & `brevettiai-0.8.6/brevettiai/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_tags.py` & `brevettiai-0.8.6/brevettiai/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tests/test_web_api.py` & `brevettiai-0.8.6/brevettiai/tests/test_web_api.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tooling/annotation_tools.py` & `brevettiai-0.8.6/brevettiai/tooling/annotation_tools.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/tooling/experiments.py` & `brevettiai-0.8.6/brevettiai/tooling/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import Optional, List
+import logging
 
 from brevettiai.platform import PlatformAPI, Job
 from brevettiai.datamodel import web_api_types as api
 
+log = logging.getLogger(__name__)
 
 def generate_model_name(name, job_type, message):
     try:
         from brevettiai.interfaces.git_state import GitRepositoryState
         git_state = GitRepositoryState.from_type(job_type)
         branch = git_state.active_branch
     except (ImportError, TypeError):
@@ -115,14 +117,15 @@
 
     def run(self, errors="raise"):
         try:
             self.job = self.platform.initialize_training(self.model, job_type=self.job_type or Job)
             self.print_info()
             self.job.start()
         except Exception as ex:
+            log.error("Exception during training", exc_info=ex)
             if errors == "raise":
                 raise ex
         return self
 
     def delete(self):
         self.platform.delete(self.model)
```

### Comparing `brevettiai-0.8.5/brevettiai/tooling/plot.py` & `brevettiai-0.8.6/brevettiai/tooling/plot.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/argparse_utils.py` & `brevettiai-0.8.6/brevettiai/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/dict_utils.py` & `brevettiai-0.8.6/brevettiai/utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/env_variables.py` & `brevettiai-0.8.6/brevettiai/utils/env_variables.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/model_version.py` & `brevettiai-0.8.6/brevettiai/utils/model_version.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/module.py` & `brevettiai-0.8.6/brevettiai/utils/module.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/onnx_benchmark.py` & `brevettiai-0.8.6/brevettiai/utils/onnx_benchmark.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/pandas_utils.py` & `brevettiai-0.8.6/brevettiai/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/polygon_utils.py` & `brevettiai-0.8.6/brevettiai/utils/polygon_utils.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/profiling.py` & `brevettiai-0.8.6/brevettiai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/tensorboard_collector.py` & `brevettiai-0.8.6/brevettiai/utils/tensorboard_collector.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/tf_serving_request.py` & `brevettiai-0.8.6/brevettiai/utils/tf_serving_request.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/upload_data.py` & `brevettiai-0.8.6/brevettiai/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/brevettiai/utils/validate_args.py` & `brevettiai-0.8.6/brevettiai/utils/validate_args.py`

 * *Files identical despite different names*

### Comparing `brevettiai-0.8.5/pyproject.toml` & `brevettiai-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brevettiai"
-version = "0.8.5"
+version = "0.8.6"
 readme = "README.md"
 homepage = "https://platform.brevetti.ai"
 documentation = "https://docs.brevetti.ai/"
 repository = "https://bitbucket.org/criterionai/core.git"
 description = "Brevetti AI library"
 license = "Apache-2.0"
 authors = ["Emil Tyge <emil@brevetti.ai>"]
@@ -27,25 +27,26 @@
 tqdm = ">=4.62"
 toml = "^0.10.2"
 pandas = ">=1.5.3"
 parse = "^1.19.0"
 cryptography = ">=36.0.1" # webapi
 shapely = ">=2.0" # Annotations
 smart-open = "^6.3.0"
-cloudpathlib = {extras = ["s3"], version = "^0.13.0"}
+cloudpathlib = "^0.14"
+boto3 = "1.26.146"
 semidbm = "^0.5.1"
 
 mmh3 = ">=3.0"  # only sample integrity
 backoff = ">=1.10" # Only in io.minio
 
 tf2onnx = ">=1.9.0"  # onnx export
 onnxruntime = ">=1.6.0"  # Benchmarking
 onnxruntime-gpu = {version = ">=1.6.0", optional = true} # Benchmarking
 h5py = "^3.6.0" # Metadata
-py7zr = "^0.18.9" # AI package
+py7zr = ">=0.18.9" # AI package
 
 
 tensorflow = {version = ">=2.7, !=2.9.2, <2.11", optional = true, markers="sys_platform != 'darwin'"}
 protobuf = {version = "<3.20",  optional = true}
 tensorflow-macos = {version = "^2.8", optional = true, markers="sys_platform == 'darwin'"}
 tensorflow-metal = { version = "^0.5", optional = true, markers="sys_platform == 'darwin'"}
 tensorflow_addons = {version = ">=0.16.1,<0.19", optional = true}
```

### Comparing `brevettiai-0.8.5/PKG-INFO` & `brevettiai-0.8.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: brevettiai
-Version: 0.8.5
+Version: 0.8.6
 Summary: Brevetti AI library
 Home-page: https://platform.brevetti.ai
 License: Apache-2.0
 Author: Emil Tyge
 Author-email: emil@brevetti.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: cv2
 Provides-Extra: cv2-headless
 Provides-Extra: export-gpu
 Provides-Extra: tf
 Provides-Extra: tfa
 Requires-Dist: backoff (>=1.10)
-Requires-Dist: cloudpathlib[s3] (>=0.13.0,<0.14.0)
+Requires-Dist: boto3 (==1.26.146)
+Requires-Dist: cloudpathlib (>=0.14,<0.15)
 Requires-Dist: cryptography (>=36.0.1)
 Requires-Dist: h5py (>=3.6.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=4.1)
 Requires-Dist: minio (>=7.0,<7.1)
 Requires-Dist: mmh3 (>=3.0)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: onnxruntime (>=1.6.0)
 Requires-Dist: onnxruntime-gpu (>=1.6.0) ; extra == "export-gpu"
 Requires-Dist: opencv-python (>=4.1) ; extra == "cv2"
 Requires-Dist: opencv-python-headless (>=4.1) ; extra == "cv2-headless"
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: parse (>=1.19.0,<2.0.0)
 Requires-Dist: protobuf (<3.20) ; extra == "tf"
-Requires-Dist: py7zr (>=0.18.9,<0.19.0)
+Requires-Dist: py7zr (>=0.18.9)
 Requires-Dist: pydantic (>=1.9.0,!=1.9.1)
 Requires-Dist: requests (>=2.23)
 Requires-Dist: semidbm (>=0.5.1,<0.6.0)
 Requires-Dist: shapely (>=2.0)
 Requires-Dist: smart-open (>=6.3.0,<7.0.0)
 Requires-Dist: tensorflow (>=2.7,!=2.9.2,<2.11) ; (sys_platform != "darwin") and (extra == "tf")
 Requires-Dist: tensorflow-io-gcs-filesystem (>=0.31.0) ; extra == "tf"
```

