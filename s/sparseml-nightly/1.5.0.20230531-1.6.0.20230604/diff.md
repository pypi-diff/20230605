# Comparing `tmp/sparseml_nightly-1.5.0.20230531-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230604-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 946186 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-May-31 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-May-31 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-May-31 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-May-31 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-May-31 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-May-31 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-May-31 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-May-31 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-May-31 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-May-31 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-May-31 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-May-31 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-May-31 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-May-31 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-31 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-May-31 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-May-31 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-May-31 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-May-31 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-May-31 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-May-31 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-May-31 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-May-31 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-May-31 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-May-31 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-May-31 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-May-31 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-May-31 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-May-31 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-May-31 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-May-31 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-May-31 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-May-31 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-May-31 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-May-31 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-May-31 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-May-31 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-May-31 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-May-31 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-May-31 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-May-31 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-May-31 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-May-31 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-May-31 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-May-31 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-May-31 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-May-31 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-May-31 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      970 b- defN 23-May-31 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-May-31 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-May-31 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-May-31 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-May-31 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-May-31 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-May-31 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-May-31 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-May-31 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-May-31 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-May-31 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-May-31 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-May-31 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-May-31 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-May-31 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-May-31 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-May-31 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-May-31 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-May-31 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-May-31 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-May-31 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-May-31 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-May-31 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-May-31 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-May-31 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-May-31 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-May-31 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-May-31 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-May-31 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-May-31 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-May-31 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-May-31 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-May-31 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-May-31 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-May-31 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-May-31 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-May-31 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-May-31 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-May-31 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-May-31 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-May-31 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-May-31 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-May-31 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-May-31 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-May-31 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-May-31 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-May-31 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14532 b- defN 23-May-31 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-May-31 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-May-31 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-May-31 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-May-31 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-May-31 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-May-31 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-May-31 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-May-31 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-May-31 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-May-31 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-May-31 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-May-31 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-May-31 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-May-31 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-May-31 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-May-31 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-May-31 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-May-31 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-May-31 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-May-31 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-May-31 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-May-31 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-May-31 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-May-31 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-May-31 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-May-31 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-May-31 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10864 b- defN 23-May-31 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-May-31 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-May-31 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-May-31 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-May-31 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-May-31 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-May-31 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-May-31 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-May-31 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-May-31 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-May-31 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-May-31 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-May-31 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-May-31 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-May-31 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-May-31 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-May-31 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-31 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-May-31 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-May-31 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-May-31 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-May-31 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-May-31 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-May-31 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-May-31 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-May-31 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-May-31 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-May-31 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-May-31 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-May-31 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-May-31 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-May-31 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-May-31 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-May-31 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-May-31 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-May-31 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-31 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-May-31 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69997 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-May-31 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-May-31 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-May-31 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-May-31 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-May-31 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-May-31 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-May-31 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-May-31 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-May-31 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-May-31 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-May-31 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-May-31 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-May-31 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-May-31 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-May-31 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-May-31 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-31 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-May-31 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-May-31 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-May-31 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-May-31 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-May-31 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-May-31 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-May-31 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-May-31 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-May-31 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-May-31 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-May-31 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-May-31 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-May-31 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-May-31 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-May-31 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-May-31 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-May-31 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      987 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-May-31 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-May-31 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    20936 b- defN 23-May-31 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-May-31 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-May-31 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-May-31 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-May-31 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-May-31 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-May-31 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43756 b- defN 23-May-31 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-May-31 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-May-31 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-May-31 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-May-31 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-May-31 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-May-31 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-May-31 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-May-31 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-May-31 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-May-31 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-May-31 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-May-31 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-May-31 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-May-31 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-May-31 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-May-31 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-May-31 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-May-31 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-May-31 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-May-31 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-May-31 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-May-31 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-May-31 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-May-31 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-May-31 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-May-31 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-May-31 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-May-31 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-May-31 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-May-31 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-May-31 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-May-31 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    34331 b- defN 23-May-31 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-May-31 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-May-31 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-May-31 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-May-31 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-May-31 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21509 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2377 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36576 b- defN 23-May-31 01:33 sparseml_nightly-1.5.0.20230531.dist-info/RECORD
-368 files, 3425950 bytes uncompressed, 886978 bytes compressed:  74.1%
+Zip file size: 946552 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jun-04 01:31 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jun-04 01:31 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jun-04 01:31 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jun-04 01:31 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-04 01:31 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jun-04 01:31 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-Jun-04 01:31 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jun-04 01:31 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jun-04 01:31 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-04 01:31 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-04 01:31 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jun-04 01:31 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-04 01:31 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jun-04 01:31 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-04 01:31 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jun-04 01:31 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-Jun-04 01:31 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jun-04 01:31 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-04 01:31 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jun-04 01:31 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-Jun-04 01:31 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jun-04 01:31 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jun-04 01:31 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jun-04 01:31 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jun-04 01:31 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jun-04 01:31 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jun-04 01:31 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-04 01:31 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jun-04 01:31 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jun-04 01:31 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jun-04 01:31 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jun-04 01:31 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jun-04 01:31 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jun-04 01:31 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jun-04 01:31 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jun-04 01:31 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jun-04 01:31 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jun-04 01:31 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jun-04 01:31 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jun-04 01:31 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jun-04 01:31 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jun-04 01:31 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jun-04 01:31 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jun-04 01:31 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jun-04 01:31 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jun-04 01:31 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jun-04 01:31 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jun-04 01:31 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jun-04 01:31 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jun-04 01:31 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-04 01:31 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14532 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jun-04 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jun-04 01:31 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jun-04 01:31 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jun-04 01:31 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jun-04 01:31 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jun-04 01:31 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jun-04 01:31 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jun-04 01:31 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jun-04 01:31 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jun-04 01:31 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-Jun-04 01:31 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-Jun-04 01:31 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jun-04 01:31 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10864 b- defN 23-Jun-04 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jun-04 01:31 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jun-04 01:31 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jun-04 01:31 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jun-04 01:31 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jun-04 01:31 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jun-04 01:31 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jun-04 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jun-04 01:31 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69997 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jun-04 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jun-04 01:31 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jun-04 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jun-04 01:31 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jun-04 01:31 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jun-04 01:31 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jun-04 01:31 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jun-04 01:31 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jun-04 01:31 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jun-04 01:31 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jun-04 01:31 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jun-04 01:31 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jun-04 01:31 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jun-04 01:31 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jun-04 01:31 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jun-04 01:31 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    21274 b- defN 23-Jun-04 01:31 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jun-04 01:31 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-Jun-04 01:31 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jun-04 01:31 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jun-04 01:31 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43772 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jun-04 01:31 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17072 b- defN 23-Jun-04 01:31 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jun-04 01:31 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jun-04 01:31 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-Jun-04 01:31 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jun-04 01:31 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jun-04 01:31 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jun-04 01:31 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jun-04 01:31 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jun-04 01:31 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jun-04 01:31 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jun-04 01:31 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jun-04 01:31 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jun-04 01:31 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-04 01:31 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jun-04 01:31 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jun-04 01:31 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jun-04 01:31 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-04 01:31 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jun-04 01:31 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jun-04 01:31 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-04 01:31 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jun-04 01:31 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34788 b- defN 23-Jun-04 01:31 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jun-04 01:31 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jun-04 01:31 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jun-04 01:31 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-Jun-04 01:31 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jun-04 01:31 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21640 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2377 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36576 b- defN 23-Jun-04 01:33 sparseml_nightly-1.6.0.20230604.dist-info/RECORD
+368 files, 3426892 bytes uncompressed, 887344 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230531.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230604.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/version.py

