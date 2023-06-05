# Comparing `tmp/aqtp-0.1.0.tar.gz` & `tmp/aqtp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtp-0.1.0.tar", last modified: Sat May 27 01:21:40 2023, max compression
+gzip compressed data, was "aqtp-0.1.1.tar", last modified: Mon Jun  5 20:44:14 2023, max compression
```

## Comparing `aqtp-0.1.0.tar` & `aqtp-0.1.1.tar`

### file list

```diff
@@ -1,188 +1,187 @@
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.976766 aqtp-0.1.0/
--rw-r--r--   0 lew      (84645) primarygroup (89939)    11358 2023-05-27 00:40:35.000000 aqtp-0.1.0/LICENSE
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1753 2023-05-27 01:21:40.976766 aqtp-0.1.0/PKG-INFO
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1133 2023-05-27 01:21:13.000000 aqtp-0.1.0/README.md
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.956766 aqtp-0.1.0/aqt/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/__init__.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.960766 aqtp-0.1.0/aqt/common/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      576 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     4354 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_common.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    14652 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_config.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    13928 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_config_schedule_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5177 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/aqt_config_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    15655 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/emulated_floating_points.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5730 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/common/emulation_utils.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.960766 aqtp-0.1.0/aqt/jax/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      576 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    13641 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_conv_general.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    12151 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_conv_general_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     8861 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_dot_general.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    14977 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_dot_general_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3783 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_matmul.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3293 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_matmul_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1083 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_ops.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    17734 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_tensor.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     4766 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_tensor_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2705 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax/aqt_utils.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.960766 aqtp-0.1.0/aqt/jax_legacy/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/__init__.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.964766 aqtp-0.1.0/aqt/jax_legacy/jax/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    17225 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    24127 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils_test.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.964766 aqtp-0.1.0/aqt/jax_legacy/jax/flax/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5671 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax/struct.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    35186 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    25400 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    42938 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    75454 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6897 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     7689 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     9842 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    11477 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3477 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2570 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils_test.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.964766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1963 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/check_config_util.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     7382 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/base_config.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      853 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1230 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1439 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1231 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      855 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      855 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      925 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1439 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1440 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1390 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1514 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1383 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1025 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      925 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1232 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6856 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     9732 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2423 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2130 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/hparams_config.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     8129 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/input_pipeline.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     7345 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     9773 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    15474 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3119 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5749 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    19735 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2611 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_benchmark.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2547 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     7921 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5854 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/primitives.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6508 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/primitives_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3927 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/quant_config.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    63692 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/quantization.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    45534 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/quantization_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1654 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/shape_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    22858 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/sparsity.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    23122 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/sparsity_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     9798 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6060 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     9777 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    10461 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/stats_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     4644 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/test_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5436 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/train_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6301 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/train_utils_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      995 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/utils.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     7056 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    15134 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/decode.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    12107 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    11082 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    13257 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.968766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6573 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.972766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1069 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1069 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1056 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1041 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1006 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1193 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      954 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1000 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1101 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1002 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      954 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1000 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1042 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1002 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      954 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1060 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1175 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1244 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.972766 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1096 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1099 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1014 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1096 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1099 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1018 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)      995 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1925 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    23300 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    33379 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    38051 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     4055 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/predict.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    51615 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5666 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    10503 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3939 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    25395 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3284 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.972766 aqtp-0.1.0/aqt/jax_legacy/utils/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      577 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     4810 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/analysis_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     5109 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/analysis_utils_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1045 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/common.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     8505 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    11978 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6807 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/hparams_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    10180 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    10192 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    20428 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/report_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    23689 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/report_utils_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     2538 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3451 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6640 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     4307 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils_test.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.976766 aqtp-0.1.0/aqt/tensorflow/
--rw-r--r--   0 lew      (84645) primarygroup (89939)      576 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/__init__.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    11332 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_conv2d.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6495 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_conv2d_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     6945 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_einsum.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    19276 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_einsum_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    24040 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_matmul.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    14193 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_matmul_test.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     3423 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_ops.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)    25108 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_tensor.py
--rw-r--r--   0 lew      (84645) primarygroup (89939)     8386 2023-05-27 00:40:35.000000 aqtp-0.1.0/aqt/tensorflow/aqt_tensor_test.py
-drwxr-xr-x   0 lew      (84645) primarygroup (89939)        0 2023-05-27 01:21:40.976766 aqtp-0.1.0/aqtp.egg-info/
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1753 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/PKG-INFO
--rw-r--r--   0 lew      (84645) primarygroup (89939)     8230 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/SOURCES.txt
--rw-r--r--   0 lew      (84645) primarygroup (89939)        1 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/dependency_links.txt
--rw-r--r--   0 lew      (84645) primarygroup (89939)        1 2023-05-27 01:04:56.000000 aqtp-0.1.0/aqtp.egg-info/not-zip-safe
--rw-r--r--   0 lew      (84645) primarygroup (89939)      132 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/requires.txt
--rw-r--r--   0 lew      (84645) primarygroup (89939)        4 2023-05-27 01:21:40.000000 aqtp-0.1.0/aqtp.egg-info/top_level.txt
--rw-r--r--   0 lew      (84645) primarygroup (89939)       38 2023-05-27 01:21:40.976766 aqtp-0.1.0/setup.cfg
--rw-r--r--   0 lew      (84645) primarygroup (89939)     1852 2023-05-27 01:21:34.000000 aqtp-0.1.0/setup.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    11358 2022-02-18 08:03:56.000000 aqtp-0.1.1/LICENSE
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    16137 2023-06-05 20:44:14.000000 aqtp-0.1.1/PKG-INFO
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    15517 2023-05-31 17:42:41.000000 aqtp-0.1.1/README.md
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/aqtp.egg-info/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    16137 2023-06-05 20:44:13.000000 aqtp-0.1.1/aqtp.egg-info/PKG-INFO
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     7613 2023-06-05 20:44:13.000000 aqtp-0.1.1/aqtp.egg-info/SOURCES.txt
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)        1 2023-06-05 20:44:13.000000 aqtp-0.1.1/aqtp.egg-info/dependency_links.txt
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)        1 2023-06-05 20:40:35.000000 aqtp-0.1.1/aqtp.egg-info/not-zip-safe
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      132 2023-06-05 20:44:13.000000 aqtp-0.1.1/aqtp.egg-info/requires.txt
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)       33 2023-06-05 20:44:13.000000 aqtp-0.1.1/aqtp.egg-info/top_level.txt
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/common/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      576 2023-02-07 18:57:52.000000 aqtp-0.1.1/common/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4354 2022-10-27 23:05:33.000000 aqtp-0.1.1/common/aqt_common.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    15305 2023-05-31 13:50:42.000000 aqtp-0.1.1/common/aqt_config.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    13928 2022-05-26 04:10:23.000000 aqtp-0.1.1/common/aqt_config_schedule_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     5177 2022-08-25 23:37:36.000000 aqtp-0.1.1/common/aqt_config_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    15983 2022-12-10 06:26:48.000000 aqtp-0.1.1/common/emulated_floating_points.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6018 2023-05-26 00:07:56.000000 aqtp-0.1.1/common/emulation_utils.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      576 2022-05-11 20:07:02.000000 aqtp-0.1.1/jax/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    13641 2023-02-21 23:38:06.000000 aqtp-0.1.1/jax/aqt_conv_general.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    12151 2022-10-31 20:31:33.000000 aqtp-0.1.1/jax/aqt_conv_general_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     8861 2022-10-31 20:31:33.000000 aqtp-0.1.1/jax/aqt_dot_general.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    14977 2023-02-21 23:38:06.000000 aqtp-0.1.1/jax/aqt_dot_general_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3783 2023-02-13 23:15:47.000000 aqtp-0.1.1/jax/aqt_matmul.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3293 2022-08-23 20:23:12.000000 aqtp-0.1.1/jax/aqt_matmul_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1083 2022-08-23 18:06:45.000000 aqtp-0.1.1/jax/aqt_ops.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    17734 2023-02-21 23:38:06.000000 aqtp-0.1.1/jax/aqt_tensor.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4766 2022-08-31 20:37:11.000000 aqtp-0.1.1/jax/aqt_tensor_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2705 2022-10-31 20:31:33.000000 aqtp-0.1.1/jax/aqt_utils.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/__init__.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-22 17:57:36.000000 aqtp-0.1.1/jax_legacy/jax/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    17245 2022-08-05 18:08:32.000000 aqtp-0.1.1/jax_legacy/jax/compute_cost_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    24127 2022-07-22 00:54:03.000000 aqtp-0.1.1/jax_legacy/jax/compute_cost_utils_test.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/flax/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-22 17:57:36.000000 aqtp-0.1.1/jax_legacy/jax/flax/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     5671 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/flax/struct.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    35186 2023-04-26 21:53:26.000000 aqtp-0.1.1/jax_legacy/jax/flax_attention.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    25400 2022-08-24 06:42:19.000000 aqtp-0.1.1/jax_legacy/jax/flax_attention_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    43734 2023-03-16 21:02:19.000000 aqtp-0.1.1/jax_legacy/jax/flax_layers.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    76138 2023-04-07 04:40:56.000000 aqtp-0.1.1/jax_legacy/jax/flax_layers_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6897 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/fp_cast.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     7689 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/fp_cast_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     9842 2022-11-09 04:18:56.000000 aqtp-0.1.1/jax_legacy/jax/get_bounds.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    11477 2022-11-09 04:18:56.000000 aqtp-0.1.1/jax_legacy/jax/get_bounds_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4605 2023-02-13 22:32:17.000000 aqtp-0.1.1/jax_legacy/jax/hlo_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2570 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/hlo_utils_test.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1963 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/check_config_util.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     7382 2022-10-01 19:27:43.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/base_config.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      853 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1230 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1439 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1231 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      855 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      855 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      925 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1439 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1440 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1390 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1514 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1383 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1025 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      925 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w8.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1232 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6856 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/config_schema.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10457 2022-10-01 19:27:43.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2423 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/configs_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2130 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/hparams_config.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     8129 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/input_pipeline.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     7345 2022-04-26 23:44:34.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/models.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     9773 2022-04-13 00:10:06.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/models_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    15474 2022-06-08 22:32:55.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/pokebnn.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3119 2022-03-30 23:32:52.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/pokebnn_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     5749 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/resnet_cost_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    21509 2022-08-06 18:21:10.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/train.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2611 2022-08-25 01:54:04.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/train_benchmark.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2547 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/train_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     7921 2022-08-06 18:21:10.000000 aqtp-0.1.1/jax_legacy/jax/imagenet/train_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     5854 2023-03-14 20:50:11.000000 aqtp-0.1.1/jax_legacy/jax/primitives.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6508 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/primitives_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3927 2022-09-02 05:18:11.000000 aqtp-0.1.1/jax_legacy/jax/quant_config.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    64889 2023-02-21 23:38:06.000000 aqtp-0.1.1/jax_legacy/jax/quantization.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    45534 2023-05-24 23:38:18.000000 aqtp-0.1.1/jax_legacy/jax/quantization_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1654 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/shape_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    22858 2023-04-25 04:25:43.000000 aqtp-0.1.1/jax_legacy/jax/sparsity.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    23122 2023-04-07 04:40:50.000000 aqtp-0.1.1/jax_legacy/jax/sparsity_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     9798 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/stats.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6060 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/stats_tag.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     9777 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/stats_tag_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10461 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/stats_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4644 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/test_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     5436 2022-09-02 05:18:11.000000 aqtp-0.1.1/jax_legacy/jax/train_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6301 2022-09-02 05:18:11.000000 aqtp-0.1.1/jax_legacy/jax/train_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      995 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/utils.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     7056 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/bleu.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    15134 2023-03-14 17:30:11.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/decode.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    12107 2023-03-09 06:08:12.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/gen_hlo.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    11172 2022-04-13 16:44:57.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    13676 2022-10-01 19:27:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6573 2022-10-01 19:27:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1069 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1069 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1056 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1041 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1006 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1193 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      954 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1000 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1101 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1002 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      954 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1000 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1042 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1002 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      954 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1060 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1175 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1244 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-25 23:30:43.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1096 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1099 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1014 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1096 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1099 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1018 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      995 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1925 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    23353 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/input_pipeline.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    33379 2022-04-26 23:44:34.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/models.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    38051 2023-04-07 04:40:52.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/models_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4145 2022-08-25 01:57:33.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/predict.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    58347 2023-04-12 04:08:36.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/train.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     5918 2022-12-16 02:22:56.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/train_flags.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10503 2022-07-14 18:46:48.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/train_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3939 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/training_hparams.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    25559 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4386 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/jax_legacy/utils/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      577 2022-03-22 17:57:36.000000 aqtp-0.1.1/jax_legacy/utils/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10590 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/analysis_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6890 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/analysis_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1045 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/common.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     9034 2022-10-01 19:27:43.000000 aqtp-0.1.1/jax_legacy/utils/config_schema_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    12303 2022-10-01 19:27:43.000000 aqtp-0.1.1/jax_legacy/utils/config_schema_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     8729 2022-09-07 23:12:53.000000 aqtp-0.1.1/jax_legacy/utils/hparams_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10236 2023-06-01 21:47:07.000000 aqtp-0.1.1/jax_legacy/utils/pandas_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10192 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/pandas_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    27383 2022-04-08 22:16:41.000000 aqtp-0.1.1/jax_legacy/utils/report_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    23689 2022-04-05 18:19:08.000000 aqtp-0.1.1/jax_legacy/utils/report_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2538 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/summary_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3451 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/summary_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6640 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/tfevent_utils.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     4307 2022-03-21 20:52:19.000000 aqtp-0.1.1/jax_legacy/utils/tfevent_utils_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)       38 2023-06-05 20:44:14.000000 aqtp-0.1.1/setup.cfg
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     1852 2023-06-05 20:42:32.000000 aqtp-0.1.1/setup.py
+drwxrwxr-x   0 lew      (84645) primarygroup (89939)        0 2023-06-05 20:44:13.000000 aqtp-0.1.1/tensorflow/
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)      576 2022-05-11 20:07:02.000000 aqtp-0.1.1/tensorflow/__init__.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    11332 2023-01-27 20:01:39.000000 aqtp-0.1.1/tensorflow/aqt_conv2d.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     6495 2023-01-27 20:01:39.000000 aqtp-0.1.1/tensorflow/aqt_conv2d_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    10824 2023-05-31 13:50:42.000000 aqtp-0.1.1/tensorflow/aqt_einsum.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    19175 2023-05-31 13:50:42.000000 aqtp-0.1.1/tensorflow/aqt_einsum_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    23260 2023-05-31 13:50:42.000000 aqtp-0.1.1/tensorflow/aqt_matmul.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    14193 2022-10-13 23:25:44.000000 aqtp-0.1.1/tensorflow/aqt_matmul_test.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     3423 2023-01-27 20:01:39.000000 aqtp-0.1.1/tensorflow/aqt_ops.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     2337 2023-05-31 13:50:42.000000 aqtp-0.1.1/tensorflow/aqt_ops_util.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)    25108 2023-01-27 20:01:39.000000 aqtp-0.1.1/tensorflow/aqt_tensor.py
+-rw-rw-r--   0 lew      (84645) primarygroup (89939)     8386 2022-08-31 20:37:11.000000 aqtp-0.1.1/tensorflow/aqt_tensor_test.py
```

### Comparing `aqtp-0.1.0/LICENSE` & `aqtp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/__init__.py` & `aqtp-0.1.1/jax_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/common/__init__.py` & `aqtp-0.1.1/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/common/aqt_common.py` & `aqtp-0.1.1/common/aqt_common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/common/aqt_config.py` & `aqtp-0.1.1/common/aqt_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 import enum
 from typing import Any, Dict, List, Optional, Type, Union
 
 from aqt.common.aqt_config_utils import _BaseConfig
 from aqt.common.aqt_config_utils import _validate_intervals
 from aqt.common.aqt_config_utils import ConfigError
 
