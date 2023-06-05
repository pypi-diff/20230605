# Comparing `tmp/torch_uncertainty-0.1.1.tar.gz` & `tmp/torch_uncertainty-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_uncertainty-0.1.1.tar", max compression
+gzip compressed data, was "torch_uncertainty-0.1.2.tar", max compression
```

## Comparing `torch_uncertainty-0.1.1.tar` & `torch_uncertainty-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11363 2023-05-17 14:21:25.756706 torch_uncertainty-0.1.1/LICENSE
--rw-r--r--   0        0        0     2996 2023-05-17 14:21:25.756706 torch_uncertainty-0.1.1/README.md
--rw-r--r--   0        0        0     2002 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3838 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/__init__.py
--rw-r--r--   0        0        0      212 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/__init__.py
--rw-r--r--   0        0        0       91 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/__init__.py
--rw-r--r--   0        0        0     6909 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/resnet.py
--rw-r--r--   0        0        0     6111 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/wideresnet.py
--rw-r--r--   0        0        0       89 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/__init__.py
--rw-r--r--   0        0        0     6564 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/resnet.py
--rw-r--r--   0        0        0     5443 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/masked/wideresnet.py
--rw-r--r--   0        0        0        0 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/mimo/__init__.py
--rw-r--r--   0        0        0       89 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/__init__.py
--rw-r--r--   0        0        0     7688 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/resnet.py
--rw-r--r--   0        0        0     5317 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/wideresnet.py
--rw-r--r--   0        0        0       77 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/standard/__init__.py
--rw-r--r--   0        0        0     4800 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/standard/resnet.py
--rw-r--r--   0        0        0     3891 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/baselines/standard/wideresnet.py
--rw-r--r--   0        0        0      221 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/__init__.py
--rw-r--r--   0        0        0     6647 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar10.py
--rw-r--r--   0        0        0     7007 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar100.py
--rw-r--r--   0        0        0     6404 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/imagenet.py
--rw-r--r--   0        0        0     4649 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/mnist.py
--rw-r--r--   0        0        0     4437 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datamodules/tiny_imagenet.py
--rw-r--r--   0        0        0      247 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/__init__.py
--rw-r--r--   0        0        0      771 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/aggregated_dataset.py
--rw-r--r--   0        0        0     4036 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/cifar_c.py
--rw-r--r--   0        0        0     2528 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/cifar_h.py
--rw-r--r--   0        0        0      559 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/imagenet_o.py
--rw-r--r--   0        0        0     1048 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/imagenet_r.py
--rw-r--r--   0        0        0      789 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/mixing_set.py
--rw-r--r--   0        0        0     5007 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/datasets/tiny_imagenet.py
--rw-r--r--   0        0        0      182 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/__init__.py
--rw-r--r--   0        0        0    15133 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/batchens_layers.py
--rw-r--r--   0        0        0     9725 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/masksembles_layers.py
--rw-r--r--   0        0        0     8318 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/layers/packed_layers.py
--rw-r--r--   0        0        0      340 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/__init__.py
--rw-r--r--   0        0        0     4042 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/brier_score.py
--rw-r--r--   0        0        0     3456 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/disagreement.py
--rw-r--r--   0        0        0     3098 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/entropy.py
--rw-r--r--   0        0        0     4060 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/fpr95.py
--rw-r--r--   0        0        0     3829 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/jensen_shannon_divergence.py
--rw-r--r--   0        0        0     3376 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/mutual_information.py
--rw-r--r--   0        0        0     3149 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/nll.py
--rw-r--r--   0        0        0     2656 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/metrics/variation_ratio.py
--rw-r--r--   0        0        0        0 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/__init__.py
--rw-r--r--   0        0        0      101 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/__init__.py
--rw-r--r--   0        0        0    11032 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/batched.py
--rw-r--r--   0        0        0    12641 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/masked.py
--rw-r--r--   0        0        0    13476 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/packed.py
--rw-r--r--   0        0        0    10540 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/std.py
--rw-r--r--   0        0        0      101 2023-05-17 14:21:25.760706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/__init__.py
--rw-r--r--   0        0        0     5704 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/batched.py
--rw-r--r--   0        0        0     6386 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/masked.py
--rw-r--r--   0        0        0     7010 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/packed.py
--rw-r--r--   0        0        0     5420 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/std.py
--rw-r--r--   0        0        0     4791 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/optimization_procedures.py
--rw-r--r--   0        0        0        0 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/routines/__init__.py
--rw-r--r--   0        0        0    10576 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/routines/classification.py
--rw-r--r--   0        0        0       42 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/transforms/__init__.py
--rw-r--r--   0        0        0      986 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/transforms/cutout.py
--rw-r--r--   0        0        0       77 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/utils/__init__.py
--rw-r--r--   0        0        0     1313 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/utils/checkpoints.py
--rw-r--r--   0        0        0      210 2023-05-17 14:21:25.764706 torch_uncertainty-0.1.1/torch_uncertainty/utils/hub.py
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.1/setup.py
--rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11363 2023-06-05 07:26:13.703778 torch_uncertainty-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3519 2023-06-05 07:26:13.703778 torch_uncertainty-0.1.2/README.md
+-rw-r--r--   0        0        0     2057 2023-06-05 07:26:13.707778 torch_uncertainty-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3159 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/__init__.py
+-rw-r--r--   0        0        0     7903 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/resnet.py
+-rw-r--r--   0        0        0     6918 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/wideresnet.py
+-rw-r--r--   0        0        0     1273 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/utils/parser_addons.py
+-rw-r--r--   0        0        0      221 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/__init__.py
+-rw-r--r--   0        0        0     6825 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar10.py
+-rw-r--r--   0        0        0     7037 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar100.py
+-rw-r--r--   0        0        0     7576 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/imagenet.py
+-rw-r--r--   0        0        0     4705 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/mnist.py
+-rw-r--r--   0        0        0     4752 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/tiny_imagenet.py
+-rw-r--r--   0        0        0      216 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/aggregated_dataset.py
+-rw-r--r--   0        0        0       89 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/__init__.py
+-rw-r--r--   0        0        0     7570 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_c.py
+-rw-r--r--   0        0        0     2700 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_h.py
+-rw-r--r--   0        0        0     1969 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/fractals.py
+-rw-r--r--   0        0        0      157 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/__init__.py
+-rw-r--r--   0        0        0     2446 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/base.py
+-rw-r--r--   0        0        0      313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/imagenet_a.py
+-rw-r--r--   0        0        0      313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/imagenet_o.py
+-rw-r--r--   0        0        0      313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/imagenet_r.py
+-rw-r--r--   0        0        0     5007 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/tiny_imagenet.py
+-rw-r--r--   0        0        0     1606 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet_r.py
+-rw-r--r--   0        0        0      182 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/__init__.py
+-rw-r--r--   0        0        0    15104 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/batchens_layers.py
+-rw-r--r--   0        0        0     9929 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/masksembles_layers.py
+-rw-r--r--   0        0        0     9048 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/packed_layers.py
+-rw-r--r--   0        0        0      340 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/__init__.py
+-rw-r--r--   0        0        0     4042 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/brier_score.py
+-rw-r--r--   0        0        0     3456 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/disagreement.py
+-rw-r--r--   0        0        0     3098 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/entropy.py
+-rw-r--r--   0        0        0     4060 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/fpr95.py
+-rw-r--r--   0        0        0     3829 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/jensen_shannon_divergence.py
+-rw-r--r--   0        0        0     3376 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/mutual_information.py
+-rw-r--r--   0        0        0     3149 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/nll.py
+-rw-r--r--   0        0        0     2656 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/variation_ratio.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/__init__.py
+-rw-r--r--   0        0        0      101 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/__init__.py
+-rw-r--r--   0        0        0    12044 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/batched.py
+-rw-r--r--   0        0        0    12641 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/masked.py
+-rw-r--r--   0        0        0    16040 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/packed.py
+-rw-r--r--   0        0        0    10540 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/std.py
+-rw-r--r--   0        0        0      101 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/__init__.py
+-rw-r--r--   0        0        0     6145 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/batched.py
+-rw-r--r--   0        0        0     6441 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/masked.py
+-rw-r--r--   0        0        0     7362 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/packed.py
+-rw-r--r--   0        0        0     5420 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/std.py
+-rw-r--r--   0        0        0     7527 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/optimization_procedures.py
+-rw-r--r--   0        0        0       65 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/post_processing/__init__.py
+-rw-r--r--   0        0        0     3426 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/post_processing/temperature_scaler.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/routines/__init__.py
+-rw-r--r--   0        0        0    14608 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/routines/classification.py
+-rw-r--r--   0        0        0      405 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/__init__.py
+-rw-r--r--   0        0        0     1255 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/cutout.py
+-rw-r--r--   0        0        0     4351 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/pixmix.py
+-rw-r--r--   0        0        0     6939 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/transforms.py
+-rw-r--r--   0        0        0       77 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/utils/__init__.py
+-rw-r--r--   0        0        0     1313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/utils/checkpoints.py
+-rw-r--r--   0        0        0      210 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/utils/hub.py
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.2/setup.py
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.2/PKG-INFO
```

### Comparing `torch_uncertainty-0.1.1/LICENSE` & `torch_uncertainty-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/pyproject.toml` & `torch_uncertainty-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch_uncertainty"
-version = "0.1.1"
+version = "0.1.2"
 description = "A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques."
 authors = [
     "ENSTA U2IS <olivier.laurent@ensta-paris.fr>",
     "Adrien Lafage <adrienlafage@outlook.com>",
     "Olivier Laurent <olivier.ar.laurent@gmail.com>",
 ]
 license = "Apache-2.0"
@@ -19,22 +19,23 @@
 einops = "^0.6.0"
 torchinfo = "^1.7.1"
 torchvision = "^0.14.1"
 timm = "^0.6.12"
 scipy = "^1.10.0"
 huggingface-hub = "^0.14.1"
 
-
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^0.991"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.0.4"
+pre-commit-hooks = "^4.4.0"
+cli-test-helpers = "^3.2.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.1.3"
 pytorch-sphinx-theme = {git = "https://github.com/torch-uncertainty/pytorch_sphinx_theme"}
 sphinx-copybutton = "^0.5.1"
 sphinx-gallery = "^0.12.2"
 matplotlib = "^3.7.1"
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/__init__.py` & `torch_uncertainty-0.1.2/torch_uncertainty/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 # fmt: off
 # flake8: noqa
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
-from typing import Callable, Type, Union
+from typing import Type, Union
 
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning.callbacks import LearningRateMonitor
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.callbacks.model_checkpoint import ModelCheckpoint
 from pytorch_lightning.loggers.tensorboard import TensorBoardLogger
-from torch.nn import Module
 from torchinfo import summary
 
 import numpy as np
 
-from .routines.classification import ClassificationSingle
 from .utils import get_version
 
+
 # fmt: on
+def init_args(
+    network: Type[pl.LightningModule], datamodule: Type[pl.LightningDataModule]
+) -> Namespace:
+    parser = ArgumentParser("torch-uncertainty")
+    parser.add_argument("--seed", type=int, default=None)
+    parser.add_argument("--test", type=int, default=None)
+    parser.add_argument("--summary", dest="summary", action="store_true")
+    parser.add_argument("--log_graph", dest="log_graph", action="store_true")
+    parser.add_argument(
+        "--channels_last",
+        action="store_true",
+        help="Use channels last memory format",
+    )
 
+    parser = pl.Trainer.add_argparse_args(parser)
+    parser = datamodule.add_argparse_args(parser)
+    parser = network.add_model_specific_args(parser)
+    args = parser.parse_args()
 