```diff
@@ -15,15 +15,15 @@
 """
 Functionality for storing and setting the version info for SparseML
 """
 
 from datetime import date
 
 
-version_base = "1.5.0"
+version_base = "1.6.0"
 is_release = False  # change to True to set the generated version as a release version
 
 
 def _generate_version():
     return (
         version_base
         if is_release
```

## sparseml/transformers/export.py

```diff
@@ -71,18 +71,20 @@
 import collections
 import copy
 import inspect
 import logging
 import math
 import os
 import shutil
+from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Union
 
 from torch.nn import Module
 from transformers import AutoConfig, AutoTokenizer
+from transformers import TrainingArguments as HFTrainingArgs
 from transformers.tokenization_utils_base import PaddingStrategy
 
 from sparseml.optim import parse_recipe_variables
 from sparseml.pytorch.optim import ScheduledModifierManager
 from sparseml.pytorch.utils import export_onnx
 from sparseml.transformers.sparsification import Trainer
 from sparseml.transformers.utils import SparseAutoModel
@@ -103,14 +105,22 @@
 OPTIONAL_DEPLOYMENT_FILES.extend(EXTERNAL_ONNX_DATA_NAME)
 OPTIONAL_DEPLOYMENT_FILES.extend(OPT_TOKENIZER_FILES)
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
+@dataclass
+class DeviceCPUTrainingArgs(HFTrainingArgs):
+    @property
+    def place_model_on_device(self):
+        # Ensure model remains in CPU during ONNX export
+        return False
+
+
 def load_task_model(task: str, model_path: str, config: Any) -> Module:
     if task == "masked-language-modeling" or task == "mlm":
         return SparseAutoModel.masked_language_modeling_from_pretrained(
             model_name_or_path=model_path,
             config=config,
             model_type="model",
         )
@@ -290,23 +300,26 @@
             model=model,
             config=config,
         )
         eval_dataset = tokenized_dataset.get("validation")
         _LOGGER.info(f"loaded validation dataset for args {data_args}")
 
     model = model.train()
+
+    args = DeviceCPUTrainingArgs(output_dir="tmp_trainer")
     trainer = Trainer(
         model=model,
+        args=args,
         model_state_path=model_path,
         eval_dataset=eval_dataset,
         recipe=None,
         recipe_args=None,
         teacher=None,
     )
-    model = model.cpu()
+
     applied = trainer.apply_manager(epoch=math.inf, checkpoint=None)
 
     if not applied:
         _LOGGER.warning(
             f"No recipes were applied for {model_path}, "
             "check to make sure recipe(s) are stored in the model_path"
         )
```