+# BEGIN GOOGLE-INTERNAL
+# LINT.IfChange
+# END GOOGLE-INTERNAL
 
 
 @dataclasses.dataclass
 class IntQuantConfig(_BaseConfig):
   # pyformat: disable
   """Config for integer quantization in aqt_ops.
 
@@ -368,7 +371,25 @@
     grad: quantization schedule for gradients (optional).
   """
   lhs: AqtScheduleConfig
   rhs: AqtScheduleConfig
   grad: Optional[AqtScheduleConfig] = None
 
 
+@dataclasses.dataclass
+class AqtEinsumConfig(_BaseConfig):
+  """Quantization config for a two-argument einsum.
+
+  Attributes:
+    lhs: quantization schedule for left-hand side argument
+    rhs: quantization schedule for right-hand side argument
+    grad: quantization schedule for gradients (optional).
+  """
+  lhs: AqtScheduleConfig
+  rhs: AqtScheduleConfig
+
+# BEGIN GOOGLE-INTERNAL
+# LINT.ThenChange(
+#   //depot/google3/knowledge/cerebra/catalyst/tensorflow/aqt/aqt_config.proto,
+#   //depot/google3/knowledge/cerebra/catalyst/tensorflow/aqt/aqt_config_utils.py
+# )
+# END GOOGLE-INTERNAL
```

### Comparing `aqtp-0.1.0/aqt/common/aqt_config_schedule_test.py` & `aqtp-0.1.1/common/aqt_config_schedule_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/common/aqt_config_utils.py` & `aqtp-0.1.1/common/aqt_config_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/common/emulated_floating_points.py` & `aqtp-0.1.1/common/emulated_floating_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,25 @@
 # limitations under the License.
 
 """Emulates various fp8 formats in bfloat16 or float32."""
 
 from aqt.common import emulation_utils
 import tensorflow as tf
 
-from tensorflow.compiler.tf2xla.python import xla  # pylint: disable=g-direct-tensorflow-import
+from google3.third_party.tensorflow.compiler.tf2xla.python import xla  # pylint: disable=g-direct-tensorflow-import
 
 FPMetadata = emulation_utils.FPMetadata
 EXPONENT_BIAS = emulation_utils.EXPONENT_BIAS
 get_max_number = emulation_utils.get_max_number
 
+# BEGIN GOOGLE-INTERNAL
+# branched from:
+# platforms/deepsea/ffds/reduced_precision/emulated_floating_points.py
+# LINT.IfChange
+# END GOOGLE-INTERNAL
 
 
 def get_exponent(t):
   """Get exponent of a tensor."""
 
   assert t.dtype in [tf.bfloat16, tf.float32]
 
@@ -475,7 +480,12 @@
   assert fp_metadata.mantissa_bits <= 6 and fp_metadata.mantissa_bits >= 0
   assert t.dtype in [tf.bfloat16, tf.float32]
 
   with tf.name_scope('emulated_e8mn'):
     return xla.reduce_precision(t, fp_metadata.exponent_bits,
                                 fp_metadata.mantissa_bits)
 
+# BEGIN GOOGLE-INTERNAL
+# LINT.ThenChange(
+#   //depot/google3/platforms/deepsea/ffds/reduced_precision/emulated_floating_points.py
+# )
+# END GOOGLE-INTERNAL
```

### Comparing `aqtp-0.1.0/aqt/common/emulation_utils.py` & `aqtp-0.1.1/common/emulation_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Metadata class and utils shared by the TF and JAX implementations."""
 import enum
 
+# BEGIN GOOGLE-INTERNAL
+# Branched from platforms/deepsea/ffds/reduced_precision/emulation_utils.py
+# LINT.IfChange
+# END GOOGLE-INTERNAL
 
 # the bias of exponent in bfloat16/float32.
 EXPONENT_BIAS = 127
 
 # Supported rounding mode.
 ROUND_AWAY_FROM_ZERO = 'round_away_from_zero'
 ROUND_TO_NEAREST_EVEN = 'round_to_nearest_even'
@@ -151,7 +155,12 @@
 def get_max_number(target_format):
   """Returns the maximum possible number (not inf) allowed by the format."""
   fp_metadata = get_metadata(target_format)
   return get_max_number_from_mantissa_and_max_exp(
       fp_metadata.mantissa_bits, fp_metadata.max_exp)
 
 
+# BEGIN GOOGLE-INTERNAL
+# LINT.ThenChange(
+#   //depot/google3/platforms/deepsea/ffds/reduced_precision/emulation_utils.py,
+# )
+# END GOOGLE-INTERNAL
```

### Comparing `aqtp-0.1.0/aqt/jax/__init__.py` & `aqtp-0.1.1/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_conv_general.py` & `aqtp-0.1.1/jax/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_conv_general_test.py` & `aqtp-0.1.1/jax/aqt_conv_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_dot_general.py` & `aqtp-0.1.1/jax/aqt_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_dot_general_test.py` & `aqtp-0.1.1/jax/aqt_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_matmul.py` & `aqtp-0.1.1/jax/aqt_matmul.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_matmul_test.py` & `aqtp-0.1.1/jax/aqt_matmul_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_ops.py` & `aqtp-0.1.1/jax/aqt_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_tensor.py` & `aqtp-0.1.1/jax/aqt_tensor.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_tensor_test.py` & `aqtp-0.1.1/jax/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax/aqt_utils.py` & `aqtp-0.1.1/jax/aqt_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils.py` & `aqtp-0.1.1/jax_legacy/jax/compute_cost_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from jax._src.lax import convolution as lax_convolution
 from jax._src.lax import lax
 from jax.interpreters import ad
 from jax.interpreters import batching
 from jax.interpreters import mlir
 import numpy as onp
 # pylint: disable=g-direct-tensorflow-import
-from tensorflow.compiler.xla.service import hlo_pb2
+from google3.third_party.tensorflow.compiler.xla.service import hlo_pb2
 # pylint: enable=g-direct-tensorflow-import
 
 FLAGS = flags.FLAGS
 
 # in everywhere it is used in AQT once the AQT migration is done.
 flags.DEFINE_bool(
     'metadata_enabled',
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/compute_cost_utils_test.py` & `aqtp-0.1.1/jax_legacy/jax/compute_cost_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/flax/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/flax/struct.py` & `aqtp-0.1.1/jax_legacy/jax/flax/struct.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention.py` & `aqtp-0.1.1/jax_legacy/jax/flax_attention.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/flax_attention_test.py` & `aqtp-0.1.1/jax_legacy/jax/flax_attention_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers.py` & `aqtp-0.1.1/jax_legacy/jax/flax_layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     # QuantOps hyperparameter to quantize inputs. If None, no activation
     # quantization will be applied.
     quant_act: Optional[QuantOps.ActHParams]
     # Quantization strategy, one of `fake_quant` or `aqt`.
     quant_type: QuantType
     weight_quant_granularity: quant_config.QuantGranularity
 
+    # BEGIN GOOGLE-INTERNAL
+    weight_sub_channels: Optional[int] = None
+    # END GOOGLE-INTERNAL
 
     act_sparsity: Optional[SparseHParams] = None
     weight_sparsity: Optional[SparseHParams] = None
 
   hparams: HParams
   paxis_name: Optional[str]
   features: Union[int, Tuple[int, ...]]
@@ -251,14 +254,17 @@
       raise ValueError(
           f'Invalid quantization granularity {weight_quant_granularity}.')
 
     weight_params = QuantOps.WeightParams(
         prec=hparams.weight_prec,
         half_shift=hparams.weight_half_shift,
         axis=weight_quant_axis,
+        # BEGIN GOOGLE-INTERNAL
+        sub_channels=hparams.weight_sub_channels,
+        # END GOOGLE-INTERNAL
         expected_scale_shape=expected_scale_shape)
 
     # TODO(wanglisa): add option to control when scale is being recomputed
 
     bounds_params = None
     if hparams.quant_act is not None:
       if isinstance(hparams.quant_act.bounds, get_bounds.DynamicBounds.Hyper):
@@ -598,14 +604,17 @@
     # half_shift flag for weights
     weight_half_shift: bool
     # QuantOps hyperparameter to quantize inputs. If None, no activation
     # quantization will be applied.
     quant_act: Optional[QuantOps.ActHParams]
     # Quantization strategy, one of `fake_quant` or `aqt`.
     quant_type: QuantType
+    # BEGIN GOOGLE-INTERNAL
+    weight_sub_channels: Optional[int] = None
+    # END GOOGLE-INTERNAL
 
   hparams: HParams
   features: int
   kernel_size: Tuple[int, ...]
   dynamic_context: quant_config.DynamicContext
   train: bool
   paxis_name: Optional[str]
@@ -669,14 +678,17 @@
           'we only support fake_quant style of aqt for ConvAqt.')
       quantized_type = hparams.quant_type.to_jax_type()
       kernel = QuantOps.create_weights_fake_quant(
           kernel,
           weight_params=QuantOps.WeightParams(
               prec=hparams.weight_prec,
               half_shift=hparams.weight_half_shift,
+              # BEGIN GOOGLE-INTERNAL
+              sub_channels=hparams.weight_sub_channels,
+              # END GOOGLE-INTERNAL
               axis=kernel_reduction_axis,
               expected_scale_shape=expected_scale_shape),
           quantized_type=quantized_type,
           quantize_weights=self.dynamic_context.quantize_weights)
 
     # Convolution
     dimension_numbers = flax.linen.linear._conv_dimension_numbers(
@@ -748,14 +760,17 @@
     # half_shift flag for weights
     weight_half_shift: bool
     # QuantOps hyperparameter to quantize inputs for logits. If None, no
     # activation quantization will be applied.
     quant_act: Optional[QuantOps.ActHParams]
     # Quantization strategy, one of `fake_quant` or `aqt`.
     quant_type: QuantType
+    # BEGIN GOOGLE-INTERNAL
+    weight_sub_channels: Optional[int] = None
+    # END GOOGLE-INTERNAL
 
   num_embeddings: int
   features: int
   hparams: HParams
   dtype: Any
   paxis_name: Optional[str]
   train: bool
@@ -778,14 +793,17 @@
         dot_precision=None,
         prefer_int8_to_int32_dot=self.dynamic_context.prefer_int8_to_int32_dot,
         weight_params=QuantOps.WeightParams(
             prec=hparams.weight_prec,
             axis=(0,),
             expected_scale_shape=(1, self.embedding.shape[0]),
             half_shift=hparams.weight_half_shift,
+            # BEGIN GOOGLE-INTERNAL
+            sub_channels=hparams.weight_sub_channels,
+            # END GOOGLE-INTERNAL
             ))
 
   def __call__(
       self,
       inputs: jnp.ndarray,
   ) -> jnp.ndarray:
     """Embeds the inputs along the last dimension.