-def main(
-    network: Type[ClassificationSingle],
-    datamodule: Type[pl.LightningDataModule],
-    loss: Module,
-    optimization_procedure: Callable[[Module], dict],
+    return args
+
+
+def cls_main(
+    network: pl.LightningModule,
+    datamodule: pl.LightningDataModule,
     root: Union[Path, str],
     net_name: str,
     args: Namespace,
 ) -> None:
-    if args.seed:
-        pl.seed_everything(args.seed, workers=True)
-
     if isinstance(root, str):
         root = Path(root)
 
-    # datamodule
-    args.root = str(root / "data")
-    dm = datamodule(**vars(args))
-
-    # model
-    model = network(
-        loss=loss,
-        optimization_procedure=optimization_procedure,
-        num_classes=dm.num_classes,
-        in_channels=dm.num_channels,
-        **vars(args),
-    )
+    if args.max_epochs is None:
+        print(
+            "Setting max_epochs to 1 for testing purposes. Set max_epochs "
+            "manually to train the model."
+        )
+        args.max_epochs = 1
+
+    if isinstance(args.seed, int):
+        pl.seed_everything(args.seed)
 
     if args.channels_last:
-        model = model.to(memory_format=torch.channels_last)
+        network = network.to(memory_format=torch.channels_last)
 
     # logger
     tb_logger = TensorBoardLogger(
         str(root / "logs"),
         name=net_name,
         default_hp_metric=False,
         log_graph=args.log_graph,
@@ -71,67 +82,26 @@
 
     # Select the best model, monitor the lr and stop if NaN
     callbacks = [
         save_checkpoints,
         LearningRateMonitor(logging_interval="step"),
         EarlyStopping(monitor="hp/val_nll", patience=np.inf, check_finite=True),
     ]
-
     # trainer
     trainer = pl.Trainer.from_argparse_args(
         args,
         callbacks=callbacks,
         logger=tb_logger,
         deterministic=(args.seed is not None),
     )
 
     if args.summary:
-        summary(model, input_size=model.example_input_array.shape)
+        summary(network, input_size=list(datamodule.input_shape).insert(0, 1))
     elif args.test is not None:
         ckpt_file, _ = get_version(
             root=(root / "logs" / net_name), version=args.test
         )
-        trainer.test(model, datamodule=dm, ckpt_path=str(ckpt_file))
+        trainer.test(network, datamodule=datamodule, ckpt_path=str(ckpt_file))
     else:
         # training and testing
-        trainer.fit(model, dm)
-        trainer.test(datamodule=dm, ckpt_path="best")
-
-
-def cli_main(
-    network: Type[ClassificationSingle],
-    datamodule: Type[pl.LightningDataModule],
-    loss: Module,
-    optimization_procedure: Callable[[Module], dict],
-    root: Union[Path, str],
-    net_name: str,
-) -> None:
-    parser = ArgumentParser("torch-uncertainty")
-    parser.add_argument(
-        "--seed",
-        type=int,
-        default=None,
-        help="Set the random seed to some value for reproducibility",
-    )
-    parser.add_argument(
-        "--test",
-        type=int,
-        default=None,
-        help="Test a specific version of the model. The checkpoint must be available in the logs folder.",
-    )
-    parser.add_argument(
-        "--summary", action="store_true", help="Print a summary of the model"
-    )
-    parser.add_argument("--log_graph", action="store_true")
-    parser.add_argument(
-        "--channels_last",
-        action="store_true",
-        help="Use channels last memory format",
-    )
-
-    parser = pl.Trainer.add_argparse_args(parser)
-    parser = datamodule.add_argparse_args(parser)
-    parser = network.add_model_specific_args(parser)
-    args = parser.parse_args()
-    main(
-        network, datamodule, loss, optimization_procedure, root, net_name, args
-    )
+        trainer.fit(network, datamodule)
+        trainer.test(datamodule=datamodule, ckpt_path="best")
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/baselines/batched/resnet.py` & `torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/resnet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,197 +1,232 @@
 # fmt: off
 from argparse import ArgumentParser, BooleanOptionalAction
-from typing import Any, Dict, Literal
+from typing import Any, Literal, Optional
 
-import torch
 import torch.nn as nn
-from torch import optim
+from pytorch_lightning import LightningModule
 
-from torch_uncertainty.models.resnet import (
+from ...models.resnet import (
     batched_resnet18,
     batched_resnet34,
     batched_resnet50,
     batched_resnet101,
     batched_resnet152,
+    masked_resnet18,
+    masked_resnet34,
+    masked_resnet50,
+    masked_resnet101,
+    masked_resnet152,
+    packed_resnet18,
+    packed_resnet34,
+    packed_resnet50,
+    packed_resnet101,
+    packed_resnet152,
+    resnet18,
+    resnet34,
+    resnet50,
+    resnet101,
+    resnet152,
+)
+from ...routines.classification import (
+    ClassificationEnsemble,
+    ClassificationSingle,
+)
+from ..utils.parser_addons import (
+    add_masked_specific_args,
+    add_packed_specific_args,
+    add_resnet_specific_args,
 )
-from torch_uncertainty.routines.classification import ClassificationEnsemble
-
-# fmt: on
-archs = [
-    batched_resnet18,
-    batched_resnet34,
-    batched_resnet50,
-    batched_resnet101,
-    batched_resnet152,
-]
-choices = [18, 34, 50, 101, 152]
 
 
-class BatchedResNet(ClassificationEnsemble):
-    r"""LightningModule for BatchEnsembles ResNet.
+# fmt: on
+class ResNet:
+    r"""ResNet backbone baseline for classification providing support for
+    various versions and architectures.
 
     Args:
         num_classes (int): Number of classes to predict.
-        num_estimators (int): Number of estimators in the ensemble.
         in_channels (int): Number of input channels.
+        loss (nn.Module): Training loss.
+        optimization_procedure (Any): Optimization procedure, corresponds to
+            what expect the `LightningModule.configure_optimizers()
+            <https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#configure-optimizers>`_
+            method.
+        version (str):
+            Determines which ResNet version to use:
+
+            - ``"vanilla"``: original ResNet
+            - ``"packed"``: Packed-Ensembles ResNet
+            - ``"batched"``: BatchEnsemble ResNet
+            - ``"masked"``: Masksemble ResNet
+
         arch (int):
             Determines which ResNet architecture to use:
 
             - ``18``: ResNet-18
             - ``32``: ResNet-32
             - ``50``: ResNet-50
             - ``101``: ResNet-101
             - ``152``: ResNet-152
 
-        loss (torch.nn.Module): Training loss.
-        optimization_procedure (Any): Optimization procedure, corresponds to
-            what expect the `LightningModule.configure_optimizers()
-            <https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#configure-optimizers>`_
-            method.
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
+        num_estimators (int, optional): Number of estimators in the ensemble.
+            Only used if :attr:`version` is either ``"packed"``, ``"batched"``
+            or ``"masked"`` Defaults to ``None``.
+        groups (int, optional): Number of groups in convolutions. Defaults to
+            ``1``.
+        scale (float, optional): Expansion factor affecting the width of the
+            estimators. Only used if :attr:`version` is ``"masked"``. Defaults
+            to ``None``.
+        alpha (float, optional): Expansion factor affecting the width of the
+            estimators. Only used if :attr:`version` is ``"packed"``. Defaults
+            to ``None``.
+        gamma (int, optional): Number of groups within each estimator. Only
+            used if :attr:`version` is ``"packed"`` and scales with
+            :attr:`groups`. Defaults to ``1s``.
         use_entropy (bool, optional): Indicates whether to use the entropy
             values as the OOD criterion or not. Defaults to ``False``.
         use_logits (bool, optional): Indicates whether to use the logits as the
             OOD criterion or not. Defaults to ``False``.
         use_mi (bool, optional): Indicates whether to use the mutual
             information as the OOD criterion or not. Defaults to ``False``.
         use_variation_ratio (bool, optional): Indicates whether to use the
             variation ratio as the OOD criterion or not. Defaults to ``False``.
+        pretrained (bool, optional): Indicates whether to use the pretrained
+            weights or not. Only used if :attr:`version` is ``"packed"``.
+            Defaults to ``False``.
+
+    Raises:
+        ValueError: If :attr:`version` is not either ``"vanilla"``,
+            ``"packed"``, ``"batched"`` or ``"masked"``.
 
-    Note:
-        The OOD criterion is by defaults the confidence score.
-
-    Warning:
-        Make sure at most only one of :attr:`use_entropy`, :attr:`use_logits`,
-        :attr:`use_mi` and :attr:`use_variation_ratio` attributes is set to
-        ``True``. Otherwise a :class:`ValueError()` will be raised.
+    Returns:
+        LightningModule: ResNet baseline ready for training and evaluation.
     """
 
-    def __init__(
-        self,
+    single = ["vanilla"]
+    ensemble = ["packed", "batched", "masked"]
+    versions = {
+        "vanilla": [resnet18, resnet34, resnet50, resnet101, resnet152],
+        "packed": [
+            packed_resnet18,
+            packed_resnet34,
+            packed_resnet50,
+            packed_resnet101,
+            packed_resnet152,
+        ],
+        "batched": [
+            batched_resnet18,
+            batched_resnet34,
+            batched_resnet50,
+            batched_resnet101,
+            batched_resnet152,
+        ],
+        "masked": [
+            masked_resnet18,
+            masked_resnet34,
+            masked_resnet50,
+            masked_resnet101,
+            masked_resnet152,
+        ],
+    }
+    archs = [18, 34, 50, 101, 152]
+
+    def __new__(
+        cls,
         num_classes: int,
-        num_estimators: int,
         in_channels: int,
-        arch: Literal[18, 34, 50, 101, 152],
         loss: nn.Module,
         optimization_procedure: Any,
+        version: Literal["vanilla", "packed", "batched", "masked"],
+        arch: int,
+        imagenet_structure: bool = True,
+        num_estimators: Optional[int] = None,
+        groups: Optional[int] = 1,
+        scale: Optional[float] = None,
+        alpha: Optional[float] = None,
+        gamma: Optional[int] = 1,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
-        imagenet_structure: bool = True,
-        **kwargs: Dict[str, Any],
-    ) -> None:
-        super().__init__(
-            num_classes=num_classes,
-            num_estimators=num_estimators,
-            use_entropy=use_entropy,
-            use_logits=use_logits,
-            use_mi=use_mi,
-            use_variation_ratio=use_variation_ratio,
-        )
-
-        # construct config
-        self.save_hyperparameters(ignore=["loss", "optimization_procedure"])
-
-        self.loss = loss
-        self.optimization_procedure = optimization_procedure
-
-        self.model = archs[choices.index(arch)](
-            in_channels=in_channels,
-            num_estimators=num_estimators,
-            num_classes=num_classes,
-            imagenet_structure=imagenet_structure,
-        )
-
-        # to log the graph
-        self.example_input_array = torch.randn(1, in_channels, 32, 32)
+        pretrained: bool = False,
+        **kwargs,
+    ) -> LightningModule:
+        params = {
+            "in_channels": in_channels,
+            "num_classes": num_classes,
+            "imagenet_structure": imagenet_structure,
+            "groups": groups,
+        }
+
+        if version not in cls.versions.keys():
+            raise ValueError(f"Unknown version: {version}")
+
+        if version == "packed":
+            params.update(
+                {
+                    "num_estimators": num_estimators,
+                    "alpha": alpha,
+                    "gamma": gamma,
+                    "pretrained": pretrained,
+                }
+            )
+        elif version == "batched":
+            params.update(
+                {
+                    "num_estimators": num_estimators,
+                }
+            )
+        elif version == "masked":
+            params.update(
+                {
+                    "num_estimators": num_estimators,
+                    "scale": scale,
+                }
+            )
 
-    def configure_optimizers(self) -> dict:
-        param_optimizer = self.optimization_procedure(self)["optimizer"]
-        weight_decay = param_optimizer.defaults["weight_decay"]
-        lr = param_optimizer.defaults["lr"]
-        momentum = param_optimizer.defaults["momentum"]
-        my_list = ["R", "S"]
-        params_multi_tmp = list(
-            filter(
-                lambda kv: (my_list[0] in kv[0]) or (my_list[1] in kv[0]),
-                self.named_parameters(),
+        model = cls.versions[version][cls.archs.index(arch)](**params)
+        kwargs.update(params)
+        # routine specific parameters
+        if version in cls.single:
+            return ClassificationSingle(
+                model=model,
+                loss=loss,
+                optimization_procedure=optimization_procedure,
+                use_entropy=use_entropy,
+                use_logits=use_logits,
+                **kwargs,
             )
-        )
-        param_core_tmp = list(
-            filter(
-                lambda kv: (my_list[0] not in kv[0])
-                and (my_list[1] not in kv[0]),
-                self.named_parameters(),
+        elif version in cls.ensemble:
+            return ClassificationEnsemble(
+                model=model,
+                loss=loss,
+                optimization_procedure=optimization_procedure,
+                use_entropy=use_entropy,
+                use_logits=use_logits,
+                use_mi=use_mi,
+                use_variation_ratio=use_variation_ratio,
+                **kwargs,
             )
-        )
-        params_multi = [param for _, param in params_multi_tmp]
-        param_core = [param for _, param in param_core_tmp]
-        optimizer = optim.SGD(
-            [
-                {"params": param_core, "weight_decay": weight_decay},
-                {"params": params_multi, "weight_decay": 0.0},
-            ],
-            lr=lr,
-            momentum=momentum,
-        )
-        scheduler = self.optimization_procedure(self)["lr_scheduler"]
-        scheduler.optimizer = optimizer
-        return {"optimizer": optimizer, "lr_scheduler": scheduler}
-
-    @property
-    def criterion(self) -> nn.Module:
-        return self.loss()
-
-    def forward(self, input: torch.Tensor) -> torch.Tensor:  # type: ignore
-        input = input.repeat(self.num_estimators, 1, 1, 1)
-        return self.model.forward(input)
-
-    @staticmethod
-    def add_model_specific_args(
-        parent_parser: ArgumentParser,
-    ) -> ArgumentParser:
-        """Defines the model's attributes via command-line options:
-
-        - ``--arch [int]``: defines :attr:`arch`. Defaults to ``18``.
-        - ``--num_estimators [int]``: defines :attr:`num_estimators`. Defaults
-          to ``1``.
-        - ``--imagenet_structure``: sets :attr:`imagenet_structure`. Defaults
-          to ``True``.
-        - ``--entropy``: sets :attr:`use_entropy` to ``True``.
-        - ``--logits``: sets :attr:`use_logits` to ``True``.
-        - ``--mutual_information``: sets :attr:`use_mi` to ``True``.
-        - ``--variation_ratio``: sets :attr:`use_variation_ratio` to ``True``.
-
-        Example:
-
-            .. parsed-literal::
-
-                python script.py --arch 18 --num_estimators 4 --alpha 2
-        """
-        parent_parser.add_argument(
-            "--arch",
-            type=int,
-            default=18,
-            choices=choices,
-            help="Type of ResNet",
-        )
-        parent_parser.add_argument(
-            "--imagenet_structure",
+
+    @classmethod
+    def add_model_specific_args(cls, parser: ArgumentParser) -> ArgumentParser:
+        parser = ClassificationEnsemble.add_model_specific_args(parser)
+        parser = add_resnet_specific_args(parser)
+        parser = add_packed_specific_args(parser)
+        parser = add_masked_specific_args(parser)
+        parser.add_argument(
+            "--version",
+            type=str,
+            choices=cls.versions.keys(),
+            default="vanilla",
+            help=f"Variation of ResNet. Choose among: {cls.versions.keys()}",
+        )
+        parser.add_argument(
+            "--pretrained",
+            dest="pretrained",
             action=BooleanOptionalAction,
-            default=True,
-            help="Use imagenet structure",
-        )
-        parent_parser.add_argument("--num_estimators", type=int, default=4)
-        parent_parser.add_argument(
-            "--entropy", dest="use_entropy", action="store_true"
-        )
-        parent_parser.add_argument(
-            "--logits", dest="use_logits", action="store_true"
-        )
-        parent_parser.add_argument(
-            "--mutual_information", dest="use_mi", action="store_true"
-        )
-        parent_parser.add_argument(
-            "--variation_ratio", dest="use_variation_ratio", action="store_true"
+            default=False,
         )
-        return parent_parser
+        return parser
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/baselines/packed/wideresnet.py` & `torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/wideresnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,189 @@
 # fmt: off
 from argparse import ArgumentParser, BooleanOptionalAction
-from typing import Any, Dict
+from typing import Any, Literal, Optional
 
-import torch
 import torch.nn as nn
+from pytorch_lightning import LightningModule
 
-from torch_uncertainty.models.wideresnet.packed import packed_wideresnet28x10
-from torch_uncertainty.routines.classification import ClassificationEnsemble
-
-# fmt: on
+from ...models.wideresnet import (
+    batched_wideresnet28x10,
+    masked_wideresnet28x10,
+    packed_wideresnet28x10,
+    wideresnet28x10,
+)
+from ...routines.classification import (
+    ClassificationEnsemble,
+    ClassificationSingle,
+)
+from ..utils.parser_addons import (
+    add_masked_specific_args,
+    add_packed_specific_args,
+    add_wideresnet_specific_args,
+)
 
 
-class PackedWideResNet(ClassificationEnsemble):
-    r"""LightningModule for Packed-Ensembles WideResNet.
+# fmt: on
+class WideResNet:
+    r"""Wide-ResNet28x10 backbone baseline for classification providing support
+    for various versions.
 
     Args:
         num_classes (int): Number of classes to predict.
-        num_estimators (int): Number of estimators in the ensemble.
         in_channels (int): Number of input channels.
-        alpha (int): Expansion factor affecting the width of the estimators.
-        gamma (int): Number of groups within each estimator.
-        loss (torch.nn.Module): Training loss.
+        loss (nn.Module): Training loss.
         optimization_procedure (Any): Optimization procedure, corresponds to
             what expect the `LightningModule.configure_optimizers()
             <https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#configure-optimizers>`_
             method.
+        version (str):
+            Determines which Wide-ResNet version to use:
+
+            - ``"vanilla"``: original Wide-ResNet
+            - ``"packed"``: Packed-Ensembles Wide-ResNet
+            - ``"batched"``: BatchEnsemble Wide-ResNet
+            - ``"masked"``: Masksemble Wide-ResNet
+
+        imagenet_structure (bool, optional): Whether to use the ImageNet
+            structure. Defaults to ``True``.
+        num_estimators (int, optional): Number of estimators in the ensemble.
+            Only used if :attr:`version` is either ``"packed"``, ``"batched"``
+            or ``"masked"`` Defaults to ``None``.
+        groups (int, optional): Number of groups in convolutions. Defaults to
+            ``1``.
+        scale (float, optional): Expansion factor affecting the width of the
+            estimators. Only used if :attr:`version` is ``"masked"``. Defaults
+            to ``None``.
+        alpha (float, optional): Expansion factor affecting the width of the
+            estimators. Only used if :attr:`version` is ``"packed"``. Defaults
+            to ``None``.
+        gamma (int, optional): Number of groups within each estimator. Only
+            used if :attr:`version` is ``"packed"`` and scales with
+            :attr:`groups`. Defaults to ``1s``.
         use_entropy (bool, optional): Indicates whether to use the entropy
             values as the OOD criterion or not. Defaults to ``False``.
         use_logits (bool, optional): Indicates whether to use the logits as the
             OOD criterion or not. Defaults to ``False``.
         use_mi (bool, optional): Indicates whether to use the mutual
             information as the OOD criterion or not. Defaults to ``False``.
         use_variation_ratio (bool, optional): Indicates whether to use the
             variation ratio as the OOD criterion or not. Defaults to ``False``.
-
-    Note:
-        The OOD criterion is by defaults the confidence score.
-
-    Warning:
-        Make sure at most only one of :attr:`use_entropy`, :attr:`use_logits`,
-        :attr:`use_mi` and :attr:`use_variation_ratio` attributes is set to
-        ``True``. Otherwise a :class:`ValueError()` will be raised.
+        pretrained (bool, optional): Indicates whether to use the pretrained
+            weights or not. Only used if :attr:`version` is ``"packed"``.
+            Defaults to ``False``.
+
+    Raises:
+        ValueError: If :attr:`version` is not either ``"vanilla"``,
+            ``"packed"``, ``"batched"`` or ``"masked"``.
+
+    Returns:
+        LightningModule: Wide-ResNet baseline ready for training and
+            evaluation.
     """
+    single = ["vanilla"]
+    ensemble = ["packed", "batched", "masked"]
+    versions = {
+        "vanilla": [wideresnet28x10],
+        "packed": [packed_wideresnet28x10],
+        "batched": [batched_wideresnet28x10],
+        "masked": [masked_wideresnet28x10],
+    }
 
-    def __init__(
-        self,
+    def __new__(
+        cls,
         num_classes: int,
-        num_estimators: int,
         in_channels: int,
-        alpha: int,
-        gamma: int,
         loss: nn.Module,
         optimization_procedure: Any,
+        version: Literal["vanilla", "packed", "batched", "masked"],
+        imagenet_structure: bool = True,
+        num_estimators: Optional[int] = None,
+        groups: Optional[int] = None,
+        scale: Optional[float] = None,
+        alpha: Optional[int] = None,
+        gamma: Optional[int] = None,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
-        imagenet_structure: bool = True,
-        **kwargs: Dict[str, Any],
-    ) -> None:
-        super().__init__(
-            num_classes=num_classes,
-            num_estimators=num_estimators,
-            use_entropy=use_entropy,
-            use_logits=use_logits,
-            use_mi=use_mi,
-            use_variation_ratio=use_variation_ratio,
-        )
-
-        # construct config
-        self.save_hyperparameters(ignore=["loss", "optimization_procedure"])
-
-        self.loss = loss
-        self.optimization_procedure = optimization_procedure
-
-        self.model = packed_wideresnet28x10(
-            in_channels=in_channels,
-            num_estimators=num_estimators,
-            num_classes=num_classes,
-            alpha=alpha,
-            gamma=gamma,
-            imagenet_structure=imagenet_structure,
-        )
-
-        # to log the graph
-        self.example_input_array = torch.randn(1, in_channels, 32, 32)
-
-    def configure_optimizers(self) -> dict:
-        """Configures the optimizers.
-
-        Returns:
-            dict: Optimizers.
-        """
-        return self.optimization_procedure(self)
-
-    @property
-    def criterion(self) -> nn.Module:
-        return self.loss()
-
-    def forward(self, input: torch.Tensor) -> torch.Tensor:  # type: ignore
-        return self.model.forward(input)
-
-    @staticmethod
-    def add_model_specific_args(
-        parent_parser: ArgumentParser,
-    ) -> ArgumentParser:
-        """Defines the model's attributes via command-line options:
-
-        - ``--num_estimators [int]``: defines :attr:`num_estimators`. Defaults
-          to ``1``.
-        - ``--imagenet_structure``: sets :attr:`imagenet_structure`. Defaults
-          to ``True``.
-        - ``--entropy``: sets :attr:`use_entropy` to ``True``.
-        - ``--logits``: sets :attr:`use_logits` to ``True``.
-        - ``--mutual_information``: sets :attr:`use_mi` to ``True``.
-        - ``--variation_ratio``: sets :attr:`use_variation_ratio` to ``True``.
-
-        Example:
-
-            .. parsed-literal::
-
-                python script.py --num_estimators 4 --alpha 2
-        """
-        parent_parser.add_argument("--num_estimators", type=int, default=4)
-        parent_parser.add_argument(
-            "--imagenet_structure",
+        # pretrained: bool = False,
+        **kwargs,
+    ) -> LightningModule:
+        params = {
+            "in_channels": in_channels,
+            "num_classes": num_classes,
+            "imagenet_structure": imagenet_structure,
+            "groups": groups,
+        }
+
+        if version not in cls.versions.keys():
+            raise ValueError(f"Unknown version: {version}")
+
+        # version specific params
+        if version == "packed":
+            params.update(
+                {
+                    "num_estimators": num_estimators,
+                    "alpha": alpha,
+                    "gamma": gamma,
+                }
+            )
+        elif version == "batched":
+            params.update(
+                {
+                    "num_estimators": num_estimators,
+                }
+            )
+        elif version == "masked":
+            params.update(
+                {
+                    "num_estimators": num_estimators,
+                    "scale": scale,
+                }
+            )
+
+        model = cls.versions[version][0](**params)
+        kwargs.update(params)
+        # routine specific parameters
+        if version in cls.single:
+            return ClassificationSingle(
+                model=model,
+                loss=loss,
+                optimization_procedure=optimization_procedure,
+                use_entropy=use_entropy,
+                use_logits=use_logits,
+                **kwargs,
+            )
+        elif version in cls.ensemble:
+            return ClassificationEnsemble(
+                model=model,
+                loss=loss,
+                optimization_procedure=optimization_procedure,
+                use_entropy=use_entropy,
+                use_logits=use_logits,
+                use_mi=use_mi,
+                use_variation_ratio=use_variation_ratio,
+                **kwargs,
+            )
+
+    @classmethod
+    def add_model_specific_args(cls, parser: ArgumentParser) -> ArgumentParser:
+        parser = ClassificationEnsemble.add_model_specific_args(parser)
+        parser = add_wideresnet_specific_args(parser)
+        parser = add_packed_specific_args(parser)
+        parser = add_masked_specific_args(parser)
+        parser.add_argument(
+            "--version",
+            type=str,
+            choices=cls.versions.keys(),
+            default="vanilla",
+            help="Variation of WideResNet. "
+            + f"Choose among: {cls.versions.keys()}",
+        )
+        parser.add_argument(
+            "--pretrained",
+            dest="pretrained",
             action=BooleanOptionalAction,
-            default=True,
-            help="Use imagenet structure",
+            default=False,
         )
-        parent_parser.add_argument(
-            "--entropy", dest="use_entropy", action="store_true"
-        )
-        parent_parser.add_argument(
-            "--logits", dest="use_logits", action="store_true"
-        )
-        parent_parser.add_argument(
-            "--mutual_information", dest="use_mi", action="store_true"
-        )
-        parent_parser.add_argument(
-            "--variation_ratio", dest="use_variation_ratio", action="store_true"
-        )
-        parent_parser.add_argument("--alpha", type=int, default=2)
-        parent_parser.add_argument("--gamma", type=int, default=1)
-        return parent_parser
+
+        return parser
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar10.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar10.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ..transforms import Cutout
 
 
 # fmt: on
 class CIFAR10DataModule(LightningDataModule):
     num_classes = 10
     num_channels = 3
+    input_shape = (3, 32, 32)
 
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
@@ -85,21 +86,27 @@
                     (0.4914, 0.4822, 0.4465),
                     (0.2023, 0.1994, 0.2010),
                 ),
             ]
         )
 
     def prepare_data(self) -> None:
-        if self.test_alt != "c":
+        if self.test_alt is None:
             self.dataset(self.root, train=True, download=True)
             self.dataset(self.root, train=False, download=True)
-        else:
+        elif self.test_alt == "c":
             self.dataset(
                 self.root,
                 severity=self.corruption_severity,
+                download=True,
+            )
+        else:
+            self.dataset(
+                self.root,
+                download=True,
             )
 
         self.ood_dataset(self.root, split="test", download=True)
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
             assert self.test_alt != "c", "CIFAR-C can only be used in testing."
@@ -115,15 +122,15 @@
             if self.val_split == 0:
                 self.val = self.dataset(
                     self.root,
                     train=False,
                     download=False,
                     transform=self.transform_test,
                 )
-        elif stage == "test" or stage is None:
+        elif stage == "test":
             self.test = self.dataset(
                 self.root,
                 train=False,
                 download=False,
                 transform=self.transform_test,
             )
             self.ood = self.ood_dataset(
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/cifar100.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar100.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from ..transforms import Cutout
 
 
 # fmt: on
 class CIFAR100DataModule(LightningDataModule):
     num_classes = 100
     num_channels = 3
+    input_shape = (3, 32, 32)
 
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/imagenet.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/imagenet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,97 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
+import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
 from torch.utils.data import DataLoader, Dataset
 from torchvision.datasets import DTD, SVHN, ImageNet, INaturalist
 
-from ..datasets import ImageNetO, ImageNetR
+from ..datasets import ImageNetA, ImageNetO, ImageNetR
 
 
 # fmt: on
 class ImageNetDataModule(LightningDataModule):
+    num_classes = 1000
+    num_channels = 3
+    test_datasets = ["r", "o", "a"]
+    ood_datasets = ["inaturalist", "imagenet-o", "svhn", "textures"]
+
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
-        val_split: int = 0,
+        ood_ds: str = "svhn",
+        test_alt: str = None,
+        procedure: str = "A3",
+        train_size: int = 224,
+        rand_augment_opt: str = None,
         num_workers: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
-        ood_name: str = "svhn",
-        test_option: str = None,
-        # num_ops: int = 2,
-        # magnitude: float = 15,
-        procedure: str = "A3",
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
         self.batch_size = batch_size
-        self.val_split = val_split
         self.num_workers = num_workers
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
-        self.ood_name = ood_name
-        self.num_classes = 1000
-        self.num_channels = 3
+        self.ood_ds = ood_ds
+        self.test_alt = test_alt
 
-        if test_option is None:
+        if test_alt is None:
             self.dataset = ImageNet
-        elif test_option == "imagenet-r":
+        elif test_alt == "r":
             self.dataset = ImageNetR
-        else:
-            raise ValueError(f"Error, {test_option} not taken in charge.")
+        elif test_alt == "o":
+            self.dataset = ImageNetO
+        elif test_alt == "a":
+            self.dataset = ImageNetA
 
-        if ood_name == "inaturalist":
+        if ood_ds == "inaturalist":
             self.ood_dataset = INaturalist
-        elif ood_name == "imagenet-o":
+        elif ood_ds == "imagenet-o":
             self.ood_dataset = ImageNetO
-        elif ood_name == "svhn":
+        elif ood_ds == "svhn":
             self.ood_dataset = SVHN
-        elif ood_name == "textures":
+        elif ood_ds == "textures":
             self.ood_dataset = DTD
         else:
-            raise ValueError(f"The dataset {ood_name} is not supported.")
+            raise ValueError(f"The dataset {ood_ds} is not supported.")
 
         self.procedure = procedure
 
-        if self.procedure == "Classic":
-            print("Classic Procedure")
-            train_size = 224
+        if self.procedure is None:
+            print("Custom Procedure")
+            train_size = train_size
+            if rand_augment_opt is not None:
+                main_transform = rand_augment_transform(rand_augment_opt, {})
+            else:
+                main_transform = nn.Identity()
         elif self.procedure == "A3":
             print("Procedure A3")
             train_size = 160
+            main_transform = rand_augment_transform("rand-m6-mstd0.5-inc1", {})
         else:
             raise ValueError("The procedure is unknown")
 
         self.transform_train = T.Compose(
             [
                 T.RandomResizedCrop(train_size),
                 T.RandomHorizontalFlip(),
-                rand_augment_transform("rand-m6-mstd0.5-inc1", {}),
+                main_transform,
                 T.ToTensor(),
                 T.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
             ]
         )
 
         self.transform_test = T.Compose(
             [
@@ -96,22 +106,28 @@
         if split not in list(self.root.iterdir()):
             raise FileNotFoundError(
                 f"a {split} Imagenet split was not found in {self.root},"
                 f" make sure the folder contains a subfolder named {split}"
             )
 
     def prepare_data(self) -> None:
-        if self.ood_name == "inaturalist":
+        if self.test_alt is not None:
+            self.data = self.dataset(
+                self.root,
+                split="test",
+                download=True,
+            )
+        if self.ood_ds == "inaturalist":
             self.ood = self.ood_dataset(
                 self.root,
                 version="2021_valid",
                 download=True,
                 transform=self.transform_test,
             )
-        elif self.ood_name != "textures":
+        elif self.ood_ds != "textures":
             self.ood = self.ood_dataset(
                 self.root,
                 split="test",
                 download=True,
                 transform=self.transform_test,
             )
         else:
@@ -120,47 +136,59 @@
                 split="train",
                 download=True,
                 transform=self.transform_test,
             )
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
+            if self.test_alt is not None:
+                raise ValueError(
+                    "The test_alt argument is not supported for training."
+                )
             self.train = self.dataset(
                 self.root,
                 split="train",
                 transform=self.transform_train,
             )
             self.val = self.dataset(
                 self.root,
                 split="val",
                 transform=self.transform_test,
             )
-        if stage == "test" or stage is None:
+        if stage == "test":
             self.test = self.dataset(
                 self.root,
                 split="val",
                 transform=self.transform_test,
             )
-            if self.ood_name == "inaturalist":
+            if self.ood_ds == "inaturalist":
                 self.ood = self.ood_dataset(
                     self.root,
                     version="2021_valid",
                     transform=self.transform_test,
                 )
             else:
                 self.ood = self.ood_dataset(
                     self.root,
                     transform=self.transform_test,
                     download=True,
                 )
 
     def train_dataloader(self) -> DataLoader:
+        r"""Gets the training dataloader for ImageNet.
+        Returns:
+            DataLoader: ImageNet training dataloader.
+        """
         return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
+        r"""Gets the validation dataloader for ImageNet.
+        Returns:
+            DataLoader: ImageNet validation dataloader.
+        """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
         r"""Gets test dataloaders for ImageNet.
         Returns:
             List[DataLoader]: ImageNet test set (in distribution data) and
             Textures test split (out-of-distribution data).
@@ -184,12 +212,16 @@
         cls,
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=256)
-        p.add_argument("--val_split", type=int, default=0)
         p.add_argument("--num_workers", type=int, default=4)
-        p.add_argument("--ood_name", type=str, default="svhn")
-        p.add_argument("--test_option", type=str)
+        p.add_argument("--ood_ds", choices=cls.ood_datasets, default="svhn")
+        p.add_argument("--test_alt", choices=cls.test_datasets, default=None)
+        p.add_argument("--procedure", choices=["A3"], default=None)
+        p.add_argument("--train_size", type=int, default=224)
+        p.add_argument(
+            "--rand_augment", dest="rand_augment_opt", type=str, default=None
+        )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/mnist.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from torchvision.datasets import MNIST, FashionMNIST
 
 from torch_uncertainty.transforms import Cutout
 
 
 # fmt: on
 class MNISTDataModule(LightningDataModule):
+    num_classes = 10
+    num_channels = 1
+    input_shape = (1, 28, 28)
+
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
         val_split: int = 0,
         num_workers: int = 1,
         cutout: int = None,
@@ -80,15 +84,15 @@
             if self.val_split == 0:
                 self.val = self.dataset(
                     self.root,
                     train=False,
                     download=False,
                     transform=self.transform_test,
                 )
-        if stage == "test" or stage is None:
+        if stage == "test":
             self.test = self.dataset(
                 self.root,
                 train=False,
                 download=False,
                 transform=self.transform_test,
             )
             self.ood = self.ood_dataset(
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datamodules/tiny_imagenet.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/tiny_imagenet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
+import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
-from torch.utils.data import DataLoader, Dataset, random_split
+from timm.data.auto_augment import rand_augment_transform
+from torch.utils.data import DataLoader, Dataset
 from torchvision.datasets import SVHN
 
 from ..datasets import TinyImageNet
 
 
 # fmt: on
 class TinyImageNetDataModule(LightningDataModule):
+    num_classes = 200
+    num_channels = 3
+
     def __init__(
         self,
         root: Union[str, Path],
         batch_size: int,
-        val_split: int = 0,
+        rand_augment_opt: str = None,
         num_workers: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
         # TODO: COMPUTE STATS
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
         self.batch_size = batch_size
-        self.val_split = val_split
         self.num_workers = num_workers
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
         self.dataset = TinyImageNet
         self.ood_dataset = SVHN
-        self.num_classes = 200
+
+        if rand_augment_opt is not None:
+            main_transform = rand_augment_transform(rand_augment_opt, {})
+        else:
+            main_transform = nn.Identity()
 
         self.transform_train = T.Compose(
             [
                 T.RandomCrop(64, padding=4),
                 T.RandomHorizontalFlip(),
+                main_transform,
                 T.ToTensor(),
                 T.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
             ]
         )
 
         self.transform_test = T.Compose(
             [
@@ -59,50 +68,52 @@
         if split not in list(self.root.iterdir()):
             raise FileNotFoundError(
                 f"a {split} TinyImagenet split was not found in {self.root},"
                 f" make sure the folder contains a subfolder named {split}"
             )
 
     def prepare_data(self) -> None:
-        # self.dataset(self.root, split="train")
-        # self.dataset(self.root, split="val")
         self.ood_dataset(self.root, split="test", download=True)
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
-            full = self.dataset(
+            self.train = self.dataset(
                 self.root,
                 split="train",
                 transform=self.transform_train,
             )
-            self.train, self.val = random_split(
-                full, [len(full) - self.val_split, self.val_split]
+            self.val = self.dataset(
+                self.root,
+                split="val",
+                transform=self.transform_test,
             )
-            if self.val_split == 0:
-                self.val = self.dataset(
-                    self.root,
-                    split="val",
-                    transform=self.transform_test,
-                )
-        if stage == "test" or stage is None:
+        if stage == "test":
             self.test = self.dataset(
                 self.root,
                 split="val",
                 transform=self.transform_test,
             )
             self.ood = self.ood_dataset(
                 self.root,
                 split="test",
                 transform=self.transform_test,
             )
 
     def train_dataloader(self) -> DataLoader:
+        r"""Gets the training dataloader for TinyImageNet.
+        Returns:
+            DataLoader: TinyImageNet training dataloader.
+        """
         return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
+        r"""Gets the validation dataloader for TinyImageNet.
+        Returns:
+            DataLoader: TinyImageNet validation dataloader.
+        """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
         r"""Gets test dataloaders for TinyImageNet.
         Returns:
             List[DataLoader]: TinyImageNet test set (in distribution data) and
             SVHN test split (out-of-distribution data).
@@ -126,10 +137,12 @@
         cls,
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=256)
-        p.add_argument("--val_split", type=int, default=0)
         p.add_argument("--num_workers", type=int, default=4)
+        p.add_argument(
+            "--rand_augment", dest="rand_augment_opt", type=str, default=None
+        )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datasets/aggregated_dataset.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datasets/aggregated_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datasets/cifar_h.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_h.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,64 +8,78 @@
 
 import numpy as np
 
 
 # fmt:on
 class CIFAR10_H(CIFAR10):
     htest_list = [["cifar-10h-probs.npy", "7b41f73eee90fdefc73bfc820ab29ba8"]]
-    cifarh_url = (
+    url = (
         "https://github.com/jcpeterson/cifar-10h/raw/master/data/"
         "cifar10h-probs.npy"
     )
 
     def __init__(
         self,
         root: str,
-        train: bool = True,
-        transform: Callable[..., Any] | None = None,
-        target_transform: Callable[..., Any] | None = None,
+        train: bool = None,
+        transform: Callable[..., Any] = None,
+        target_transform: Callable[..., Any] = None,
         download: bool = False,
     ) -> None:
         """`CIFAR-10H <https://github.com/jcpeterson/cifar-10h>`_ Dataset.
 
         Args:
             root (string): Root directory of dataset where file
                 ``cifar-10h-probs.npy`` exists or will be saved to if download
                 is set to True.
-            train (bool, optional): If True, creates dataset from training set,
-                otherwise creates from test set.
+            train (bool, optional): For API consistency, not used.
             transform (callable, optional): A function/transform that takes in
                 a PIL image and returns a transformed version. E.g,
                 ``transforms.RandomCrop``
             target_transform (callable, optional): A function/transform that
                 takes in the target and transforms it.
             download (bool, optional): If True, downloads the dataset from the
                 internet and puts it in root directory. If dataset is already
                 downloaded, it is not downloaded again.
         """
 
-        super().__init__(root, train, transform, target_transform, download)
+        print(
+            "WARNING: CIFAR10_H cannot be used with Classification routines "
+            "for now."
+        )
+        super().__init__(
+            root,
+            train=False,
+            transform=transform,
+            target_transform=target_transform,
+            download=download,
+        )
 
-        # Download the new targets
-        if not self._check_specific_integrity() and download:
-            download_url(
-                self.cifarh_url,
-                root,
-                filename=self.htest_list[0][0],
-                md5=self.htest_list[0][1],
-            )
-        elif not download:
+        if download:
+            self.download()
+
+        if not self._check_specific_integrity():
             raise RuntimeError(
-                "Dataset not found. You can use download=True to download it"
+                "Dataset not found or corrupted. You can use download=True to "
+                "download it."
             )
+
         self.targets = list(
             torch.as_tensor(
                 np.load(os.path.join(self.root, self.htest_list[0][0]))
             )
         )
 
     def _check_specific_integrity(self) -> bool:
         for filename, md5 in self.htest_list:
             fpath = os.path.join(self.root, filename)
             if not check_integrity(fpath, md5):
                 return False
         return True
+
+    def download(self) -> None:
+        download_url(
+            self.url,
+            self.root,
+            filename=self.htest_list[0][0],
+            md5=self.htest_list[0][1],
+        )
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/datasets/tiny_imagenet.py` & `torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/tiny_imagenet.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/layers/batchens_layers.py` & `torch_uncertainty-0.1.2/torch_uncertainty/layers/batchens_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,14 @@
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.kernel_size = _pair(kernel_size)
         self.num_estimators = num_estimators
         self.stride = _pair(stride)
         self.padding = padding if isinstance(padding, str) else _pair(padding)
         self.dilation = _pair(dilation)
-        self.groups = groups
 
         self.conv = nn.Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
             stride=stride,
             padding=padding,
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/layers/masksembles_layers.py` & `torch_uncertainty-0.1.2/torch_uncertainty/layers/masksembles_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,26 +199,29 @@
         bias: bool = True,
         device: Union[Any, None] = None,
         dtype: Union[Any, None] = None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
 
+        if scale < 1:
+            raise ValueError(f"Attribute `scale` should be >= 1, not {scale}.")
+
         self.mask = Mask1D(
             in_features, num_masks=num_estimators, scale=scale, **factory_kwargs
         )
-        self.conv1x1 = nn.Linear(
+        self.linear = nn.Linear(
             in_features=in_features,
             out_features=out_features,
             bias=bias,
             **factory_kwargs,
         )
 
     def forward(self, input: Tensor) -> Tensor:
-        return self.conv1x1(self.mask(input))
+        return self.linear(self.mask(input))
 
 
 class MaskedConv2d(nn.Module):
     r"""Masksembles-style Conv2d layer.
 
     Args:
         in_channels (int): Number of channels in the input image.
@@ -260,14 +263,17 @@
         bias: bool = True,
         device: Union[Any, None] = None,
         dtype: Union[Any, None] = None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
 
+        if scale < 1:
+            raise ValueError(f"Attribute `scale` should be >= 1, not {scale}.")
+
         self.mask = Mask2D(
             in_channels, num_masks=num_estimators, scale=scale, **factory_kwargs
         )
         self.conv = nn.Conv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/layers/packed_layers.py` & `torch_uncertainty-0.1.2/torch_uncertainty/layers/packed_layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,24 @@
         last: bool = False,
         device=None,
         dtype=None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
 
+        if alpha <= 0:
+            raise ValueError(f"Attribute `alpha` should be > 0, not {alpha}")
+
+        if not isinstance(gamma, int):
+            raise ValueError(
+                f"Attribute `gamma` should be an int, not " f"{type(gamma)}"
+            )
+        if gamma <= 0:
+            raise ValueError(f"Attribute `gamma` should be >= 1, not {gamma}")
+
         self.num_estimators = num_estimators
         self.rearrange = rearrange
 
         # Define the number of features of the underlying convolution
         extended_in_features = int(in_features * (1 if first else alpha))
         extended_out_features = int(
             out_features * (num_estimators if last else alpha)
@@ -160,14 +170,24 @@
         last: bool = False,
         device: Union[Any, None] = None,
         dtype: Union[Any, None] = None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
 
+        if alpha <= 0:
+            raise ValueError(f"Attribute `alpha` should be > 0, not {alpha}")
+
+        if not isinstance(gamma, int):
+            raise ValueError(
+                f"Attribute `gamma` should be an int, not " f"{type(gamma)}"
+            )
+        if gamma <= 0:
+            raise ValueError(f"Attribute `gamma` should be >= 1, not {gamma}")
+
         self.num_estimators = num_estimators
 
         # Define the number of channels of the underlying convolution
         extended_in_channels = int(in_channels * (1 if first else alpha))
         extended_out_channels = int(
             out_channels * (num_estimators if last else alpha)
         )
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/brier_score.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/brier_score.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/disagreement.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/disagreement.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/entropy.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/fpr95.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/fpr95.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/jensen_shannon_divergence.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/jensen_shannon_divergence.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/mutual_information.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/mutual_information.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/nll.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/nll.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/metrics/variation_ratio.py` & `torch_uncertainty-0.1.2/torch_uncertainty/metrics/variation_ratio.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/batched.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/batched.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """_BatchedResNet in PyTorch.
 
 Reference:
 [1] Kaiming He, Xiangyu Zhang, Shaoqing Ren, Jian Sun
     Deep Residual Learning for Image Recognition. arXiv:1512.03385
 """
 # fmt: off
+from typing import List, Type, Union
+
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 
 from ...layers import BatchConv2d, BatchLinear
 
 # fmt: on
@@ -26,43 +28,47 @@
 
     def __init__(
         self,
         in_planes: int,
         planes: int,
         stride: int = 1,
         num_estimators: int = 4,
+        groups: int = 1,
     ) -> None:
         super().__init__()
         self.conv1 = BatchConv2d(
             in_planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
+            groups=groups,
             stride=stride,
             padding=1,
             bias=False,
         )
         self.bn1 = nn.BatchNorm2d(planes)
         self.conv2 = BatchConv2d(
             planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
+            groups=groups,
             stride=1,
             padding=1,
             bias=False,
         )
         self.bn2 = nn.BatchNorm2d(planes)
 
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != self.expansion * planes:
             self.shortcut = nn.Sequential(
                 nn.Conv2d(
                     in_planes,
                     self.expansion * planes,
+                    groups=groups,
                     kernel_size=1,
                     stride=stride,
                     bias=False,
                 ),
                 nn.BatchNorm2d(self.expansion * planes),
             )
 
@@ -79,51 +85,56 @@
 
     def __init__(
         self,
         in_planes: int,
         planes: int,
         stride: int = 1,
         num_estimators: int = 4,
+        groups: int = 1,
     ) -> None:
         super(Bottleneck, self).__init__()
         self.conv1 = BatchConv2d(
             in_planes,
             planes,
             kernel_size=1,
             num_estimators=num_estimators,
+            groups=groups,
             bias=False,
         )
         self.bn1 = nn.BatchNorm2d(planes)
         self.conv2 = BatchConv2d(
             planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
+            groups=groups,
             stride=stride,
             padding=1,
             bias=False,
         )
         self.bn2 = nn.BatchNorm2d(planes)
         self.conv3 = BatchConv2d(
             planes,
             self.expansion * planes,
             num_estimators=num_estimators,
+            groups=groups,
             kernel_size=1,
             bias=False,
         )
         self.bn3 = nn.BatchNorm2d(self.expansion * planes)
 
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != self.expansion * planes:
             self.shortcut = nn.Sequential(
                 BatchConv2d(
                     in_planes,
                     self.expansion * planes,
                     kernel_size=1,
                     num_estimators=num_estimators,
+                    groups=groups,
                     stride=stride,
                     bias=False,
                 ),
                 nn.BatchNorm2d(self.expansion * planes),
             )
 
     def forward(self, input: Tensor) -> Tensor:
@@ -134,45 +145,49 @@
         out = F.relu(out)
         return out
 
 
 class _BatchedResNet(nn.Module):
     def __init__(
         self,
-        block,
-        num_blocks,
+        block: Type[Union[BasicBlock, Bottleneck]],
+        num_blocks: List[int],
         in_channels: int,
-        num_estimators,
+        num_estimators: int,
+        groups: int = 1,
         num_classes=10,
         width_multiplier: int = 1,
         imagenet_structure: bool = True,
     ):
         super().__init__()
         self.in_planes = 64 * width_multiplier
+        self.num_estimators = num_estimators
 
         self.width_multiplier = width_multiplier
         if imagenet_structure:
             self.conv1 = BatchConv2d(
                 3,
                 64 * self.width_multiplier,
                 kernel_size=7,
                 stride=2,
                 padding=3,
-                bias=False,
                 num_estimators=num_estimators,
+                groups=groups,
+                bias=False,
             )
         else:
             self.conv1 = BatchConv2d(
                 in_channels,
                 64 * self.width_multiplier,
                 kernel_size=3,
                 stride=1,
                 padding=1,
-                bias=False,
                 num_estimators=num_estimators,
+                groups=groups,
+                bias=False,
             )
         self.bn1 = nn.BatchNorm2d(64 * self.width_multiplier)
 
         if imagenet_structure:
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
@@ -181,69 +196,85 @@
 
         self.layer1 = self._make_layer(
             block,
             64 * width_multiplier,
             num_blocks[0],
             stride=1,
             num_estimators=num_estimators,
+            groups=groups,
         )
         self.layer2 = self._make_layer(
             block,
             128 * width_multiplier,
             num_blocks[1],
             stride=2,
             num_estimators=num_estimators,
+            groups=groups,
         )
         self.layer3 = self._make_layer(
             block,
             256 * width_multiplier,
             num_blocks[2],
             stride=2,
             num_estimators=num_estimators,
+            groups=groups,
         )
         self.layer4 = self._make_layer(
             block,
             512 * width_multiplier,
             num_blocks[3],
             stride=2,
             num_estimators=num_estimators,
+            groups=groups,
         )
         self.pool = nn.AdaptiveAvgPool2d(output_size=1)
         self.flatten = nn.Flatten(1)
 
         self.linear = BatchLinear(
             512 * width_multiplier * block.expansion,
             num_classes,
             num_estimators=num_estimators,
         )
 
-    def _make_layer(self, block, planes, num_blocks, stride, num_estimators):
+    def _make_layer(
+        self,
+        block: Type[Union[BasicBlock, Bottleneck]],
+        planes: int,
+        num_blocks: int,
+        stride: int,
+        num_estimators: int,
+        groups: int,
+    ):
         strides = [stride] + [1] * (num_blocks - 1)
         layers = []
         for stride in strides:
-            layers.append(block(self.in_planes, planes, stride, num_estimators))
+            layers.append(
+                block(self.in_planes, planes, stride, num_estimators, groups)
+            )
             self.in_planes = planes * block.expansion
         return nn.Sequential(*layers)
 
     def forward(self, x):
-        out = F.relu(self.bn1(self.conv1(x)))
+        out = x.repeat(self.num_estimators, 1, 1, 1)
+        out = F.relu(self.bn1(self.conv1(out)))
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
         out = self.pool(out)
         out = self.flatten(out)
         out = self.linear(out)
         return out
 
 
 def batched_resnet18(
     in_channels: int,
     num_estimators: int,
+    groups: int,
     num_classes: int,
     imagenet_structure: bool = True,
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
@@ -257,21 +288,23 @@
     """
     return _BatchedResNet(
         BasicBlock,
         [2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet34(
     in_channels: int,
     num_estimators: int,
+    groups: int,
     num_classes: int,
     imagenet_structure: bool = True,
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
@@ -285,21 +318,23 @@
     """
     return _BatchedResNet(
         BasicBlock,
         [3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet50(
     in_channels: int,
     num_estimators: int,
+    groups: int,
     num_classes: int,
     width_multiplier: int = 1,
     imagenet_structure: bool = True,
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
@@ -315,21 +350,23 @@
     return _BatchedResNet(
         Bottleneck,
         [3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         width_multiplier=width_multiplier,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet101(
     in_channels: int,
     num_estimators: int,
+    groups: int,
     num_classes: int,
     imagenet_structure: bool = True,
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
@@ -343,21 +380,23 @@
     """
     return _BatchedResNet(
         Bottleneck,
         [3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
 
 
 def batched_resnet152(
     in_channels: int,
     num_estimators: int,
+    groups: int,
     num_classes: int,
     imagenet_structure: bool = True,
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
@@ -373,9 +412,10 @@
     """
     return _BatchedResNet(
         Bottleneck,
         [3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/masked.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/masked.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         stride: int = 1,
         num_estimators: int = 4,
         scale: float = 2.0,
         groups: int = 1,
     ):
         super(BasicBlock, self).__init__()
 
-        # No subgroups for the first layer
         self.conv1 = MaskedConv2d(
             in_planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
             scale=scale,
+            groups=groups,
             stride=stride,
             padding=1,
             bias=False,
         )
         self.bn1 = nn.BatchNorm2d(planes)
         self.conv2 = MaskedConv2d(
             planes,
@@ -90,21 +90,21 @@
         stride: int = 1,
         num_estimators: int = 4,
         scale: float = 2.0,
         groups: int = 1,
     ):
         super(Bottleneck, self).__init__()
 
-        # No subgroups for the first layer
         self.conv1 = MaskedConv2d(
             in_planes,
             planes,
             kernel_size=1,
             num_estimators=num_estimators,
             scale=scale,
+            groups=groups,
             bias=False,
         )
         self.bn1 = nn.BatchNorm2d(planes)
         self.conv2 = MaskedConv2d(
             planes,
             planes,
             kernel_size=3,
@@ -178,25 +178,25 @@
         if imagenet_structure:
             self.conv1 = nn.Conv2d(
                 self.in_channels,
                 block_planes,
                 kernel_size=7,
                 stride=2,
                 padding=3,
-                groups=1,  # No groups for the first layer
+                groups=groups,
                 bias=False,
             )
         else:
             self.conv1 = nn.Conv2d(
                 self.in_channels,
                 block_planes,
                 kernel_size=3,
                 stride=1,
                 padding=1,
-                groups=1,
+                groups=groups,
                 bias=False,
             )
 
         self.bn1 = nn.BatchNorm2d(block_planes)
 
         if imagenet_structure:
             self.optional_pool = nn.MaxPool2d(
@@ -275,15 +275,16 @@
                     groups=groups,
                 )
             )
             self.in_planes = planes * block.expansion
         return nn.Sequential(*layers)
 
     def forward(self, x: Tensor) -> Tensor:
-        out = F.relu(self.bn1(self.conv1(x)))
+        out = x.repeat(self.num_estimators, 1, 1, 1)
+        out = F.relu(self.bn1(self.conv1(out)))
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = self.layer4(out)
 
         out = self.pool(out)
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/packed.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/packed.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,58 +3,93 @@
 
 import torch.nn as nn
 import torch.nn.functional as F
 from einops import rearrange
 from torch import Tensor
 
 from ...layers import PackedConv2d, PackedLinear
+from ...utils import load_hf
 
 # fmt: on
 __all__ = [
     "packed_resnet18",
     "packed_resnet34",
     "packed_resnet50",
     "packed_resnet101",
     "packed_resnet152",
 ]
 
+weight_ids = {
+    "10": {
+        "18": None,
+        "32": None,
+        "50": "pe_resnet50_c10",
+        "101": None,
+        "152": None,
+    },
+    "100": {
+        "18": None,
+        "32": None,
+        "50": "pe_resnet50_c100",
+        "101": None,
+        "152": None,
+    },
+    "1000": {
+        "18": None,
+        "32": None,
+        "50": "pe_resnet50_in1k",
+        "101": None,
+        "152": None,
+    },
+    "1000_wider": {
+        "18": None,
+        "32": None,
+        "50": "pex4_resnet50",
+        "101": None,
+        "152": None,
+    },
+}
+
 
 class BasicBlock(nn.Module):
     expansion = 1
 
     def __init__(
         self,
         in_planes: int,
         planes: int,
         stride: int = 1,
         alpha: float = 2,
         num_estimators: int = 4,
         gamma: int = 1,
+        groups: int = 1,
     ):
         super(BasicBlock, self).__init__()
 
         # No subgroups for the first layer
         self.conv1 = PackedConv2d(
             in_planes,
             planes,
             kernel_size=3,
             alpha=alpha,
             num_estimators=num_estimators,
+            groups=groups,
             stride=stride,
             padding=1,
             bias=False,
         )
         self.bn1 = nn.BatchNorm2d(planes * alpha)
         self.conv2 = PackedConv2d(
             planes,
             planes,
             kernel_size=3,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
             stride=1,
             padding=1,
             bias=False,
         )
         self.bn2 = nn.BatchNorm2d(planes * alpha)
 
         self.shortcut = nn.Sequential()
@@ -63,14 +98,15 @@
                 PackedConv2d(
                     in_planes,
                     self.expansion * planes,
                     kernel_size=1,
                     alpha=alpha,
                     num_estimators=num_estimators,
                     gamma=gamma,
+                    groups=groups,
                     stride=stride,
                     bias=False,
                 ),
                 nn.BatchNorm2d(self.expansion * planes * alpha),
             )
 
     def forward(self, x: Tensor) -> Tensor:
@@ -88,62 +124,66 @@
         self,
         in_planes: int,
         planes: int,
         stride: int = 1,
         alpha: float = 2,
         num_estimators: int = 4,
         gamma: int = 1,
+        groups: int = 1,
     ):
         super(Bottleneck, self).__init__()
 
         # No subgroups for the first layer
         self.conv1 = PackedConv2d(
             in_planes,
             planes,
             kernel_size=1,
             alpha=alpha,
             num_estimators=num_estimators,
-            gamma=1,  # No groups in the first layer
+            gamma=1,  # No groups from gamma in the first layer
+            groups=groups,
             bias=False,
         )
         self.bn1 = nn.BatchNorm2d(planes * alpha)
         self.conv2 = PackedConv2d(
             planes,
             planes,
             kernel_size=3,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
             stride=stride,
             padding=1,
-            groups=1,
+            groups=groups,
             bias=False,
         )
         self.bn2 = nn.BatchNorm2d(planes * alpha)
         self.conv3 = PackedConv2d(
             planes,
             self.expansion * planes,
             kernel_size=1,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
             bias=False,
         )
         self.bn3 = nn.BatchNorm2d(self.expansion * planes * alpha)
 
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != self.expansion * planes:
             self.shortcut = nn.Sequential(
                 PackedConv2d(
                     in_planes,
                     self.expansion * planes,
                     kernel_size=1,
                     alpha=alpha,
                     num_estimators=num_estimators,
                     gamma=gamma,
+                    groups=groups,
                     stride=stride,
                     bias=False,
                 ),
                 nn.BatchNorm2d(self.expansion * planes * alpha),
             )
 
     def forward(self, x: Tensor) -> Tensor:
@@ -161,14 +201,15 @@
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         alpha: int = 2,
         gamma: int = 1,
+        groups: int = 1,
         imagenet_structure: bool = True,
     ) -> None:
         super().__init__()
 
         self.in_channels = in_channels
         self.num_estimators = num_estimators
         self.in_planes = 64
@@ -180,29 +221,29 @@
                 block_planes,
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 alpha=alpha,
                 num_estimators=num_estimators,
                 gamma=1,  # No groups for the first layer
-                groups=1,
+                groups=groups,
                 bias=False,
                 first=True,
             )
         else:
             self.conv1 = PackedConv2d(
                 self.in_channels,
                 block_planes,
                 kernel_size=3,
                 stride=1,
                 padding=1,
                 alpha=alpha,
                 num_estimators=num_estimators,
                 gamma=1,  # No groups for the first layer
-                groups=1,
+                groups=groups,
                 bias=False,
                 first=True,
             )
 
         self.bn1 = nn.BatchNorm2d(block_planes * alpha)
 
         if imagenet_structure:
@@ -216,41 +257,45 @@
             block,
             block_planes,
             num_blocks[0],
             stride=1,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
         )
         self.layer2 = self._make_layer(
             block,
             block_planes * 2,
             num_blocks[1],
             stride=2,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
         )
         self.layer3 = self._make_layer(
             block,
             block_planes * 4,
             num_blocks[2],
             stride=2,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
         )
         self.layer4 = self._make_layer(
             block,
             block_planes * 8,
             num_blocks[3],
             stride=2,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
         )
 
         self.pool = nn.AdaptiveAvgPool2d(output_size=1)
         self.flatten = nn.Flatten(1)
 
         self.linear = PackedLinear(
             block_planes * 8 * block.expansion,
@@ -265,26 +310,28 @@
         block: Type[Union[BasicBlock, Bottleneck]],
         planes: int,
         num_blocks: int,
         stride: int,
         alpha: float,
         num_estimators: int,
         gamma: int,
+        groups: int,
     ) -> nn.Module:
         strides = [stride] + [1] * (num_blocks - 1)
         layers = []
         for stride in strides:
             layers.append(
                 block(
                     self.in_planes,
                     planes,
                     stride,
                     alpha=alpha,
                     num_estimators=num_estimators,
                     gamma=gamma,
+                    groups=groups,
                 )
             )
             self.in_planes = planes * block.expansion
         return nn.Sequential(*layers)
 
     def forward(self, x: Tensor) -> Tensor:
         out = F.relu(self.bn1(self.conv1(x)))
@@ -306,147 +353,185 @@
 
 def packed_resnet18(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    groups: int,
     imagenet_structure: bool = True,
+    pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-18.
     """
-    return _PackedResNet(
+    net = _PackedResNet(
         block=BasicBlock,
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
+        groups=groups,
         num_classes=num_classes,
         imagenet_structure=imagenet_structure,
     )
+    if pretrained:
+        weights = weight_ids[str(num_classes)][18]
+        if weights is None:
+            raise ValueError("No pretrained weights for this configuration")
+        net.load_state_dict(load_hf(weights))
+    return net
 
 
 def packed_resnet34(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    groups: int,
     imagenet_structure: bool = True,
+    pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-34.
     """
-    return _PackedResNet(
+    net = _PackedResNet(
         block=BasicBlock,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
+        groups=groups,
         num_classes=num_classes,
         imagenet_structure=imagenet_structure,
     )
+    if pretrained:
+        weights = weight_ids[str(num_classes)][34]
+        if weights is None:
+            raise ValueError("No pretrained weights for this configuration")
+        net.load_state_dict(load_hf(weights))
+    return net
 
 
 def packed_resnet50(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    groups: int,
     imagenet_structure: bool = True,
+    pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-50.
     """
-    return _PackedResNet(
+    net = _PackedResNet(
         block=Bottleneck,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
+        groups=groups,
         num_classes=num_classes,
         imagenet_structure=imagenet_structure,
     )
+    if pretrained:
+        weights = weight_ids[str(num_classes)][50]
+        if weights is None:
+            raise ValueError("No pretrained weights for this configuration")
+        net.load_state_dict(load_hf(weights))
+    return net
 
 
 def packed_resnet101(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    groups: int,
     imagenet_structure: bool = True,
+    pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-101.
     """
-    return _PackedResNet(
+    net = _PackedResNet(
         block=Bottleneck,
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
+        groups=groups,
         num_classes=num_classes,
         imagenet_structure=imagenet_structure,
     )
+    if pretrained:
+        weights = weight_ids[str(num_classes)][101]
+        if weights is None:
+            raise ValueError("No pretrained weights for this configuration")
+        net.load_state_dict(load_hf(weights))
+    return net
 
 
 def packed_resnet152(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
+    groups: int,
     imagenet_structure: bool = True,
+    pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -455,17 +540,24 @@
         num_classes (int): Number of classes to predict.
         imagenet_structure (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-152.
     """
-    return _PackedResNet(
+    net = _PackedResNet(
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
+        groups=groups,
         num_classes=num_classes,
         imagenet_structure=imagenet_structure,
     )
+    if pretrained:
+        weights = weight_ids[str(num_classes)][152]
+        if weights is None:
+            raise ValueError("No pretrained weights for this configuration")
+        net.load_state_dict(load_hf(weights))
+    return net
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/resnet/std.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/std.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/batched.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/batched.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,44 +14,48 @@
     def __init__(
         self,
         in_planes,
         planes,
         dropout_rate,
         stride=1,
         num_estimators=4,
+        groups: int = 1,
     ):
         super().__init__()
         self.bn1 = nn.BatchNorm2d(in_planes)
         self.conv1 = BatchConv2d(
             in_planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
+            groups=groups,
             padding=1,
             bias=False,
         )
         self.dropout = nn.Dropout(p=dropout_rate)
         self.bn2 = nn.BatchNorm2d(planes)
         self.conv2 = BatchConv2d(
             planes,
             planes,
             kernel_size=3,
             num_estimators=num_estimators,
+            groups=groups,
             stride=stride,
             padding=1,
             bias=False,
         )
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != planes:
             self.shortcut = nn.Sequential(
                 BatchConv2d(
                     in_planes,
                     planes,
                     kernel_size=1,
                     num_estimators=num_estimators,
+                    groups=groups,
                     stride=stride,
                     bias=True,
                 ),
             )
 
     def forward(self, x):
         out = self.dropout(self.conv1(F.relu(self.bn1(x))))
@@ -64,17 +68,18 @@
     def __init__(
         self,
         depth: int,
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         num_estimators: int,
+        groups: int = 1,
         dropout_rate: float = 0.0,
         imagenet_structure: bool = True,
-    ):
+    ) -> None:
         super().__init__()
         self.num_estimators = num_estimators
         self.in_planes = 16
 
         assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         n = (depth - 4) / 6
         k = widen_factor
@@ -82,30 +87,30 @@
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
         if imagenet_structure:
             self.conv1 = BatchConv2d(
                 in_channels,
                 nStages[0],
                 num_estimators=self.num_estimators,
+                groups=groups,
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 bias=True,
-                groups=1,
             )
         else:
             self.conv1 = BatchConv2d(
                 in_channels,
                 nStages[0],
                 num_estimators=self.num_estimators,
+                groups=groups,
                 kernel_size=3,
                 stride=1,
                 padding=1,
                 bias=True,
-                groups=1,
             )
 
         if imagenet_structure:
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
@@ -114,30 +119,33 @@
         self.layer1 = self._wide_layer(
             WideBasicBlock,
             nStages[1],
             n,
             dropout_rate,
             stride=1,
             num_estimators=self.num_estimators,
+            groups=groups,
         )
         self.layer2 = self._wide_layer(
             WideBasicBlock,
             nStages[2],
             n,
             dropout_rate,
             stride=2,
             num_estimators=self.num_estimators,
+            groups=groups,
         )
         self.layer3 = self._wide_layer(
             WideBasicBlock,
             nStages[3],
             n,
             dropout_rate,
             stride=2,
             num_estimators=self.num_estimators,
+            groups=groups,
         )
         self.bn1 = nn.BatchNorm2d(nStages[3])
 
         self.pool = nn.AdaptiveAvgPool2d(output_size=1)
         self.flatten = nn.Flatten(1)
 
         self.linear = BatchLinear(
@@ -150,34 +158,37 @@
         self,
         block: nn.Module,
         planes: int,
         num_blocks: int,
         dropout_rate: float,
         stride: int,
         num_estimators: int,
+        groups: int,
     ):
         strides = [stride] + [1] * (int(num_blocks) - 1)
         layers = []
 
         for stride in strides:
             layers.append(
                 block(
-                    self.in_planes,
-                    planes,
-                    dropout_rate,
-                    stride,
-                    num_estimators,
+                    in_planes=self.in_planes,
+                    planes=planes,
+                    dropout_rate=dropout_rate,
+                    stride=stride,
+                    num_estimators=num_estimators,
+                    groups=groups,
                 )
             )
             self.in_planes = planes
 
         return nn.Sequential(*layers)
 
     def forward(self, x):
-        out = self.conv1(x)
+        out = x.repeat(self.num_estimators, 1, 1, 1)
+        out = self.conv1(out)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = F.relu(self.bn1(out))
 
         out = self.pool(out)
@@ -186,14 +197,15 @@
 
         return out
 
 
 def batched_wideresnet28x10(
     in_channels: int,
     num_estimators: int,
+    groups: int,
     num_classes: int,
     imagenet_structure: bool = True,
 ) -> _BatchedWide:
     """BatchEnsemble of Wide-ResNet-28x10 from `Wide Residual Networks
     <https://arxiv.org/pdf/1605.07146.pdf>`_.
 
     Args:
@@ -209,9 +221,10 @@
     return _BatchedWide(
         in_channels=in_channels,
         depth=28,
         widen_factor=10,
         dropout_rate=0.3,
         num_classes=num_classes,
         num_estimators=num_estimators,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/masked.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/masked.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,16 @@
                 )
             )
             self.in_planes = planes
 
         return nn.Sequential(*layers)
 
     def forward(self, x):
-        out = self.conv1(x)
+        out = x.repeat(self.num_estimators, 1, 1, 1)
+        out = self.conv1(out)
         out = self.optional_pool(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = F.relu(self.bn1(out))
 
         out = self.pool(out)
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/packed.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/packed.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,50 +19,54 @@
         in_planes: int,
         planes: int,
         dropout_rate: float,
         stride: int = 1,
         alpha: float = 2,
         num_estimators: int = 4,
         gamma: int = 1,
+        groups: int = 1,
     ):
         super().__init__()
         self.bn1 = nn.BatchNorm2d(alpha * in_planes)
         self.conv1 = PackedConv2d(
             in_planes,
             planes,
             kernel_size=3,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
             padding=1,
             bias=False,
         )
         self.dropout = nn.Dropout(p=dropout_rate)
         self.bn2 = nn.BatchNorm2d(alpha * planes)
         self.conv2 = PackedConv2d(
             planes,
             planes,
             kernel_size=3,
             alpha=alpha,
             num_estimators=num_estimators,
             gamma=gamma,
+            groups=groups,
             stride=stride,
             padding=1,
             bias=False,
         )
         self.shortcut = nn.Sequential()
         if stride != 1 or in_planes != planes:
             self.shortcut = nn.Sequential(
                 PackedConv2d(
                     in_planes,
                     planes,
                     kernel_size=1,
                     alpha=alpha,
                     num_estimators=num_estimators,
                     gamma=gamma,
+                    groups=groups,
                     stride=stride,
                     bias=True,
                 ),
             )
 
     def forward(self, x):
         out = self.dropout(self.conv1(F.relu(self.bn1(x))))
@@ -77,14 +81,15 @@
         depth: int,
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         num_estimators: int = 4,
         alpha: int = 2,
         gamma: int = 1,
+        groups: int = 1,
         dropout_rate: float = 0,
         imagenet_structure: bool = True,
     ):
         super().__init__()
         self.num_estimators = num_estimators
         self.in_planes = 16
 
@@ -100,28 +105,29 @@
                 nStages[0],
                 kernel_size=7,
                 alpha=alpha,
                 num_estimators=self.num_estimators,
                 stride=2,
                 padding=3,
                 gamma=1,  # No groups for the first layer
-                groups=1,
+                groups=groups,
                 bias=True,
                 first=True,
             )
         else:
             self.conv1 = PackedConv2d(
                 in_channels,
                 nStages[0],
                 kernel_size=3,
                 alpha=alpha,
                 num_estimators=self.num_estimators,
                 stride=1,
                 padding=1,
                 gamma=gamma,
+                groups=groups,
                 bias=True,
                 first=True,
             )
 
         if imagenet_structure:
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
@@ -134,34 +140,37 @@
             nStages[1],
             num_blocks,
             dropout_rate,
             stride=1,
             alpha=alpha,
             num_estimators=self.num_estimators,
             gamma=gamma,
+            groups=groups,
         )
         self.layer2 = self._wide_layer(
             WideBasicBlock,
             nStages[2],
             num_blocks,
             dropout_rate,
             stride=2,
             alpha=alpha,
             num_estimators=self.num_estimators,
             gamma=gamma,
+            groups=groups,
         )
         self.layer3 = self._wide_layer(
             WideBasicBlock,
             nStages[3],
             num_blocks,
             dropout_rate,
             stride=2,
             alpha=alpha,
             num_estimators=self.num_estimators,
             gamma=gamma,
+            groups=groups,
         )
         self.bn1 = nn.BatchNorm2d(nStages[3] * alpha, momentum=0.9)
 
         self.pool = nn.AdaptiveAvgPool2d(output_size=1)
         self.flatten = nn.Flatten(1)
 
         self.linear = PackedLinear(
@@ -178,28 +187,30 @@
         planes: int,
         num_blocks: int,
         dropout_rate: float,
         stride: int,
         alpha: float,
         num_estimators: int,
         gamma: int,
+        groups: int,
     ):
         strides = [stride] + [1] * (int(num_blocks) - 1)
         layers = []
 
         for stride in strides:
             layers.append(
                 block(
                     in_planes=self.in_planes,
                     planes=planes,
                     dropout_rate=dropout_rate,
                     stride=stride,
                     alpha=alpha,
                     num_estimators=num_estimators,
                     gamma=gamma,
+                    groups=groups,
                 )
             )
             self.in_planes = planes
 
         return nn.Sequential(*layers)
 
     def forward(self, x):
@@ -220,14 +231,15 @@
 
 
 def packed_wideresnet28x10(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
+    groups: int,
     num_classes: int,
     imagenet_structure: bool = True,
 ) -> _PackedWide:
     """Packed-Ensembles of Wide-ResNet-28x10 from `Wide Residual Networks
     <https://arxiv.org/pdf/1605.07146.pdf>`_.
 
     Args:
@@ -247,9 +259,10 @@
         depth=28,
         widen_factor=10,
         num_classes=num_classes,
         dropout_rate=0.3,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
+        groups=groups,
         imagenet_structure=imagenet_structure,
     )
```

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/models/wideresnet/std.py` & `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/std.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/torch_uncertainty/utils/checkpoints.py` & `torch_uncertainty-0.1.2/torch_uncertainty/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.1/setup.py` & `torch_uncertainty-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['torch_uncertainty',
  'torch_uncertainty.baselines',
- 'torch_uncertainty.baselines.batched',
- 'torch_uncertainty.baselines.masked',
- 'torch_uncertainty.baselines.mimo',
- 'torch_uncertainty.baselines.packed',
- 'torch_uncertainty.baselines.standard',
+ 'torch_uncertainty.baselines.classification',
+ 'torch_uncertainty.baselines.utils',
  'torch_uncertainty.datamodules',
  'torch_uncertainty.datasets',
+ 'torch_uncertainty.datasets.cifar',
+ 'torch_uncertainty.datasets.imagenet',
  'torch_uncertainty.layers',
  'torch_uncertainty.metrics',
  'torch_uncertainty.models',
  'torch_uncertainty.models.resnet',
  'torch_uncertainty.models.wideresnet',
+ 'torch_uncertainty.post_processing',
  'torch_uncertainty.routines',
  'torch_uncertainty.transforms',
  'torch_uncertainty.utils']
 
 package_data = \
 {'': ['*']}
 
@@ -31,17 +31,17 @@
  'tensorboard>=2.11.2,<3.0.0',
  'timm>=0.6.12,<0.7.0',
  'torchinfo>=1.7.1,<2.0.0',
  'torchvision>=0.14.1,<0.15.0']
 
 setup_kwargs = {
     'name': 'torch-uncertainty',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques.',
-    'long_description': '<div align="center">\n\n![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)\n\n[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty) [![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml) [![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/) [![Code Coverage](https://img.shields.io/codecov/c/github/ENSTA-U2IS/torch-uncertainty.svg)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty) [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n</div>\n\n_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.\n\n---\n\nThis package provides a multi-level API, including:\n- ready-to-train baselines on research datasets, such as ImageNet and CIFAR\n- baselines available for training on your datasets\n- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR.\n- layers available for use in your networks\n\n## Installation\n\nThe package can be installed from PyPI:\n\n```sh\npip install torch-uncertainty\n```\n\nTo contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.\n\n## Getting Started and Documentation\n\nPlease find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).\n\nA quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).\n\n## Implemented baselines\n\nTo date, the following baselines are implemented:\n\n- Deep Ensembles\n- Masksembles\n- Packed-Ensembles\n\n## Tutorials\n\n\n## Awesome Uncertainty repositories\n\nYou may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).\n\n## Other References\n\nThis package also contains the official implementation of Packed-Ensembles.\n\nIf you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):\n\t\n    @inproceedings{laurent2023packed,\n        title={Packed-Ensembles for Efficient Uncertainty Estimation},\n        author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},\n        booktitle={ICLR},\n        year={2023}\n    }\n',
+    'long_description': '<div align="center">\n\n![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)\n\n[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty)\n[![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml)\n[![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/)\n[![Code Coverage](https://codecov.io/github/ENSTA-U2IS/torch-uncertainty/coverage.svg?branch=master)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n</div>\n\n_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.\n\n:construction: _TorchUncertainty_ is in early development :construction: - expect massive changes but do reach out to us and contribute if you are interested by the project!\n\n---\n\nThis package provides a multi-level API, including:\n\n- ready-to-train baselines on research datasets, such as ImageNet and CIFAR\n- baselines available for training on your datasets\n- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR (work in progress 🚧).\n- layers available for use in your networks\n- post-processing methods such as temperature scaling\n\n## Installation\n\nThe package can be installed from PyPI:\n\n```sh\npip install torch-uncertainty\n```\n\nTo contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.\n\n## Getting Started and Documentation\n\nPlease find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).\n\nA quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).\n\n## Implemented methods\n\n### Baselines\n\nTo date, the following baselines are implemented:\n\n- Deep Ensembles\n- BatchEnsemble\n- Masksembles\n- Packed-Ensembles (see [blog post](https://medium.com/@adrien.lafage/make-your-neural-networks-more-reliable-with-packed-ensembles-7ad0b737a873))\n\n### Post-processing methods\n\nTo date, the following post-processing methods are implemented:\n\n- Temperature scaling\n\n## Tutorials\n\n## Awesome Uncertainty repositories\n\nYou may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).\n\n## Other References\n\nThis package also contains the official implementation of Packed-Ensembles.\n\nIf you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):\n\n```text\n@inproceedings{laurent2023packed,\n    title={Packed-Ensembles for Efficient Uncertainty Estimation},\n    author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},\n    booktitle={ICLR},\n    year={2023}\n}\n```\n',
     'author': 'ENSTA U2IS',
     'author_email': 'olivier.laurent@ensta-paris.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `torch_uncertainty-0.1.1/PKG-INFO` & `torch_uncertainty-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-uncertainty
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques.
 License: Apache-2.0
 Keywords: deep-learning,pytorch,uncertainty,ensembles,uncertainty-quantification,predictive-uncertainty,reliable-ai,deep-learning-uncertainty
 Author: ENSTA U2IS
 Author-email: olivier.laurent@ensta-paris.fr
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,26 +22,34 @@
 Requires-Dist: torchvision (>=0.14.1,<0.15.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)
 
-[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty) [![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml) [![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/) [![Code Coverage](https://img.shields.io/codecov/c/github/ENSTA-U2IS/torch-uncertainty.svg)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty) [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty)
+[![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml)
+[![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/)
+[![Code Coverage](https://codecov.io/github/ENSTA-U2IS/torch-uncertainty/coverage.svg?branch=master)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 </div>
 
 _TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.
 
+:construction: _TorchUncertainty_ is in early development :construction: - expect massive changes but do reach out to us and contribute if you are interested by the project!
+
 ---
 
 This package provides a multi-level API, including:
+
 - ready-to-train baselines on research datasets, such as ImageNet and CIFAR
 - baselines available for training on your datasets
-- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR.
+- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR (work in progress 🚧).
 - layers available for use in your networks
+- post-processing methods such as temperature scaling
 
 ## Installation
 
 The package can be installed from PyPI:
 
 ```sh
 pip install torch-uncertainty
@@ -51,35 +59,45 @@
 
 ## Getting Started and Documentation
 
 Please find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).
 
 A quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).
 
-## Implemented baselines
+## Implemented methods
+
+### Baselines
 
 To date, the following baselines are implemented:
 
 - Deep Ensembles
+- BatchEnsemble
 - Masksembles
-- Packed-Ensembles
+- Packed-Ensembles (see [blog post](https://medium.com/@adrien.lafage/make-your-neural-networks-more-reliable-with-packed-ensembles-7ad0b737a873))
 
-## Tutorials
+### Post-processing methods
+
+To date, the following post-processing methods are implemented:
 
+- Temperature scaling
+
+## Tutorials
 
 ## Awesome Uncertainty repositories
 
 You may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).
 
 ## Other References
 
 This package also contains the official implementation of Packed-Ensembles.
 
 If you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):
-	
-    @inproceedings{laurent2023packed,
-        title={Packed-Ensembles for Efficient Uncertainty Estimation},
-        author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},
-        booktitle={ICLR},
-        year={2023}
-    }
+
+```text
+@inproceedings{laurent2023packed,
+    title={Packed-Ensembles for Efficient Uncertainty Estimation},
+    author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},
+    booktitle={ICLR},
+    year={2023}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