## sparseml/transformers/sparsification/trainer.py

```diff
@@ -121,15 +121,15 @@
         training_args = kwargs.get("args")
         self.metadata = (
             self._extract_metadata(
                 metadata_args=metadata_args,
                 training_args_dict=training_args.to_dict(),
                 data_args_dict=asdict(data_args) if data_args else {},
             )
-            if training_args
+            if training_args and metadata_args
             else None
         )
 
         report_to = (
             ""
             if "args" not in kwargs
             or not kwargs["args"]
@@ -758,15 +758,14 @@
         )
 
     def _get_fake_dataloader(
         self,
         num_samples: int,
         tokenizer: "PreTrainedTokenizerBase",  # noqa: F821
     ):
-
         # Rearrange inputs' keys to match those defined by model foward func, which
         # seem to define how the order of inputs is determined in the exported model
         forward_args_spec = inspect.getfullargspec(self.model.__class__.forward)
         synthetic_input = self._get_fake_input(
             forward_func_input_keys=forward_args_spec.args,
             tokenizer=tokenizer,
         )
@@ -816,15 +815,14 @@
         model_state_path: str,
         recipe: Optional[str],
         recipe_args: Optional[Union[Dict[str, Any], str]] = None,
         metadata_args: Optional[List[str]] = None,
         teacher: Optional[Union[Module, str]] = None,
         **kwargs,
     ):
-
         super().__init__(
             model=model,
             model_state_path=model_state_path,
             recipe=recipe,
             recipe_args=recipe_args,
             metadata_args=metadata_args,
             teacher=teacher,
```