@@ -829,14 +847,17 @@
       # weight matrix in the logits layer, which is what we need for AQT.
       embedding_quant_ops = QuantOps.create_weights_ops(
           embedding,
           weight_params=QuantOps.WeightParams(
               prec=weight_prec,
               axis=(1,),
               half_shift=weight_half_shift,
+              # BEGIN GOOGLE-INTERNAL
+              sub_channels=hparams.weight_sub_channels,
+              # END GOOGLE-INTERNAL
               ))
       embedding_quant_ops.assert_scale_shape_is(shape=(self.num_embeddings, 1))
 
       quantized_embedding = embedding_quant_ops.to_quantized(
           embedding, dtype=quantized_type)
       quantized_embedded_inputs = quantized_embedding[inputs]
       # Since the embedding matrix 'quantized_embedding' is gathered based on
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/flax_layers_test.py` & `aqtp-0.1.1/jax_legacy/jax/flax_layers_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 from jax import dtypes
 from jax import lax
 from jax import random
 from jax.nn import initializers
 import jax.numpy as jnp
 import numpy as onp
 
+# BEGIN GOOGLE-INTERNAL
+from google3.nlp.nlx.infrastructure.flaxformer import sharding
+# END GOOGLE-INTERNAL
 
 FLAGS = flags.FLAGS
 
 # fp-1-4-3
 #    1: sign
 #    4: number of exponent-bits, (bias = 11), range: -11, ..., 4
 #    3: number of significand-bits (excluding hidden-bit)
@@ -1968,14 +1971,20 @@
         bias_init=initializers.ones,
         kernel_axis_names=('a', 'b', 'c'),
     )
     y, variables = model.init_with_output(rng, x)
     # We transform the last input dimension to two output dimensions (2, 2).
     onp.testing.assert_allclose(y, onp.full((1, 2, 2), 3.))
 
+    # BEGIN GOOGLE-INTERNAL
+    # The output sharding dimensions have been collapsed.
+    sharding.check_params_and_axis_names_match(variables)
+    self.assertEqual(variables['params_axes']['kernel_axes'],
+                     sharding.axis_names('a', 'b * c'))
+    # END GOOGLE-INTERNAL
 
   def test_dense_general_two_axes(self):
     rng = random.PRNGKey(0)
     x = jnp.ones((1, 2, 2))
     model = flax_layers.DenseGeneralAqt(
         hparams=self.hparams,
         train=False,
@@ -1986,11 +1995,17 @@
         bias_init=initializers.ones,
         kernel_axis_names=('a', 'b', 'c'),
     )
     y, variables = model.init_with_output(rng, x)
     # We transform the last two input dimensions (2, 2) to one output dimension.
     onp.testing.assert_allclose(y, onp.full((1, 3), 4.))
 
+    # BEGIN GOOGLE-INTERNAL
+    # The input sharding dimensions have been collapsed.
+    sharding.check_params_and_axis_names_match(variables)
+    self.assertEqual(variables['params_axes']['kernel_axes'],
+                     sharding.axis_names('a * b', 'c'))
+    # END GOOGLE-INTERNAL
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast.py` & `aqtp-0.1.1/jax_legacy/jax/fp_cast.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/fp_cast_test.py` & `aqtp-0.1.1/jax_legacy/jax/fp_cast_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds.py` & `aqtp-0.1.1/jax_legacy/jax/get_bounds.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/get_bounds_test.py` & `aqtp-0.1.1/jax_legacy/jax/get_bounds_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils.py` & `aqtp-0.1.1/jax_legacy/jax/hlo_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 import os.path
 import re
 from typing import Any, Callable, Sequence, Text, Tuple, Union
 from flax import linen as nn
 import jax
 import jax.numpy as jnp
 
+# BEGIN GOOGLE-INTERNAL
+from google3.pyglib import gfile
+# END GOOGLE-INTERNAL
 
 # pylint: disable=g-direct-tensorflow-import
-from tensorflow.compiler.xla.service import hlo_pb2
+from google3.third_party.tensorflow.compiler.xla.service import hlo_pb2
 # pylint: enable=g-direct-tensorflow-import
 
 
 def load_hlo_proto_from_jax_fn(fn: Callable[..., Any], *fn_args: Any,
                                **fn_kwargs: Any) -> hlo_pb2.HloModuleProto:
   """Loads HLO proto object from jax function.
 
@@ -83,14 +86,42 @@
     file_path: file path to write the HLO to.
   """
   hlo_module_proto_str = computation.as_serialized_hlo_module_proto()
   hlo_txt = computation.as_hlo_text()
   output_hlo_to_file(hlo_module_proto_str, hlo_txt, file_path)
 
 
+# BEGIN GOOGLE-INTERNAL
+def output_hlo_to_file(hlo_module_proto_str: Union[bytes, Text],
+                       hlo_txt: Union[str, Text], file_path: str):
+  """Saves HLO proto string and hlo text to given file path.
+
+  The file format is determined by the file_path extension, i.e. for .txt file
+  only saves the hlo_txt, and for .pb file only save the hlo_module_proto_str
+  binary.
+
+  Args:
+    hlo_module_proto_str: hlo module proto serialized as string
+    hlo_txt: hlo text
+    file_path: file path to write the HLO to.
+  """
+  _, ext = os.path.splitext(file_path)
+  if ext == '.pb':
+    # At the moment, we're not saving HloProto because the method that we've
+    # been using before (as_serialized_hlo_module_proto, ParseFromString and
+    # then create a HloProto) takes a while to compute. See cl/309175318 for
+    # discussion.
+    with gfile.Open(file_path, 'wb') as f:
+      f.write(hlo_module_proto_str)
+  elif ext == '.txt':
+    with gfile.Open(file_path, 'w') as f:
+      f.write(hlo_txt)
+
+
+# END GOOGLE-INTERNAL
 
 
 def count_ops_in_hlo_proto(hlo_proto: hlo_pb2.HloModuleProto,
                            ops_regex: str) -> int:
   """Counts specific ops in hlo proto, whose names match the provided pattern.
 
   Args:
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/hlo_utils_test.py` & `aqtp-0.1.1/jax_legacy/jax/hlo_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/check_config_util.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/check_config_util.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/base_config.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs_script/config_schema_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,14 +105,25 @@
   def test_schema_matches_expected(self, num_blocks):
     # This tests that the schema of the configdict returned by 'config_schema',
     # once all references are resolved, matches an expected schema. 'Schema'
     # here means the names and structure of fields at each level of the
     # configuration hierarchy. A value of 'None' in the expected schemas defined
     # below indicates a real configuration would have a concrete scalar value
     # there.
+    # BEGIN GOOGLE-INTERNAL
+    sparsity_schema = {
+        'type': None,
+        'prune_rate': [None, None],  # set to default structured
+        'smallest': None,
+        'order': None,
+        'absolute': None,
+        'structure_decay': None,
+        'sparse_ste': None
+    }
+    # END GOOGLE-INTERNAL
     quant_act_schema = {
         'bounds': {
             'initial_bound': None,
             'stddev_coeff': None,
             'absdev_coeff': None,
             'mix_coeff': None,
             'reset_stats': None,
@@ -126,32 +137,41 @@
             'cams_stddev_coeff': None,
             'mean_of_max_coeff': None,
             'use_old_code': None,
         },
         'input_distribution': None,
         'prec': None,
         'half_shift': None,
+        # BEGIN GOOGLE-INTERNAL
+        'sub_channels': None,
+        # END GOOGLE-INTERNAL
     }
 
     dense_schema = {
         'weight_prec': None,
         'weight_quant_granularity': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
+        # BEGIN GOOGLE-INTERNAL
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
         'weight_sparsity': sparsity_schema,
         'act_sparsity': sparsity_schema,
     }
 
     conv_schema = {
         'weight_prec': None,
         'weight_quant_granularity': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
+        # BEGIN GOOGLE-INTERNAL
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
     }
 
     residual_block_schema = {
         'conv_se': conv_schema,
         'conv_proj': conv_schema,
         'conv_1': conv_schema,
         'conv_2': conv_schema,
@@ -184,14 +204,18 @@
         'act_function': None,
         'shortcut_ch_shrink_method': None,
         'shortcut_ch_expand_method': None,
         'shortcut_spatial_method': None,
         'teacher_model': None,
         'is_teacher': None,
         'seed': None,
+        # BEGIN GOOGLE-INTERNAL
+        'sub_channels': None,
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
         'sparsity': sparsity_schema,
         'weight_sparsity': sparsity_schema,
         'act_sparsity': sparsity_schema,
         'lr_scheduler': {
             'warmup_epochs': None,
             'cooldown_epochs': None,
             'scheduler': None,
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/configs_test.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/configs_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/hparams_config.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/hparams_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/input_pipeline.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/models_test.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/pokebnn.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/pokebnn_test.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/pokebnn_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/resnet_cost_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 import jax.nn
 import jax.numpy as jnp
 from ml_collections import config_flags
 import optax
 import tensorflow.compat.v2 as tf
 from tensorflow.io import gfile
 
+# BEGIN GOOGLE-INTERNAL
+
+from vision_transformer.vit_jax import checkpoint as vit_checkpoint
+from vision_transformer.vit_jax import models as vit_models
+from vision_transformer.vit_jax.configs import models as models_config
+import google3.learning.deepmind.xmanager2.client.google as xm  # pylint: disable=unused-import
+
+# END GOOGLE-INTERNAL
 
 COMPUTE_MEMORY_COST_FILENAME = 'compute_memory_cost.json'
 
 FLAGS = flags.FLAGS
 
 flags.DEFINE_string(
     'model_dir', default=None, help=('Directory to store model data.'))
@@ -246,14 +254,17 @@
   # hparams.activation_bound_start_step. (For models with quantized weights,
   # weights are quantized from the beginning of training.)
   # However, for unquantized activations, hparams.activation_bound_start_step is
   # set to -1, but the report start_step cannot be negative, so the max()
   # sets the start_step to 0 in this case.
   report_start_step = max(0, hparams.activation_bound_start_step)
   create_end_of_training_report = report_utils.create_end_of_training_report
+  # BEGIN GOOGLE-INTERNAL
+  create_end_of_training_report = report_utils.create_end_of_training_report_internal
+  # END GOOGLE-INTERNAL
   report = create_end_of_training_report(
       model_dir=FLAGS.model_dir,
       eval_freq=eval_freq,
       num_train_steps=num_train_steps,
       early_stop_attr='eval_accuracy',
       early_stop_agg=report_utils.MinOrMax.MAX,
       early_stop_ds_dir=None,
@@ -261,14 +272,18 @@
       other_ds_dirs=None,
       tags_to_include=[
           'eval_accuracy', 'eval_loss', 'train_accuracy', 'train_loss',
           'train_learning_rate'
       ],
       window_size_in_steps=eval_freq * 5,
       start_step=report_start_step,
+      # BEGIN GOOGLE-INTERNAL
+      xid=FLAGS.xm_xid,
+      wid=FLAGS.xm_wid
+      # END GOOGLE-INTERNAL
   )
   logging.info('report created.')
   if FLAGS.report_dir is None:
     report_dir = FLAGS.model_dir
   else:
     report_dir = FLAGS.report_dir
   report_path = report_utils.save_report(report, report_dir)
@@ -387,14 +402,39 @@
     teacher = {
         'model':
             lambda var, img, labels: jax.nn.softmax(
                 teacher_model.apply(var, img)),
         'variables':
             teacher_variables,
     }
+  # BEGIN GOOGLE-INTERNAL
+  elif hparams.teacher_model == 'vit':
+    # Hide ViT as google internal since model creation depends on google3
+    # create a ViT model and load checkpoints
+    # Select a fine-tuned checkpoint from ViT model table.
+    # The ViT model is R50+L/32, and is pretrained on imagenet21k for 300 epochs
+    # The selected checkpoint has a final val acc of 0.897908 on imagenet2012
+    model_config = models_config.AUGREG_CONFIGS['R50_L_32']
+    # The model checkpoint is stored in the cloud
+    vit_path = '/cns/tp-d/home/yichizh/R50_L_32_i21k_300ep_imagenet2012_20ksteps.npz'
+    # Get model instance - no weights are initialized yet.
+    # hard code num of classes to 1000 for imagenet2012
+    teacher_model = vit_models.VisionTransformer(
+        num_classes=1000, **model_config)
+    # Load a checkpoint from cloud
+    teacher_variables = {'params': vit_checkpoint.load(vit_path)}
+    # create a dictionary for better argument passing
+    teacher = {
+        'model':
+            lambda var, img, labels: jax.nn.softmax(
+                teacher_model.apply(var, img, train=False)),
+        'variables':
+            teacher_variables,
+    }
+  # END GOOGLE-INTERNAL
   elif hparams.teacher_model == 'labels':
     teacher = {
         'model':
             lambda var, img, labels: common_utils.onehot(
                 labels, num_classes=1000),
         'variables': {},  # no need of variables in this case
     }
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_benchmark.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/train_benchmark.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_test.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/imagenet/train_utils.py` & `aqtp-0.1.1/jax_legacy/jax/imagenet/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/primitives.py` & `aqtp-0.1.1/jax_legacy/jax/primitives.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/primitives_test.py` & `aqtp-0.1.1/jax_legacy/jax/primitives_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/quant_config.py` & `aqtp-0.1.1/jax_legacy/jax/quant_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/quantization.py` & `aqtp-0.1.1/jax_legacy/jax/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,17 @@
     """Parameters for weight quantization."""
     prec: _PrecT  # expected precision for weight quantization.
     # enable all available values during quantization
     half_shift: bool
     # Axis along which to quantize weights (the non-feature axis).
     axis: Optional[Iterable[int]]
 
+    # BEGIN GOOGLE-INTERNAL
+    sub_channels: Optional[int] = None
+    # END GOOGLE-INTERNAL
 
     # expected scale shape for weights quantization. Defaults to None.
     expected_scale_shape: Union[None, int, Tuple[int, ...]] = None
 
   @dataclass
   class ActHParams:
     """Parameters for activation quantization."""
@@ -168,14 +171,17 @@
 
     input_distribution: InputDistribution
     # float means fixed bound. '-1' means no quantization.
     bounds: ActsBoundT
     prec: _PrecT
     half_shift: bool
 
+    # BEGIN GOOGLE-INTERNAL
+    sub_channels: Optional[int] = None
+    # END GOOGLE-INTERNAL
 
   def __init__(
       self,  #
       *,
       prec: Union[int, _FloatQuant],
       scale: Optional[jnp.ndarray],
       symmetric: bool,
@@ -406,14 +412,18 @@
     half_shift = weight_params.half_shift
     if isinstance(prec, _FloatQuant):
       ops = cls.create_symmetric_fp(bounds=weight_bounds, fp_quant=prec)
     else:
       ops = cls.create_symmetric(
           bounds=weight_bounds, prec=prec, half_shift=half_shift)
 
+    # BEGIN GOOGLE-INTERNAL
+    if weight_params.sub_channels is not None:
+      return ops
+    # END GOOGLE-INTERNAL
 
     if weight_params.expected_scale_shape is not None:
       # NOTE: We set keepdim to True when computing weights scale, as a result
       # the axes which are reduced are left in the result as dimensions with
       # size one. User should correctly pass the shape with reduced dimensions
       # set to 1.
       ops.assert_scale_shape_is(shape=weight_params.expected_scale_shape)
@@ -449,19 +459,39 @@
     """
     # TODO(yichi): if weight_params.prec is None or weight_binarize flag True:
     if weight_params.prec is None or not quantize_weights:
       return w
 
     weight_shape = w.shape
 
+    # BEGIN GOOGLE-INTERNAL
+    if weight_params.sub_channels and weight_params.sub_channels > 1:
+      # TODO(shivaniagrawal): we can relax this condition.
+      assert len(weight_shape) == 2, ('weight has shape %s' % weight_shape)
+
+      n = weight_params.sub_channels
+      logging.info('Applying sub channel quantization.')
+      if weight_shape[0] % n != 0:
+        raise ValueError(f'Shape of weight: {weight_shape} is not compatible '
+                         f'for applying sub channel: {n}')
+      # increase the number of channels by n
+      w = w.reshape((int(weight_shape[0] / n), int(weight_shape[1] * n)))
+
+    # END GOOGLE-INTERNAL
 
     ops = cls.create_weights_ops(w, weight_params=weight_params)
     weight_rescaled = ops.fake_quant(
         w, quantized_type=quantized_type, fake_dependency=fake_dependency)
 
+    # BEGIN GOOGLE-INTERNAL
+    if weight_params.sub_channels and weight_params.sub_channels > 1:
+      logging.info('DeApplying sub channel quantization.')
+      weight_rescaled = weight_rescaled.reshape(weight_shape)
+
+    # END GOOGLE-INTERNAL
 
     return weight_rescaled
 
   # TODO(malmaud): rename 'input' to activation here and elsewhere in this file.
   @classmethod
   def create_input_ops(
       cls, inputs: jnp.ndarray, *, hparams: ActHParams,
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/quantization_test.py` & `aqtp-0.1.1/jax_legacy/jax/quantization_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/shape_utils.py` & `aqtp-0.1.1/jax_legacy/jax/shape_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/sparsity.py` & `aqtp-0.1.1/jax_legacy/jax/sparsity.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/sparsity_test.py` & `aqtp-0.1.1/jax_legacy/jax/sparsity_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/stats.py` & `aqtp-0.1.1/jax_legacy/jax/stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag.py` & `aqtp-0.1.1/jax_legacy/jax/stats_tag.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/stats_tag_test.py` & `aqtp-0.1.1/jax_legacy/jax/stats_tag_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/stats_test.py` & `aqtp-0.1.1/jax_legacy/jax/stats_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/test_utils.py` & `aqtp-0.1.1/jax_legacy/jax/test_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/train_utils.py` & `aqtp-0.1.1/jax_legacy/jax/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/train_utils_test.py` & `aqtp-0.1.1/jax_legacy/jax/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/utils.py` & `aqtp-0.1.1/jax_legacy/jax/utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/bleu.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/bleu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/decode.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/decode.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/gen_hlo.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,17 @@
 def get_embedding_config(
     parent_config: ml_collections.ConfigDict) -> ml_collections.ConfigDict:
   """Create a ConfigDict corresponding to aqt.flax_layers.Embedding.HParams."""
   config = ml_collections.ConfigDict()
   config_schema_utils.set_default_reference(
       config, parent_config,
       ["weight_prec", "quant_type", "quant_act", "weight_half_shift",
+       # BEGIN GOOGLE-INTERNAL
+       "weight_sub_channels",
+       # END GOOGLE-INTERNAL
        ])
   config.lock()
   return config
 
 
 def get_config(n_layers: int, use_auto_acts: bool,
                fp_quant: bool) -> ml_collections.ConfigDict:
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,31 +193,40 @@
             'exclude_zeros': None,
             'use_mean_of_max': None,
             'granularity': None
         },
         'input_distribution': None,
         'prec': None,
         'half_shift': None,
+        # BEGIN GOOGLE-INTERNAL
+        'sub_channels': None,
+        # END GOOGLE-INTERNAL
     }
 
     dense_schema = {
         'weight_prec': None,
         'weight_quant_granularity': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
+        # BEGIN GOOGLE-INTERNAL
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
         'weight_sparsity': sparsity_schema,
         'act_sparsity': sparsity_schema,
     }
 
     embedding_schema = {
         'weight_prec': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_half_shift': None,
+        # BEGIN GOOGLE-INTERNAL
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
     }
 
     mlp_block_schema = {
         'dense_1': dense_schema,
         'dense_2': dense_schema,
     }
 
@@ -282,14 +291,18 @@
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_quant_granularity': None,
         'dense': dense_schema,
         'embedding': embedding_schema,
         'mlp_block': mlp_block_schema,
         'attention': attention_schema,
+        # BEGIN GOOGLE-INTERNAL
+        'sub_channels': None,
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
         'sparsity': sparsity_schema,
         'weight_sparsity': sparsity_schema,
         'act_sparsity': sparsity_schema,
         'model_hparams': {
             'emb_dim': None,
             'num_heads': None,
             'qkv_dim': None,
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py` & `aqtp-0.1.1/jax_legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/input_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import jax
 
 import tensorflow.compat.v2 as tf
 import tensorflow_datasets as tfds
 import tensorflow_text as tftxt
 
-from sentencepiece import SentencePieceTrainer
+from google3.third_party.sentencepiece.src.python.sentencepiece_trainer import SentencePieceTrainer
 
 AUTOTUNE = tf.data.experimental.AUTOTUNE
 
 
 # -----------------------------------------------------------------------------
 # Raw TFDS dataset.
 # -----------------------------------------------------------------------------
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/models_test.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/predict.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         dynamic_context=dynamic_context,
         hparams=hparams,
         should_decode=True,
         dropout_rate=0.0,
         attention_dropout_rate=0.0,
         use_bfloat16=False)
     mutable = ['cache']