## sparseml/yolov8/trainers.py

```diff
@@ -16,14 +16,15 @@
 import shutil
 import subprocess
 import sys
 import tempfile
 import warnings
 from copy import copy, deepcopy
 from datetime import datetime, timedelta
+from functools import partial
 from pathlib import Path
 from typing import List, Optional
 
 import torch
 
 from sparseml.optim.helpers import load_recipe_yaml_str
 from sparseml.pytorch.optim.manager import ScheduledModifierManager
@@ -484,14 +485,20 @@
         if self.best_fitness == self.fitness:
             torch.save(ckpt, self.best)
         del ckpt
 
     def final_eval(self):
         # skip final eval if we are using a recipe
         if self.manager is None and self.checkpoint_manager is None:
+            # patch the validator, so it always has access to the
+            #  trainer object, which is needed to circumvent original ultralytics
+            #  call that ignores the trainer object
+            #  https://github.com/ultralytics/ultralytics/blob/
+            #  6c65934b555e64bf26edd699865754b5ff651d0c/ultralytics/yolo/engine/trainer.py#L551
+            self.validator = partial(self.validator, trainer=self)
             return super().final_eval()
 
     def callback_teardown(self):
         # NOTE: this callback is registered in __init__
         if self.manager is not None:
             self.manager.finalize()
```

## Comparing `sparseml_nightly-1.5.0.20230531.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230604.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230531.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230604.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.5.0.20230531
+Version: 1.6.0.20230604
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7.0,<3.11
 Description-Content-Type: text/markdown
-Requires-Dist: sparsezoo-nightly (~=1.5.0)
+Requires-Dist: sparsezoo-nightly (~=1.6.0)
 Requires-Dist: setuptools (<=59.5.0)
 Requires-Dist: jupyter (>=1.0.0)
 Requires-Dist: ipywidgets (>=7.0.0)
 Requires-Dist: pyyaml (>=5.0.0)
 Requires-Dist: progressbar2 (>=3.0.0)
 Requires-Dist: numpy (<=1.21.6,>=1.0.0)
 Requires-Dist: matplotlib (>=3.0.0)
@@ -37,24 +37,25 @@
 Requires-Dist: pandas (>=0.25.0)
 Requires-Dist: packaging (>=20.0)
 Requires-Dist: psutil (>=5.0.0)
 Requires-Dist: pydantic (>=1.5.0)
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: scikit-image (>=0.15.0)
 Requires-Dist: scikit-learn (>=0.24.2)
-Requires-Dist: scipy (>=1.0.0)
 Requires-Dist: tqdm (>=4.0.0)
 Requires-Dist: toposort (>=1.0)
 Requires-Dist: GPUtil (>=1.4.0)
 Requires-Dist: protobuf (<=3.20.1,>=3.12.2)
 Requires-Dist: click (!=8.0.0,>=7.1.2)
+Requires-Dist: scipy (<1.9.2,>=1.8) ; python_version <= "3.9"
+Requires-Dist: scipy (>=1.0.0) ; python_version > "3.9"
 Provides-Extra: deepsparse
-Requires-Dist: deepsparse-nightly (~=1.5.0) ; extra == 'deepsparse'
+Requires-Dist: deepsparse-nightly (~=1.6.0) ; extra == 'deepsparse'
 Provides-Extra: deepsparse-ent
-Requires-Dist: deepsparse-ent (~=1.5.0) ; extra == 'deepsparse-ent'
+Requires-Dist: deepsparse-ent (~=1.6.0) ; extra == 'deepsparse-ent'
 Provides-Extra: dev
 Requires-Dist: beautifulsoup4 (==4.9.3) ; extra == 'dev'
 Requires-Dist: black (==22.12.0) ; extra == 'dev'
 Requires-Dist: flake8 (==3.9.2) ; extra == 'dev'
 Requires-Dist: isort (==5.8.0) ; extra == 'dev'
 Requires-Dist: m2r2 (~=0.2.7) ; extra == 'dev'
 Requires-Dist: mistune (<3,>=2.0.3) ; extra == 'dev'
@@ -86,41 +87,42 @@
 Requires-Dist: tensorboard (<2.0.0) ; extra == 'tf_v1'
 Requires-Dist: tf2onnx (<1.6,>=1.0.0) ; extra == 'tf_v1'
 Provides-Extra: tf_v1_gpu
 Requires-Dist: tensorflow-gpu (<2.0.0) ; extra == 'tf_v1_gpu'
 Requires-Dist: tensorboard (<2.0.0) ; extra == 'tf_v1_gpu'
 Requires-Dist: tf2onnx (<1.6,>=1.0.0) ; extra == 'tf_v1_gpu'
 Provides-Extra: torch
-Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torch'
+Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'torch'
 Requires-Dist: gputils ; extra == 'torch'
 Provides-Extra: torch_all
-Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torch_all'
+Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'torch_all'
 Requires-Dist: gputils ; extra == 'torch_all'
 Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'torch_all'
 Requires-Dist: torchaudio (<=0.13) ; extra == 'torch_all'
 Provides-Extra: torchvision
-Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torchvision'
+Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'torchvision'
 Requires-Dist: gputils ; extra == 'torchvision'
 Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'torchvision'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'torchvision'
 Provides-Extra: transformers
-Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'transformers'
+Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'transformers'
 Requires-Dist: gputils ; extra == 'transformers'
-Requires-Dist: nm-transformers-nightly (~=1.5.0) ; extra == 'transformers'
+Requires-Dist: nm-transformers-nightly (~=1.6.0) ; extra == 'transformers'
 Requires-Dist: datasets (<=1.18.4) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
 Provides-Extra: ultralytics
 Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
+Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'ultralytics'
 Provides-Extra: yolov5
-Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'yolov5'
+Requires-Dist: torch (<1.14,>=1.7.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
 Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'yolov5'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'yolov5'
-Requires-Dist: nm-yolov5-nightly (~=1.5.0) ; extra == 'yolov5'
+Requires-Dist: nm-yolov5-nightly (~=1.6.0) ; extra == 'yolov5'
 
 <!--
 Copyright (c) 2021 - present / Neuralmagic, Inc. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
@@ -223,15 +225,15 @@
 - [Ultralytics YOLOv5](integrations/ultralytics-yolov5#tutorials)
 
 ## Installation
 
 This repository is tested on Python 3.7-3.10, and Linux/Debian systems.
 
 It is recommended to install in a [virtual environment](https://docs.python.org/3/library/venv.html) to keep your system in order.
-Currently supported ML Frameworks are the following: `torch>=1.1.0,<=1.12.1`, `tensorflow>=1.8.0,<2.0.0`, `tensorflow.keras >= 2.2.0`.
+Currently supported ML Frameworks are the following: `torch>=1.1.0,<1.14`, `tensorflow>=1.8.0,<2.0.0`, `tensorflow.keras >= 2.2.0`.
 
 Install with pip using:
 
 ```bash
 pip install sparseml
 ```
```

## Comparing `sparseml_nightly-1.5.0.20230531.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230604.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230531.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230531.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230604.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 sparseml/__init__.py,sha256=nxuiUykjTFTYiw28TB9H75wWbdzr6Y0j-2h4dabdp54,1413
 sparseml/analytics.py,sha256=WhXdKgK1-ll9sRzn2n8z-FAikQ02J8rUeWmceiX5S7E,898
 sparseml/base.py,sha256=oOPiaU2JhI0beFwp8Obe7hbt3kUuNvI5XD1wTBCtLnc,10284
 sparseml/log.py,sha256=K5E3goPRIPY7Uc14JcX-4oLXVWu7ecOPf1NYBGHc1r0,2483
-sparseml/version.py,sha256=jmrGrUNSNjL1K4iFHcD1xXttUBhm20Y6rTeTfP-tEvM,1511
+sparseml/version.py,sha256=IANtJ2lwLlKC1tGVdfq0LveVx77c3yZrd5RIhvbn8MM,1511
 sparseml/benchmark/__init__.py,sha256=WynUhMzXq3-iQAhPwcmcMOj2_xCa9brLubs7gxq9T3U,758
 sparseml/benchmark/info.py,sha256=yRA5QgKQNKjOZhQH9uNvVuWlqL4eXDVikA8pL5Mzha4,17631
 sparseml/benchmark/serialization.py,sha256=FPpcC93x5H86Fqil9YbERUpltu7qhhIQjsyYaSlW_20,10778
 sparseml/deepsparse/__init__.py,sha256=o5ITzTEOlH--61_SXMISrmPcRk4ci91FGlR-aQxwOn4,863
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
@@ -309,22 +309,22 @@
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
 sparseml/transformers/__init__.py,sha256=8J1vljjZiybTTdNXN9e9senxvZUmKXKHAB5-H4D_4nY,1511
-sparseml/transformers/export.py,sha256=Du_UBTeYtWMYY-NZIi8OtVWfY5fLkdze-ab50kesn2g,20936
+sparseml/transformers/export.py,sha256=SjYBxPPkuZAPEBqDeJNPZuDsmKAw_SzboUnAT1ClU64,21274
 sparseml/transformers/masked_language_modeling.py,sha256=xV1H7jyWCWMKTiow501cI498I5ouNC68nF7g-QNuzjw,30756
 sparseml/transformers/question_answering.py,sha256=E_Ljec9bNDrZ2KD3unTlbcRxEpyYU6C9asuEynhh4AQ,36557
 sparseml/transformers/text_classification.py,sha256=UYCpgSGTkmeGOeePQF5Idd8uY4GHQc-ShZK5SFOlP7E,40299
 sparseml/transformers/token_classification.py,sha256=6RUe1CmXQv7dHsE35aTg-xLW1g4BGakRp6pn0un2_mE,34350
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
-sparseml/transformers/sparsification/trainer.py,sha256=g2tP2s_W8Pmpef1CuCIsMD_teRkq9ZRIppR0Uq84Mpw,43756
+sparseml/transformers/sparsification/trainer.py,sha256=lylAxTy4WMmTqthB6ie4kUg1eIevSMIe11UcAO0WU9o,43772
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
 sparseml/transformers/utils/model.py,sha256=JRq-p0CqKlWLdbhD9e8V2YkFtSZ6xLE9B512TTR8d2M,17072
 sparseml/utils/__init__.py,sha256=-WKBN4DERhw7rTJkarilkyAM9pw4rW8qkXGRPSEJ8SM,844
 sparseml/utils/frameworks.py,sha256=S-cGkbVc6DoWfI6Hu5AkIqF0Vi1PyxKX5GfhwRfpv_E,886
@@ -349,20 +349,20 @@
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=9PORu1YtaIjWqKIXwMiWWqs3b_wrBt7oGNnNPgfq8Lw,34331
+sparseml/yolov8/trainers.py,sha256=mzOuog5BmQg3tER3m35zqTcKRlxiw9IqCpgBy-Ep1sA,34788
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.5.0.20230531.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.5.0.20230531.dist-info/METADATA,sha256=m_TNCMJzxiQ0EakHrV-kujMZzCOwe9zpDH7jI6MXklY,21509
-sparseml_nightly-1.5.0.20230531.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.5.0.20230531.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.5.0.20230531.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
-sparseml_nightly-1.5.0.20230531.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.5.0.20230531.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230604.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230604.dist-info/METADATA,sha256=2W7rnW2LXAXgS9oa8LHJikGqJzXhlwL_gUH3RQv2cT4,21640
+sparseml_nightly-1.6.0.20230604.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230604.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230604.dist-info/entry_points.txt,sha256=KbSvJr3uXYQgZRF0Mzi5B89ijSwsiZalXMxinJRaass,2377
+sparseml_nightly-1.6.0.20230604.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230604.dist-info/RECORD,,
```