+    # BEGIN GOOGLE-INTERNAL
+    mutable = ['cache', 'sparsity']
+    # END GOOGLE-INTERNAL
     flat_logits, new_vars = model.apply(
         {
             'params': params,
             'cache': flat_cache,
             **state
         },
         encoded=encoded_inputs,
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 from absl import logging
 
 from aqt.jax_legacy.jax import compute_cost_utils
 from aqt.jax_legacy.jax import hlo_utils
 from aqt.jax_legacy.jax import quant_config
 from aqt.jax_legacy.jax import train_utils
 
+# BEGIN GOOGLE-INTERNAL
+from aqt.jax_legacy.jax.google import custom_losses
+# END GOOGLE-INTERNAL
 
 from aqt.jax_legacy.jax.wmt_mlperf import bleu
 from aqt.jax_legacy.jax.wmt_mlperf import input_pipeline
 from aqt.jax_legacy.jax.wmt_mlperf import models
 from aqt.jax_legacy.jax.wmt_mlperf import predict
 
 # train_flags is imported for the side effect of flag definitions.
@@ -63,26 +66,54 @@
 import jax.numpy as jnp
 from ml_collections import config_flags
 import numpy as np
 import sacrebleu
 import tensorflow.compat.v2 as tf
 import tensorflow_text as tftxt
 
+# BEGIN GOOGLE-INTERNAL
+# Importing xm to define xm flags as suggested in
+# https://yaqs.corp.google.com/eng/q/4603557278646272#a5707702298738688
+import google3.learning.deepmind.xmanager2.client.google as xm  # pylint: disable=unused-import
+
+from google3.pyglib import timer
+from google3.pyglib.contrib.gpathlib import gpath
+# END GOOGLE-INTERNAL
 
 
 flax.config.update('flax_use_orbax_checkpointing', False)
 
 T = TypeVar('T')
 
 EOS_TOKEN = 2  # Default Sentencepiece EOS token.
 
 COMPUTE_MEMORY_COST_FILENAME = 'compute_memory_cost.json'
 
 FLAGS = flags.FLAGS
 
+# BEGIN GOOGLE-INTERNAL
+
+CONFIG_DIR = gpath.GPath(
+    'google3/third_party/py/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs')
+
+# TODO(b/175245107): Get rid of this 'hparams_config_filename' flag that points
+# to a JSON file in favor of hparams_config_dict, which points to a file
+# defining a configdict. Just have to update train_test, which still relies on
+# JSON-based config files.
+flags.DEFINE_string(
+    'hparams_config_filename',
+    default=None,
+    help=(
+        'Path to a JSON file in google3 that specifies a TrainingHParams'
+        ' instance. If relative, it is interpreted as relative to'
+        ' hparams_configs in Piper. If absolute, it can be anywhere loadable by'
+        ' gfile.'
+    ),
+)
+# END GOOGLE-INTERNAL
 
 flags.DEFINE_bool(
     'log_sparsity_scalars',
     default=True,
     help=(
         'Log `apply_sparsity`, `update_weight_sparsity` and '
         '`update_act_sparsity`  scalars to Tensorboard'
@@ -361,14 +392,21 @@
         mutable=True,
         rngs={'dropout': dropout_rng})
     new_state, _ = flax.core.pop(new_variables, 'params')
     loss, weight_sum = compute_weighted_cross_entropy(logits, targets, weights)
     mean_loss = loss / weight_sum
     total_loss = mean_loss
 
+    # BEGIN GOOGLE-INTERNAL
+    if hparams.weight_outlier_regularization != 0.0:
+      or_loss = custom_losses.weight_outlier_regularization_loss(
+          params,
+          weights_regex_pattern=hparams.weight_outlier_regularization_regex)
+      total_loss = mean_loss + hparams.weight_outlier_regularization * or_loss
+    # END GOOGLE-INTERNAL
 
     return total_loss, (logits, new_state)
 
   step = optimizer.state.step
   learning_rate_fn = create_learning_rate_scheduler(
       hparams.learning_rate_schedule)
   lr = learning_rate_fn(step)
@@ -382,14 +420,22 @@
     metrics = {}
   metrics['learning_rate'] = lr
   metrics['apply_sparsity'] = dynamic_context.apply_sparsity
   metrics['num_update_sparsity'] = dynamic_context.num_update_sparsity
   metrics['update_weight_sparsity'] = dynamic_context.update_weight_sparsity
   metrics['update_act_sparsity'] = dynamic_context.update_act_sparsity
 
+  # BEGIN GOOGLE-INTERNAL
+  # Compute or_loss for logging
+  # TODO(wanglisa): Is there a way to avoid computing it twice?
+  or_loss = custom_losses.weight_outlier_regularization_loss(
+      optimizer.target,
+      weights_regex_pattern=hparams.weight_outlier_regularization_regex)
+  metrics['or_loss'] = or_loss
+  # END GOOGLE-INTERNAL
 
   return new_state, new_optimizer, metrics, new_dropout_rng
 
 # TODO(shivaniagrawal): parametrize the axis_name and use the same axis name
 # throughout Transformer model.
 p_train_step = jax.pmap(
     functools.partial(train_step),
@@ -964,14 +1010,58 @@
         train_ds=train_ds,
         eval_ds_dict=eval_ds_dict,
         train_eval_ds=train_eval_ds,
         predict_ds_dict=predict_ds_dict,
         encoder=encoder)
 
 
+# BEGIN GOOGLE-INTERNAL
+def prepare_and_save_report(datasets: Datasets,
+                            hparams: training_hparams.TrainingHParams) -> None:
+  """Creates a report for this run and saved it to FLAGS.report_dir."""
+  other_ds_dirs = [pathlib.Path('train')]
+  for eval_dataset_name in datasets.eval_ds_dict:
+    if eval_dataset_name == FLAGS.eval_dataset_name:
+      continue
+    other_ds_dirs.append(
+        pathlib.Path(eval_ds_name_to_summary_dir(eval_dataset_name)))
+
+  # Make window large enough to cover approx. 5 events, and no bigger than
+  # number of training steps.
+  window_size_in_steps = min(FLAGS.eval_frequency * 5, hparams.num_train_steps)
+
+  # For models with quantization, we should only do early stopping after the
+  # model is quantized during training, so after
+  # hparams.activation_bound_start_step. (For models with quantized weights,
+  # weights are quantized from the beginning of training.)
+  # However, for unquantized activations, hparams.activation_bound_start_step is
+  # set to -1, but the report start_step cannot be negative, so the max()
+  # sets the start_step to 0 in this case.
+  report_start_step = max(0, hparams.activation_bound_start_step)
+  report = report_utils.create_end_of_training_report_internal(
+      model_dir=FLAGS.model_dir,
+      xid=FLAGS.xm_xid,
+      eval_freq=FLAGS.eval_frequency,
+      num_train_steps=hparams.num_train_steps,
+      early_stop_attr='perplexity',
+      early_stop_agg=report_utils.MinOrMax.MIN,
+      early_stop_ds_dir=pathlib.Path('eval'),
+      smoothing_kernel=report_utils.SmoothingKernel.RECTANGULAR,
+      other_ds_dirs=other_ds_dirs,
+      tags_to_include=[
+          'accuracy', 'loss', 'or_loss', 'perplexity', 'bleu', 'sacrebleu'
+      ],
+      window_size_in_steps=window_size_in_steps,
+      start_step=report_start_step,
+      wid=FLAGS.xm_wid)
+
+  report_path = report_utils.save_report(report, pathlib.Path(FLAGS.report_dir))
+  logging.info('Report saved to %s.', str(report_path))
+
+# END GOOGLE-INTERNAL
 
 
 def main(argv):
   if len(argv) > 1:
     raise app.UsageError('Too many command-line arguments.')
   # This seems to be necessary even when importing TF2?
   tf.enable_v2_behavior()
@@ -981,14 +1071,21 @@
     if 'configs' in FLAGS.hparams_config_dict:
       hparams_config_dict = FLAGS.hparams_config_dict.configs[FLAGS.config_idx]
     else:
       hparams_config_dict = FLAGS.hparams_config_dict
     hparams = hparams_utils.load_dataclass_from_config_dict(
         training_hparams.TrainingHParams, hparams_config_dict)
 
+  # BEGIN GOOGLE-INTERNAL
+  # TODO(shivaniagrawal): This piece of code is to be deprecated.
+  elif FLAGS.hparams_config_filename:
+    hparams = hparams_utils.load_dataclass_from_disk(
+        training_hparams.TrainingHParams,
+        gpath.GPath(FLAGS.hparams_config_filename), CONFIG_DIR)
+  # END GOOGLE-INTERNAL
 
   # Number of local devices for this host.
   n_devices = jax.local_device_count()
 
   if hparams.per_host_batch_size % n_devices:
     raise ValueError(
         f'Batch size must be divisible by the number of devices. Got batch '
@@ -1003,14 +1100,25 @@
       hparams.random_seed,
       eval_dataset_list=eval_dataset_names_list,
       batch_size=hparams.per_host_batch_size)
 
   with concurrent.futures.ThreadPoolExecutor(max_workers=1) as io_executor:
     run_training(datasets=datasets, hparams=hparams, io_executor=io_executor)
 
+  # BEGIN GOOGLE-INTERNAL
+  if jax.host_id() == 0:
+    if FLAGS.report_dir:
+      if gpath.GPath(FLAGS.report_dir).exists():
+        prepare_and_save_report(datasets=datasets, hparams=hparams)
+      else:
+        logging.info('%s does not exist, could not save report.',
+                     FLAGS.report_dir)
+    else:
+      logging.info('No report saved, since no --report_dir provided.')
+  # END GOOGLE-INTERNAL
 
 
 def save_best_checkpoint(*, model_dir: str, training_state: TrainingState,
                          loss: float) -> None:
   """Saves a checkpoint if 'loss' is smaller than the loss of the previous best-model checkpoint."""
 
   prefix = 'best_checkpoint_eval_loss_'
@@ -1058,17 +1166,38 @@
     state_dict_keys.extend([
         'min_per_ch', 'max_per_ch', 'mean_per_ch', 'stddev_per_ch',
         'absdev_per_ch', 'stddev_per_ch_uncentered', 'absdev_per_ch_uncentered',
     ])
   return state_dict_keys
 
 
+# BEGIN GOOGLE-INTERNAL
+def _write_state_dict_to_cns(last_state_dict_summary, step):
+  """Write out state dict to CNS."""
+  stats_path = gpath.GPath(FLAGS.model_dir) / 'stats'
+  stats_output = stats_path / f'{step}.pkl'
+  if not stats_path.is_dir():
+    stats_path.mkdir()
+
+  with stats_output.open('wb') as stats_file:
+    stats_to_pickle = jax.tree_map(
+        lambda e: np.array(e.astype(jnp.float32)),
+        last_state_dict_summary,
+    )
+    pickle.dump(stats_to_pickle, stats_file)
+
+
+# END GOOGLE-INTERNAL
 
 
 def eval_ds_name_to_summary_dir(eval_dataset_name: str) -> str:
+  # BEGIN GOOGLE-INTERNAL
+  return 'eval_' + str('--'.join(gpath.GPath(eval_dataset_name).parts))
+  # pylint: disable=unreachable
+  # END GOOGLE-INTERNAL
   return 'eval_' + str('--'.join(os.path.abspath(eval_dataset_name).parts))
 
 
 def does_checkpoint_exist(model_dir: str) -> bool:
   """Determine if a checkpoint for this training run has already been saved."""
   # The model directory where checkpoints are saved doesn't exist yet.
   if not tf.io.gfile.exists(model_dir):
@@ -1202,14 +1331,18 @@
           hparams=hparams,
           transformer_kwargs=transformer_kwargs)
     state = jax_utils.replicate(state)
     optimizer = optimizer.replicate()
     logging.info('Replicated optimizer.')
 
   t_loop_start = time.time()
+  # BEGIN GOOGLE-INTERNAL
+  t_train = timer.MultiIntervalTimer()
+  t_train.Start()
+  # END GOOGLE-INTERNAL
   for step, batch in zip(range(start_step, num_train_steps), train_iter):
     # Shard data to devices and do a training step.
     training_state, metrics = run_train_step(
         training_state=training_state, batch=batch, step=step, hparams=hparams)
     state = training_state.flax_state
     optimizer = training_state.optimizer
     metrics_all.append(metrics)
@@ -1218,59 +1351,91 @@
     state_dict_summary_all.append(state_dict_summary)
 
     # Save a Checkpoint
     if step % FLAGS.checkpoint_freq == 0 and step > 0:
       if jax.host_id() == 0 and FLAGS.save_checkpoints:
         training_state.save_checkpoint(model_dir=FLAGS.model_dir, step=step)
 
+    # BEGIN GOOGLE-INTERNAL
+    # Periodic statistics serialization.
+    if jax.host_id() == 0 and step % stats_serialization_freq == 0:
+      t_train.Stop()
+      # Individual entries in state_dict_summary_all are not modified after
+      # insertion and can't have race conditions.
+      io_executor.submit(
+          _write_state_dict_to_cns,
+          state_dict_summary_all[-1],
+          step,
+      )
+      t_train.Start()
+    # END GOOGLE-INTERNAL
 
     # Periodic metric handling.
     if step % eval_freq == 0:
+      # BEGIN GOOGLE-INTERNAL
+      t_train.Stop()
+      # END GOOGLE-INTERNAL
 
       # Training Metrics
       if FLAGS.compute_train_metrics:
         metrics_all = common_utils.get_metrics(metrics_all)
         state_dict_summary_all = common_utils.get_metrics(
             state_dict_summary_all)
         lr = metrics_all.pop('learning_rate').mean()
 
         metrics_sums = jax.tree_map(jnp.sum, metrics_all)
         denominator = metrics_sums.pop('denominator')
+        # BEGIN GOOGLE-INTERNAL
+        or_loss = metrics_sums.pop('or_loss').mean()
+        # END GOOGLE-INTERNAL
         summary = jax.tree_map(lambda x: x / denominator, metrics_sums)  # pylint: disable=cell-var-from-loop
         summary['learning_rate'] = lr
         if FLAGS.log_sparsity_scalars:
           apply_sparsity = metrics_all.pop('apply_sparsity').mean()
           update_weight_sparsity = metrics_all.pop(
               'update_weight_sparsity').mean()
           update_act_sparsity = metrics_all.pop('update_act_sparsity').mean()
           num_update_sparsity = metrics_all.pop('num_update_sparsity').mean()
           summary['apply_sparsity'] = apply_sparsity
           summary['update_weight_sparsity'] = update_weight_sparsity
           summary['update_act_sparsity'] = update_act_sparsity
           summary['num_update_sparsity'] = num_update_sparsity
+        # BEGIN GOOGLE-INTERNAL
+        summary['or_loss'] = or_loss
+        # END GOOGLE-INTERNAL
         summary['perplexity'] = jnp.clip(jnp.exp(summary['loss']), a_max=1.0e4)
         logging.info('train in step: %d, loss: %.4f', step, summary['loss'])
         steps_per_eval = eval_freq if step != 0 else 1
         steps_per_sec = steps_per_eval / (time.time() - t_loop_start)
+        # BEGIN GOOGLE-INTERNAL
+        train_steps_per_sec = steps_per_eval / t_train.GetDuration()
+        # END GOOGLE-INTERNAL
         t_loop_start = time.time()
 
         if jax.host_id() == 0:
           assert train_summary_writer is not None, ('train_summary_writer was '
                                                     'not initialized on host 0')
           train_summary_writer.scalar('steps per second', steps_per_sec, step)
+          # BEGIN GOOGLE-INTERNAL
+          train_summary_writer.scalar('training steps per second',
+                                      train_steps_per_sec, step)
+          # END GOOGLE-INTERNAL
           for key, val in summary.items():
             train_summary_writer.scalar(key, val, step)
 
           summary_utils.write_state_dict_summaries_to_tb(
               state_dict_summary_all, train_summary_writer,
               FLAGS.state_dict_summary_freq, step)
           train_summary_writer.flush()
 
       state_dict_summary_all = []
       metrics_all = []
+      # BEGIN GOOGLE-INTERNAL
+      logging.info('train time: %.4f s step %d', t_train.GetDuration(), step)
+      # END GOOGLE-INTERNAL
 
       # TODO(shivaniagrawal): Add bleu score summaries for additional eval
       # datasets?
       # Additional eval metrics
       for eval_dataset_name, eval_ds in datasets.eval_ds_dict.items():
         summary_writer = None
         t_add_eval_start = time.time()
@@ -1356,11 +1521,16 @@
         assert eval_summary_writer is not None, ('eval_summary_writer was not '
                                                  'initialized on host 0')
         eval_summary_writer.scalar('bleu', bleu_score, step)
         eval_summary_writer.scalar('sacrebleu', sacrebleu_score, step)
         eval_summary_writer.text('samples', exemplars, step)
         eval_summary_writer.flush()
 
+      # BEGIN GOOGLE-INTERNAL
+      # restart training-only timer
+      t_train.Reset()
+      t_train.Start()
+      # END GOOGLE-INTERNAL
 
 
 if __name__ == '__main__':
   app.run(main)
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/train_flags.py`

 * *Files 5% similar despite different names*

```diff
@@ -184,7 +184,14 @@
     'state_dict_summary_freq',
     default=200,
     help=(
         'Number of training steps between state dict summaries reported to '
         'Tensorboard. Relevant to --visualize_acts_bound and --collect_acts_stats.'
     ))
 
+# BEGIN GOOGLE-INTERNAL
+flags.DEFINE_string(
+    'report_dir',
+    default='/cns/tp-d/home/cerebra-catalyst/exp_reports/wmt_mlperf',
+    help=('Directory to save experiment report '
+          'to after training has completed. '))
+# END GOOGLE-INTERNAL
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/train_test.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/training_hparams.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py` & `aqtp-0.1.1/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 from aqt.jax_legacy.jax.quantization import QuantType
 from aqt.jax_legacy.jax.wmt_mlperf import models
 from aqt.jax_legacy.jax.wmt_mlperf import training_hparams
 from aqt.jax_legacy.utils import hparams_utils as os_hparams_utils
 
 T = TypeVar('T')
 
+# BEGIN GOOGLE-INTERNAL
+HPARAMS_CONFIG_DIR = pathlib.Path(
+    'third_party/py/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/'
+)
+# END GOOGLE-INTERNAL
 
 # Default fixed bound and getbounds coefficients
 # These values were determined empirically to be reasonable defaults.
 
 DEFAULTS = {}
 DEFAULTS['mlp_dense_1'] = {
     'fixed': 1.0,
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/__init__.py` & `aqtp-0.1.1/tensorflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/common.py` & `aqtp-0.1.1/jax_legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils.py` & `aqtp-0.1.1/jax_legacy/utils/config_schema_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,26 +125,32 @@
           "weight_prec",
           "weight_quant_granularity",
           "quant_type",
           "quant_act",
           "weight_half_shift",
           "act_sparsity",
           "weight_sparsity",
+          # BEGIN GOOGLE-INTERNAL
+          "weight_sub_channels",
+          # END GOOGLE-INTERNAL
       ])
   config.lock()
   return config
 
 
 def get_conv_config(
     parent_config: ml_collections.ConfigDict) -> ml_collections.ConfigDict:
   """Creates a ConfigDict corresponding to aqt.flax_layers.ConvAqt.HParams."""
   config = ml_collections.ConfigDict()
   set_default_reference(config, parent_config, [
       "weight_prec", "weight_quant_granularity", "quant_type", "quant_act",
       "weight_half_shift",
+      # BEGIN GOOGLE-INTERNAL
+      "weight_sub_channels",
+      # END GOOGLE-INTERNAL
   ])
   config.lock()
   return config
 
 
 def get_fp_quant_config() -> ml_collections.ConfigDict:
   config = ml_collections.ConfigDict({
@@ -215,14 +221,17 @@
           "hyper_str": str_ph(),
       },
       "weight_decay": float_ph(),
       "activation_bound_update_freq": int_ph(),
       "activation_bound_start_step": int_ph(),
       "prec": prec,
       "sparsity": sparsity,
+      # BEGIN GOOGLE-INTERNAL
+      "sub_channels": int_ph(),
+      # END GOOGLE-INTERNAL
       "half_shift": bool_ph(),
       "quant_type": str_ph(),
       "quant_act": {
           "bounds": bounds,
           # TODO(shivaniagrawal): The input distribution is really an intrinsic
           # model property and shouldn't be part of the model configuration.
           # Update the hparam dataclasses to eliminate the input_distribution
@@ -235,13 +244,21 @@
   set_default_reference(
       base_config, base_config, "weight_prec", parent_field="prec")
   set_default_reference(base_config.quant_act, base_config, "prec")
   set_default_reference(
       base_config, base_config, "act_sparsity", parent_field="sparsity")
   set_default_reference(
       base_config, base_config, "weight_sparsity", parent_field="sparsity")
+  # BEGIN GOOGLE-INTERNAL
+  set_default_reference(
+      base_config,
+      base_config,
+      "weight_sub_channels",
+      parent_field="sub_channels")
+  set_default_reference(base_config.quant_act, base_config, "sub_channels")
+  # END GOOGLE-INTERNAL
 
   set_default_reference(
       base_config, base_config, "weight_half_shift", parent_field="half_shift")
   set_default_reference(base_config.quant_act, base_config, "half_shift")
 
   return base_config
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/config_schema_utils_test.py` & `aqtp-0.1.1/jax_legacy/utils/config_schema_utils_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,21 +251,27 @@
               'exclude_zeros': None,
               'use_mean_of_max': None,
               'granularity': None
           },
           'input_distribution': None,
           'prec': prec,
           'half_shift': None,
+          # BEGIN GOOGLE-INTERNAL
+          'sub_channels': None,
+          # END GOOGLE-INTERNAL
       }
     else:
       quant_act_schema = {
           'bounds': None,
           'input_distribution': None,
           'prec': prec,
           'half_shift': None,
+          # BEGIN GOOGLE-INTERNAL
+          'sub_channels': None,
+          # END GOOGLE-INTERNAL
       }
     prune_rate = None if use_unstructured else [None, None]
     sparsity = {
         'type': None,
         'prune_rate': prune_rate,
         'smallest': None,
         'order': None,
@@ -284,14 +290,18 @@
         'prec': prec,
         'half_shift': None,
         'weight_prec': prec,
         'weight_half_shift': None,
         'quant_type': None,
         'quant_act': quant_act_schema,
         'weight_quant_granularity': None,
+        # BEGIN GOOGLE-INTERNAL
+        'sub_channels': None,
+        'weight_sub_channels': None,
+        # END GOOGLE-INTERNAL
         'sparsity': sparsity,  # Top level sparsity value, sets both weight and
         # activation sparsity,
         'weight_sparsity': sparsity,
         'act_sparsity': sparsity,
     }
 
     config = config_schema_utils.get_base_config(
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/hparams_utils.py` & `aqtp-0.1.1/jax_legacy/utils/hparams_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 from aqt.jax_legacy.jax import quantization
 from aqt.jax_legacy.jax import sparsity
 from aqt.jax_legacy.jax.flax import struct as flax_struct
 import dacite
 import jax
 import ml_collections
 
+# BEGIN GOOGLE-INTERNAL
+from google3.pyglib import gfile
+from google3.pyglib import resources
+from google3.pyglib.contrib.gpathlib import gpath
+# END GOOGLE-INTERNAL
 
 T = TypeVar('T')
 
 dataclass = flax_struct.dataclass if not typing.TYPE_CHECKING else dataclasses.dataclass
 
 
 @dataclass
@@ -77,14 +82,23 @@
   """
   if jax.host_id() == 0 and output_dir is not None:
     # The directory is usually created automatically by the time we reach here,
     # but on some training runs it appears not to be.
     # MakeDirs will create the directory if it doesn't already exist and is a
     # no-op if it already exists.
 
+    # BEGIN GOOGLE-INTERNAL
+    output_dir = gpath.GPath(output_dir)
+    gfile.MakeDirs(output_dir)
+    data_dict = dataclasses.asdict(hparams)
+    with gfile.Open(output_dir / 'hparams_config.json', 'w') as file:
+      json.dump(data_dict, file, indent=2)
+    return
+    # pylint: disable=unreachable
+    # END GOOGLE-INTERNAL
 
     os.makedirs(output_dir, exist_ok=True)
     save_dataclass_to_disk(hparams,
                            os.path.join(output_dir, 'hparams_config.json'))
 
 
 def load_dataclass_from_dict(dataclass_name: Type[T],
@@ -153,14 +167,52 @@
     An instance of 'dataclass' populated with the JSON data.
   """
 
   data_dict = json.loads(json_data)
   return load_dataclass_from_dict(dataclass_name, data_dict)
 
 
+# BEGIN GOOGLE-INTERNAL
+def load_dataclass_from_disk(
+    dataclass_name: Type[T],
+    path: gpath.GPath,
+    config_dir: Optional[gpath.GPath] = None) -> T:
+  """Loads dataclass from a JSON file on disk.
+
+  Args:
+    dataclass_name: Name of the dataclass.
+    path: Path to the JSON file to load the dataclass from. Either a path
+      relative to config_dir (next arg), or absolute path readable by gpath.
+    config_dir: Optional path to config file directory.
+
+  Returns:
+    An instance of `dataclass` populated with the JSON file data
+  """
+
+  if path.is_absolute():
+    json_data = path.read_text()
+  else:
+    if path.parts[0] == 'google3':
+      json_data = resources.GetResource(path, mode='rt')
+    else:
+      if not config_dir:
+        raise ValueError('If path is relative, config_dir must be specified.')
+      json_data = resources.GetResource(str(config_dir / path), mode='rt')
+  try:
+    dataclass_obj = load_dataclass_from_json(
+        dataclass_name=dataclass_name, json_data=json_data)
+  except Exception as err:
+    # Reraising exception with additional error message to provide more context.
+    # The catch-all is permitted according to the stype guide because the
+    # exception is reraised.
+    raise Exception(
+        f'Dataclass loading error: Json data at {path} could not be '
+        f'loaded into the dataclass of type {dataclass_name}.') from err
+  return dataclass_obj
+# END GOOGLE-INTERNAL
 
 
 # TODO(shivaniagrawal): functionality `load_hparams_from_file` is created for a
 # generic (model hparams independent) train_hparams class; either we should move
 # towards shared TrainHparams or remove the following functionalities.
 def load_hparams_from_config_dict(hparams_classname: Type[T],
                                   model_classname: Type[Any],
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils.py` & `aqtp-0.1.1/jax_legacy/utils/pandas_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,9 +281,9 @@
 
   Returns:
     A matplotlib boxplot of type matplotlib.axes._subplots.AxesSubplot.
 
   """
   grouped_df = pd.DataFrame(
       {group: values[column_to_plot] for group, values in df.groupby(by)})
-  medians = grouped_df.median().sort_values()
+  medians = grouped_df.median().sort_values()  # pytype: disable=attribute-error  # pandas-15-upgrade
   return grouped_df[medians.index].boxplot(rot=0, return_type='axes')
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/pandas_utils_test.py` & `aqtp-0.1.1/jax_legacy/utils/pandas_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/report_utils.py` & `aqtp-0.1.1/jax_legacy/utils/report_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 import time
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from aqt.jax_legacy.utils import hparams_utils
 from aqt.jax_legacy.utils import tfevent_utils
 import numpy as onp
 from tensorflow.io import gfile
+# BEGIN GOOGLE-INTERNAL
+from google3.googlex.positron.tensorflow.reporting import utils as xm_query_utils
+from google3.learning.deepmind.xmanager2.client import xmanager_api
+from google3.pyglib import gfile as pyglib_gfile
+from google3.pyglib.concurrent import parallel
+from google3.pyglib.contrib.gpathlib import gpath
+# END GOOGLE-INTERNAL
 
 # Constants
 COMPUTE_MEMORY_COST_FILENAME = 'compute_memory_cost.json'
 HPARAMS_CONFIG_FILENAME = 'hparams_config.json'
 REPORT_FILENAME = 'report.json'
 
 EventSeries = tfevent_utils.EventSeries
@@ -133,14 +140,30 @@
                          'window_size_in_steps must be provided.')
       return functools.partial(
           self.triangular_kernel, window_size_in_steps=window_size_in_steps)
     else:
       raise ValueError('SmoothingKernel enum option not recognized.')
 
 
+# BEGIN GOOGLE-INTERNAL
+@dataclasses.dataclass
+class MetadataCorp:
+  """Google-internal experiment metadata."""
+
+  # XManager experiment ID.
+  xid: Optional[int] = None
+
+  # XManager worker ID.
+  wid: Optional[int] = None
+
+  # Information about the citc client from which experiment was launched.
+  citc_client_info: Optional[xm_query_utils.XManagerClientInfo] = None
+
+
+# END GOOGLE-INTERNAL
 
 
 @dataclasses.dataclass
 class ExperimentReport:
   """Report for a single experiment run based on its TFEvents files."""
   # Model directory corresponding to single run, with TFEvents files to
   # generate report from.
@@ -189,14 +212,22 @@
 
   # Tensorboard ID or URL.
   tensorboard_id: Optional[str] = None
 
   # Full path to hparams config file.
   hparams_config_path: Optional[str] = None
 
+  # BEGIN GOOGLE-INTERNAL
+  # Compute and memory cost information, for more details see
+  # googlex/positron/tensorflow/jax/shared_utils/compute_cost_utils.py.
+  compute_memory_cost: Optional[Dict[str, float]] = None
+
+  # Google-specific metadata (XManager, CitC etc.)
+  metadata_corp: Optional[MetadataCorp] = None
+  # END GOOGLE-INTERNAL
 
 
 def check_for_nans(event_series: EventSeries, start_step: int) -> Optional[int]:
   """Finds step >= start_step at which first NaN value occurs if there are any.
 
   Args:
     event_series: list of tuples (step, value).
@@ -558,7 +589,171 @@
   data_dict = dataclasses.asdict(report)
   path = pathlib.Path(report_dir / report_path / REPORT_FILENAME)
   with gfile.GFile(path, 'w') as file:
     json.dump(data_dict, file, indent=2)
   return report_dir / report_path
 
 
+# BEGIN GOOGLE-INTERNAL
+def create_end_of_training_report_internal(
+    model_dir: str,
+    xid: int,
+    eval_freq: int,
+    num_train_steps: int,
+    early_stop_attr: str,
+    early_stop_agg: MinOrMax,
+    smoothing_kernel: SmoothingKernel,
+    early_stop_ds_dir: Optional[pathlib.Path] = None,
+    other_ds_dirs: Optional[List[pathlib.Path]] = None,
+    tags_to_include: Optional[List[str]] = None,
+    window_size_in_steps: int = 1,
+    start_step: int = 0,
+    wid: Optional[int] = None,
+) -> ExperimentReport:
+  """Google-internal wrapper function of create_end_of_training_report().
+
+  Pulls additional information from XManager experiment to populate report.
+
+  Args:
+    model_dir: A model directory corresponding to a single model run, with
+      TFEvent file(s) and a single hparams_config file. The TFEvent files can
+      either be stored directly in model_dir, or in subdirectories in model_dir,
+      but not both.
+    xid: XManager experiment id. Used to retrieve metadata.
+    eval_freq: Frequency of event saving.
+    num_train_steps: Number of training steps.
+    early_stop_attr: Attribute to find minimum or maximum of, e.g. 'perplexity'.
+    early_stop_agg: Which aggregator to use to find early_stop_step. See
+      MinOrMax class for enum options.
+    smoothing_kernel: Which kernel to use for smoothing. See SmoothingKernel
+      class for enum options.
+    early_stop_ds_dir: The events subdir in model_dir to use to find
+      early_stop_step if model_dir has subdirs. The early_stop_attr within
+      early_stop_ds_dir will be used to find the early_stop_step.
+    other_ds_dirs: List of other subdirs in model_dir with events to report.
+    tags_to_include: List of event tags that should be included.
+    window_size_in_steps: Number of steps to average over. Should be multiple of
+      eval_freq. If set to 1, no averaging will be applied.
+    start_step: After which step to consider early stopping, e.g. if set to 100,
+      only steps >= 100 will be considered.
+    wid: XManager worker id.
+
+  Returns:
+    An ExperimentReport dataclass instance.
+
+  """
+
+  xm_client = xmanager_api.XManagerApi(xm_deployment_env='alphabet')
+  experiment = xm_client.get_experiment(xid)
+
+  experiment_name = experiment.name
+  user_name = experiment.author
+  launch_time = experiment.creation_time.strftime('%Y%m%dT%H%M%S')
+
+  xm_query = xm_query_utils.XManagerQuery([xid])
+  tensorboard_id = str(xm_query.xmanager_to_mldash_mapping()[xid])
+
+  if early_stop_ds_dir is not None:
+    early_stop_ds_dir = str(early_stop_ds_dir)
+  if other_ds_dirs is not None:
+    other_ds_dirs = [str(d) for d in other_ds_dirs]
+
+  report = create_end_of_training_report(
+      model_dir=model_dir,
+      eval_freq=eval_freq,
+      num_train_steps=num_train_steps,
+      early_stop_attr=early_stop_attr,
+      early_stop_agg=early_stop_agg,
+      smoothing_kernel=smoothing_kernel,
+      early_stop_ds_dir=early_stop_ds_dir,
+      other_ds_dirs=other_ds_dirs,
+      tags_to_include=tags_to_include,
+      window_size_in_steps=window_size_in_steps,
+      start_step=start_step,
+      experiment_name=experiment_name,
+      user_name=user_name,
+      launch_time=launch_time,
+      tensorboard_id=tensorboard_id,
+  )
+
+  compute_memory_cost = None
+  if COMPUTE_MEMORY_COST_FILENAME in pyglib_gfile.ListDir(model_dir):
+    with pyglib_gfile.Open(
+        model_dir / pathlib.Path(COMPUTE_MEMORY_COST_FILENAME), 'rt') as f:
+      compute_memory_cost = json.load(f)
+
+  metadata_corp = MetadataCorp(
+      xid=xid,
+      wid=wid,
+      citc_client_info=xm_query.xmanager_client_infos()[xid],
+  )
+
+  report.metadata_corp = metadata_corp
+  report.compute_memory_cost = compute_memory_cost
+  report.hparams_config_path = str(model_dir /
+                                   pathlib.Path(HPARAMS_CONFIG_FILENAME))
+
+  return report
+
+
+def load_report_fn(report_path: gpath.GPath) -> Optional[ExperimentReport]:
+  """Tries to load report from path, if it exists. Returns None otherwise."""
+  report = None
+  if not pyglib_gfile.Exists(report_path):
+    print(f'File {report_path} does not exist.')
+    return report
+
+  try:
+    report = hparams_utils.load_dataclass_from_disk(ExperimentReport,
+                                                    report_path)
+  except pyglib_gfile.FileError as file_error:
+    print(f'Failed to load file {report_path}.')
+    print(file_error)
+  return report
+
+
+def load_report(model_dir: gpath.GPath,
+                report_dir: gpath.GPath) -> Optional[ExperimentReport]:
+  """Loads existing ExperimentReport instance from report directory.
+
+  Args:
+    model_dir: Model directory of run to load report for (lookup key).
+    report_dir: Report directory in which reports are saved.
+
+  Returns:
+    An ExperimentReport instance.
+  """
+  model_report_path = report_path_from_model_dir(pathlib.Path(model_dir))
+  report_path = report_dir / model_report_path / REPORT_FILENAME
+  return load_report_fn(report_path)
+
+
+def load_all_reports(report_dir: gpath.GPath,
+                     num_threads: int) -> List[ExperimentReport]:
+  """Loads all reports from report directory.
+
+  Args:
+    report_dir: Report directory in which reports are saved.  Returns
+      ExperimentReport instance.
+    num_threads: Number of threads (threadpool workers) for parallelization.
+
+  Returns:
+    A list of ExperimentReport instances.
+  """
+  list_of_kwargs_to_function = [{
+      'report_path': report / REPORT_FILENAME
+  } for report in report_dir.iterdir()]
+  start = time.time()
+  reports = parallel.RunInParallel(
+      function=load_report_fn,
+      list_of_kwargs_to_function=list_of_kwargs_to_function,
+      num_workers=num_threads)
+  # remove None values from reports list
+  reports = [rep for rep in reports if rep]
+  end = time.time()
+  print(f'time to load reports: {end-start}')
+  print(f'Number of reports loaded: {len(reports)}')
+
+  return reports
+
+
+# END GOOGLE-INTERNAL
```

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/report_utils_test.py` & `aqtp-0.1.1/jax_legacy/utils/report_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils.py` & `aqtp-0.1.1/jax_legacy/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/summary_utils_test.py` & `aqtp-0.1.1/jax_legacy/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils.py` & `aqtp-0.1.1/jax_legacy/utils/tfevent_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/jax_legacy/utils/tfevent_utils_test.py` & `aqtp-0.1.1/jax_legacy/utils/tfevent_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_conv2d.py` & `aqtp-0.1.1/tensorflow/aqt_conv2d.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_conv2d_test.py` & `aqtp-0.1.1/tensorflow/aqt_conv2d_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_einsum.py` & `aqtp-0.1.1/tensorflow/aqt_einsum.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 In sum of sums (i,j->), both inputs have their only axes contract.
 
 Of course, if an axis is contracting, all axes across all inputs with the same
 label are contracting.
 """
 
 import string
-from typing import Tuple
+from typing import Dict, Iterable, Optional, Tuple
 
 from aqt.common import aqt_config
 from aqt.common import aqt_config_utils
+from aqt.tensorflow import aqt_ops_util
 from aqt.tensorflow import aqt_tensor
 import tensorflow.compat.v1 as tf
 
 # We repeatedly use protected methods from classes defined in other modules to
 # avoid exporting them as part of the public API.
 # pylint: disable=protected-access
 
@@ -177,7 +178,135 @@
 
     with tf.name_scope('inv_scale'):
       assert len(lhs_inv_scale.shape) == len(lhs.shape)
       assert len(rhs_inv_scale.shape) == len(rhs.shape)
       inv_scale = tf.einsum(eq, lhs_inv_scale, rhs_inv_scale,
                             **tf_einsum_kwargs)
       return out * inv_scale
+
+
+class Einsum:
+  """Encapsulates a quantized einsum op and calibration state."""
+
+  def __init__(
+      self,
+      eq: str,
+      config: aqt_config.AqtEinsumConfig,
+      lhs_shape: Iterable[Optional[int]],
+      rhs_shape: Iterable[Optional[int]],
+      name: str = 'einsum',
+      lhs_name: str = 'lhs',
+      rhs_name: str = 'rhs',
+  ):
+    """Creates a Einsum instance.
+
+    This encapsulates the state necessary for quantizing both
+    of the einsum arguments.
+
+    Args:
+      eq: the einsum equation.
+      config: an AqtEinsumConfig
+      lhs_shape: shape of the lhs tensor
+      rhs_shape: shape of the rhs tensor
+      name: variable scope for all variables to be created.
+      lhs_name: scope for left hand side variables only.
+      rhs_name: scope for right hand side variables only.
+    """
+    self.eq = eq
+    self.name = name
+    self.lhs_name = lhs_name
+    self.rhs_name = rhs_name
+
+    with tf.variable_scope(name):
+      self.lhs_quantizer = aqt_tensor.TensorQuantizer(
+          lhs_shape, config.lhs, name=lhs_name)
+      self.rhs_quantizer = aqt_tensor.TensorQuantizer(
+          rhs_shape, config.rhs, name=rhs_name)
+
+  def update_lhs(
+      self,
+      x: tf.Tensor,
+      weights: tf.Tensor,
+      event_count: tf.Tensor,
+  ) -> tf.Operation:
+    """Updates variables for an observation of the lhs.
+
+    Updating variables for an argument updates the statistics
+    for a new input to account for incremental observations of
+    a tensor's entries' magnitudes.
+
+    This also updates the scales, if they were set according to
+    a previous calibration config and now we've moved on to
+    a new event associated with a different calibration configuration
+    in the schedule.
+
+    Args:
+      x: a tensor for the observation of an lhs input
+      weights: a weight matrix broadcastable to x, representing how much weight
+        the corresponding axes should have on statistics associated with
+        quantizing that dimension.
+      event_count: the event of the observation
+
+    Returns:
+      The tf.Operation corresponding to the update
+    """
+    return self.lhs_quantizer.update(x, weights, event_count)
+
+  def update_rhs(
+      self,
+      x: tf.Tensor,
+      weights: tf.Tensor,
+      event_count: tf.Tensor,
+  ) -> tf.Operation:
+    """Computes analogue of update_lhs, but for rhs."""
+    return self.rhs_quantizer.update(x, weights, event_count)
+
+  def apply(
+      self,
+      lhs: tf.Tensor,
+      rhs: tf.Tensor,
+      train: bool = True,
+      **tf_einsum_kwargs
+  ) -> tf.Tensor:
+    """Generates a pure quantized einsum op.
+
+    Make sure that `apply` is called within the context of any updates
+    to statistics used for calibration you'd like to happen before the
+    op.
+
+    Args:
+      lhs: a float32 tensor for the left hand side
+      rhs: a float32 tensor for the right hand side
+      train: whether to generate the training or serving graph
+      **tf_einsum_kwargs: Keyword arguments to pass onto `einsum`.
+
+    Returns:
+      A tf.Tensor generated from possibly quantizing lhs and rhs
+      with clip bounds derived from the current quantizer statistics.
+    """
+
+    return einsum(
+        self.eq,
+        self.lhs_quantizer,
+        lhs,
+        self.rhs_quantizer,
+        rhs,
+        train,
+        **tf_einsum_kwargs)
+
+  def diagnostics(
+      self,
+      lhs: tf.Tensor,
+      rhs: tf.Tensor,
+  ) -> Dict[str, tf.Tensor]:
+    """Returns a dictionary from keys to diagnostic tensors.
+
+    Args:
+      lhs: lhs argument to self.Apply, used for deriving diangostics relative to
+        a given input.
+      rhs: as above, but for rhs
+
+    Returns:
+      A dictionary with various quantization-related diagnostics,
+      whose string keys are prefixed by self.name/self.{lhs,rhs}_name.
+    """
+    return aqt_ops_util.diagnostics(self, lhs, rhs)
```

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_einsum_test.py` & `aqtp-0.1.1/tensorflow/aqt_einsum_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,28 +88,25 @@
     rhs_config: aqt_config.AqtScheduleConfig,
     lhs_weights: Optional[tf.Tensor] = None,
     rhs_weights: Optional[tf.Tensor] = None,
     varscope_name: str = "einsum",
     train: bool = True,
     **einsum_kwargs) -> tf.Tensor:
   """Updates quantizers at event_count=0 and computes einsum."""
-  with tf.variable_scope(varscope_name):
-    lhs_tq = aqt_tensor.TensorQuantizer(
-        lhs.shape, lhs_config, name="lhs")
-    rhs_tq = aqt_tensor.TensorQuantizer(
-        rhs.shape, rhs_config, name="rhs")
+  aqtc = aqt_config.AqtEinsumConfig(
+      lhs=lhs_config, rhs=rhs_config)
+  einsum = aqt_einsum.Einsum(eq, aqtc, lhs.shape, rhs.shape, name=varscope_name)
 
   event_count = tf.constant(0, tf.int64)
   updates = [
-      lhs_tq.update(lhs, lhs_weights, event_count),
-      rhs_tq.update(rhs, rhs_weights, event_count)
+      einsum.update_lhs(lhs, lhs_weights, event_count),
+      einsum.update_rhs(rhs, rhs_weights, event_count)
   ]
   with tf.control_dependencies(updates):
-    return aqt_ops.aqt_einsum(eq, lhs_tq, lhs, rhs_tq, rhs, train,
-                              **einsum_kwargs)
+    return einsum.apply(lhs, rhs, train, **einsum_kwargs)
 
 
 def _generate_missing_shared_axes() -> Sequence[Dict[str, Any]]:
   """Cases where shared axes are missing."""
 
   keys = ["testcase_name", "eq", "lhs_share", "rhs_share"]
   cases: Sequence[Tuple[str, str, Sequence[int], Sequence[int]]] = [
```

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_matmul.py` & `aqtp-0.1.1/tensorflow/aqt_matmul.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 `aqt_ops`.
 """
 
 from typing import Callable, Dict, Iterable, Optional
 
 from aqt.common import aqt_config
 from aqt.common import aqt_config_utils
+from aqt.tensorflow import aqt_ops_util
 from aqt.tensorflow import aqt_tensor
 import tensorflow.compat.v1 as tf
 
 # TODO(b/220181240): Remove the pylint disable below and avoid using protected
 # methods.
 # We repeatedly use protected methods from classes defined in other modules to
 # avoid exporting them as part of the public API.
@@ -616,27 +617,8 @@
       rhs: as above, but for rhs
       grad: If specified, the gradient for deriving diagnostics.
 
     Returns:
       A dictionary with various quantization-related diagnostics,
       whose string keys are prefixed by self.name/self.{lhs,rhs}_name.
     """
-    d = {}
-    quantizers = [
-        (self.lhs_name, self.lhs_quantizer, lhs),
-        (self.rhs_name, self.rhs_quantizer, rhs),
-    ]
-    if grad is not None:
-      assert self.grad_quantizer is not None, (
-          'If grad is given, then grad_quantizer must be defined.')
-      quantizers.append((self.grad_name, self.grad_quantizer, grad))
-    for prefix, quantizer, argument in quantizers:
-      clipped_proportion = tf.cast(tf.abs(argument) > quantizer.clip_range(),
-                                   tf.float32)
-      prefix = f'{self.name}/{prefix}'
-      d[f'{prefix}/clipped_proportion'] = tf.math.reduce_mean(
-          clipped_proportion)
-      d[f'{prefix}/clip'] = quantizer.clip_range()
-      d[f'{prefix}/event_count'] = quantizer._last_update
-      for name, var in quantizer.calibration_variables().items():
-        d[f'{prefix}/{name}'] = var
-    return d
+    return aqt_ops_util.diagnostics(self, lhs, rhs, grad)
```

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_matmul_test.py` & `aqtp-0.1.1/tensorflow/aqt_matmul_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_ops.py` & `aqtp-0.1.1/tensorflow/aqt_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_tensor.py` & `aqtp-0.1.1/tensorflow/aqt_tensor.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/aqt/tensorflow/aqt_tensor_test.py` & `aqtp-0.1.1/tensorflow/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.1.0/setup.py` & `aqtp-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "tensorflow-datasets>=4.5.2",
     "dacite>=1.6.0",
     "ml_collections>=0.1.1",
 ]
 
 setup(
     name="aqtp",
-    version="0.1.0",
+    version="0.1.1",
     description="AQT: Accurate Quantized Training",
     long_description="\n\n".join([README]),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

