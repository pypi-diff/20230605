# Comparing `tmp/PVNet-0.0.9.tar.gz` & `tmp/PVNet-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-0.0.9.tar", last modified: Thu May 18 16:08:24 2023, max compression
+gzip compressed data, was "PVNet-0.1.0.tar", last modified: Mon Jun  5 15:21:20 2023, max compression
```

## Comparing `PVNet-0.0.9.tar` & `PVNet-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-18 16:08:10.000000 PVNet-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-18 16:08:10.000000 PVNet-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 16:08:24.583270 PVNet-0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 16:08:24.000000 PVNet-0.0.9/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-18 16:08:10.000000 PVNet-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/pvnet/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/data/datamodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/pvnet/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-05-18 16:08:10.000000 PVNet-0.0.9/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-18 16:08:10.000000 PVNet-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 16:08:10.000000 PVNet-0.0.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-18 16:08:10.000000 PVNet-0.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 16:08:24.583270 PVNet-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-18 16:08:10.000000 PVNet-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:24.583270 PVNet-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:08:10.000000 PVNet-0.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-18 16:08:10.000000 PVNet-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:21:20.698422 PVNet-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 15:21:08.000000 PVNet-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 15:21:08.000000 PVNet-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:21:20.698422 PVNet-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:21:20.698422 PVNet-0.1.0/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 15:21:20.000000 PVNet-0.1.0/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-05 15:21:20.000000 PVNet-0.1.0/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:21:20.000000 PVNet-0.1.0/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-05 15:21:20.000000 PVNet-0.1.0/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 15:21:20.000000 PVNet-0.1.0/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-05 15:21:08.000000 PVNet-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:21:20.698422 PVNet-0.1.0/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 15:21:08.000000 PVNet-0.1.0/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-06-05 15:21:08.000000 PVNet-0.1.0/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-05 15:21:08.000000 PVNet-0.1.0/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 15:21:08.000000 PVNet-0.1.0/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-05 15:21:08.000000 PVNet-0.1.0/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-05 15:21:08.000000 PVNet-0.1.0/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-05 15:21:08.000000 PVNet-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 15:21:08.000000 PVNet-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-05 15:21:08.000000 PVNet-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:21:20.698422 PVNet-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 15:21:08.000000 PVNet-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:21:20.698422 PVNet-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:21:08.000000 PVNet-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-05 15:21:08.000000 PVNet-0.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-05 15:21:08.000000 PVNet-0.1.0/tests/test_app.py
```

### Comparing `PVNet-0.0.9/LICENSE` & `PVNet-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-0.0.9/PKG-INFO` & `PVNet-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.0.9
+Version: 0.1.0
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.0.9/PVNet.egg-info/PKG-INFO` & `PVNet-0.1.0/PVNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.0.9
+Version: 0.1.0
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.0.9/README.md` & `PVNet-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-0.0.9/pvnet/callbacks.py` & `PVNet-0.1.0/pvnet/callbacks.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,129 @@
-"""Custom callbacks developed to be able to use early stopping and learning rate finder even when
-pretraining parts of the network.
+"""Custom callbacks
 """
 from lightning.pytorch import Trainer
 from lightning.pytorch.callbacks import BaseFinetuning, EarlyStopping, LearningRateFinder
 from lightning.pytorch.trainer.states import TrainerFn
 
 
 class PhaseEarlyStopping(EarlyStopping):
+    """Monitor a validation metric and stop training when it stops improving.
+
+    Only functions in a specific phase of training.
+    """
+
     training_phase = None
 
     def switch_phase(self, phase: str):
+        """Switch phase of callback"""
         if phase == self.training_phase:
             self.activate()
         else:
             self.deactivate()
 
     def deactivate(self):
+        """Deactivate callback"""
         self.active = False
 
     def activate(self):
+        """Activate callback"""
         self.active = True
 
     def _should_skip_check(self, trainer: Trainer) -> bool:
         return (
             (trainer.state.fn != TrainerFn.FITTING) or (trainer.sanity_checking) or not self.active
         )
 
 
 class PretrainEarlyStopping(EarlyStopping):
+    """Monitor a validation metric and stop training when it stops improving.
+
+    Only functions in the 'pretrain' phase of training.
+    """
+
     training_phase = "pretrain"
 
 
 class MainEarlyStopping(EarlyStopping):
+    """Monitor a validation metric and stop training when it stops improving.
+
+    Only functions in the 'main' phase of training.
+    """
+
     training_phase = "main"
 
 
 class PretrainFreeze(BaseFinetuning):
+    """Freeze the satellite and NWP encoders during pretraining"""
+
     training_phase = "pretrain"
 
     def __init__(self):
+        """Freeze the satellite and NWP encoders during pretraining"""
         super().__init__()
 
     def freeze_before_training(self, pl_module):
+        """Freeze satellite and NWP encoders before training start"""
         # freeze any module you want
         modules = []
         if pl_module.include_sat:
             modules += [pl_module.sat_encoder]
         if pl_module.include_nwp:
             modules += [pl_module.nwp_encoder]
         self.freeze(modules)
 
     def finetune_function(self, pl_module, current_epoch, optimizer):
+        """Unfreeze satellite and NWP encoders"""
         if not self.active:
             modules = []
             if pl_module.include_sat:
                 modules += [pl_module.sat_encoder]
             if pl_module.include_nwp:
                 modules += [pl_module.nwp_encoder]
             self.unfreeze_and_add_param_group(
                 modules=modules,
                 optimizer=optimizer,
                 train_bn=True,
             )
 
     def switch_phase(self, phase: str):
+        """Switch phase of callback"""
         if phase == self.training_phase:
             self.activate()
         else:
             self.deactivate()
 
     def deactivate(self):
+        """Deactivate callback"""
         self.active = False
 
     def activate(self):
+        """Activate callback"""
         self.active = True
 
 
 class PhasedLearningRateFinder(LearningRateFinder):
     """Finds a learning rate at the start of each phase of learning"""
 
     active = True
 
     def on_fit_start(self, *args, **kwargs):
+        """Do nothing"""
         return
 
     def on_train_epoch_start(self, trainer, pl_module):
+        """Run learning rate finder on epoch start and then deactivate"""
         if self.active:
             self.lr_find(trainer, pl_module)
             self.deactivate()
 
     def switch_phase(self, phase: str):
+        """Switch training phase"""
         self.activate()
 
     def deactivate(self):
+        """Deactivate callback"""
         self.active = False
 
     def activate(self):
+        """Activate callback"""
         self.active = True
```

### Comparing `PVNet-0.0.9/pvnet/optimizers.py` & `PVNet-0.1.0/pvnet/optimizers.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,56 +3,71 @@
 
 from abc import ABC, abstractmethod
 
 import torch
 
 
 class AbstractOptimizer(ABC):
-    """Optimizer classes will be used by model like:
+    """Abstract class for optimizer
+
+    Optimizer classes will be used by model like:
     > OptimizerGenerator = AbstractOptimizer()
     > optimizer = OptimizerGenerator(model.parameters())
     The returned object `optimizer` must be something that may be returned by `pytorch_lightning`'s
     `configure_optimizers()` method.
     See :
         https://lightning.ai/docs/pytorch/stable/common/lightning_module.html#configure-optimizers
 
     """
 
     @abstractmethod
     def __call__(self):
+        """Abstract call"""
         pass
 
 
 class Adam(AbstractOptimizer):
+    """Adam optimizer"""
+
     def __init__(self, lr=0.0005, **kwargs):
+        """Adam optimizer"""
         self.lr = lr
         self.kwargs = kwargs
 
     def __call__(self, model_parameters):
+        """Return optimizer"""
         return torch.optim.Adam(model_parameters, lr=self.lr, **self.kwargs)
 
 
 class AdamW(AbstractOptimizer):
+    """AdamW optimizer"""
+
     def __init__(self, lr=0.0005, **kwargs):
+        """AdamW optimizer"""
         self.lr = lr
         self.kwargs = kwargs
 
     def __call__(self, model_parameters):
+        """Return optimizer"""
         return torch.optim.AdamW(model_parameters, lr=self.lr, **self.kwargs)
 
 
 class AdamWReduceLROnPlateau(AbstractOptimizer):
+    """AdamW optimizer and reduce on plateau scheduler"""
+
     def __init__(self, lr=0.0005, patience=3, factor=0.5, threshold=2e-4, **opt_kwargs):
+        """AdamW optimizer and reduce on plateau scheduler"""
         self.lr = lr
         self.patience = patience
         self.factor = factor
         self.threshold = threshold
         self.opt_kwargs = opt_kwargs
 
     def __call__(self, model_parameters):
+        """Return optimizer"""
         opt = torch.optim.AdamW(model_parameters, lr=self.lr, **self.opt_kwargs)
         sch = torch.optim.lr_scheduler.ReduceLROnPlateau(
             opt,
             factor=self.factor,
             patience=self.patience,
             threshold=self.threshold,
         )
```

### Comparing `PVNet-0.0.9/pvnet/training.py` & `PVNet-0.1.0/pvnet/training.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+"""Training"""
+import os
 from typing import Optional
 
 import hydra
 import torch
 from lightning.pytorch import (
     Callback,
     LightningDataModule,
     LightningModule,
     Trainer,
     seed_everything,
 )
+from lightning.pytorch.callbacks import ModelCheckpoint
 from lightning.pytorch.loggers import Logger
-from omegaconf import DictConfig
+from lightning.pytorch.loggers.wandb import WandbLogger
+from omegaconf import DictConfig, OmegaConf
 
 from pvnet import utils
 
 log = utils.get_logger(__name__)
 
 torch.set_default_dtype(torch.float32)
 
 
-def callbacks_to_phase(callbacks, phase):
+def _callbacks_to_phase(callbacks, phase):
     for c in callbacks:
         if hasattr(c, "switch_phase"):
             c.switch_phase(phase)
 
 
 def train(config: DictConfig) -> Optional[float]:
     """Contains training pipeline.
+
     Instantiates all PyTorch Lightning objects from config.
 
     Args:
         config (DictConfig): Configuration composed by Hydra.
 
     Returns:
         Optional[float]: Metric score for hyperparameter optimization.
@@ -45,49 +50,72 @@
     datamodule: LightningDataModule = hydra.utils.instantiate(config.datamodule)
 
     # Init lightning model
     log.info(f"Instantiating model <{config.model._target_}>")
     model: LightningModule = hydra.utils.instantiate(config.model)
 
     # Init lightning loggers
-    logger: list[Logger] = []
+    loggers: list[Logger] = []
     if "logger" in config:
         for _, lg_conf in config.logger.items():
             if "_target_" in lg_conf:
                 log.info(f"Instantiating logger <{lg_conf._target_}>")
-                logger.append(hydra.utils.instantiate(lg_conf))
+                loggers.append(hydra.utils.instantiate(lg_conf))
 
     # Init lightning callbacks
     callbacks: list[Callback] = []
     if "callbacks" in config:
         for _, cb_conf in config.callbacks.items():
             if "_target_" in cb_conf:
                 log.info(f"Instantiating callback <{cb_conf._target_}>")
                 callbacks.append(hydra.utils.instantiate(cb_conf))
 
+    # Align the wandb id with the checkpoint path
+    # - only works if wandb logger and model checkpoint used
+    # - this makes it easy to push the model to huggingface
+    use_wandb_logger = False
+    for logger in loggers:
+        log.info(f"{logger}")
+        if isinstance(logger, WandbLogger):
+            use_wandb_logger = True
+            wandb_logger = logger
+            break
+
+    if use_wandb_logger:
+        for callback in callbacks:
+            log.info(f"{callback}")
+            if isinstance(callback, ModelCheckpoint):
+                callback.dirpath = "/".join(
+                    callback.dirpath.split("/")[:-1] + [wandb_logger.version]
+                )
+                # Also save model config here - this makes for easy model push to huggingface
+                os.makedirs(callback.dirpath, exist_ok=True)
+                OmegaConf.save(config.model, f"{callback.dirpath}/model_config.yaml")
+                break
+
     should_pretrain = False
     for c in callbacks:
         should_pretrain |= hasattr(c, "training_phase") and c.training_phase == "pretrain"
 
     if should_pretrain:
-        callbacks_to_phase(callbacks, "pretrain")
+        _callbacks_to_phase(callbacks, "pretrain")
 
     trainer: Trainer = hydra.utils.instantiate(
         config.trainer,
-        logger=logger,
+        logger=loggers,
         _convert_="partial",
         callbacks=callbacks,
     )
 
     if should_pretrain:
         # Pre-train the model
         datamodule.block_nwp_and_sat = True
         trainer.fit(model=model, datamodule=datamodule)
 
-    callbacks_to_phase(callbacks, "main")
+    _callbacks_to_phase(callbacks, "main")
 
     datamodule.block_nwp_and_sat = False
     trainer.should_stop = False
 
     # Train the model completely
     trainer.fit(model=model, datamodule=datamodule)
```

### Comparing `PVNet-0.0.9/pvnet/utils.py` & `PVNet-0.1.0/pvnet/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+"""Utils"""
 import logging
 import os
 import warnings
 from collections.abc import Sequence
 
+import lightning.pytorch as pl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import pytorch_lightning as pl
 import rich.syntax
 import rich.tree
+import xarray as xr
 import yaml
-from ocf_datapipes.utils.consts import BatchKey
+from lightning.pytorch.loggers import Logger
+from lightning.pytorch.utilities import rank_zero_only
+from ocf_datapipes.utils.consts import BatchKey, Location
 from ocf_datapipes.utils.geospatial import osgb_to_lat_lon
 from omegaconf import DictConfig, OmegaConf
-from pytorch_lightning.loggers import Logger
-from pytorch_lightning.utilities import rank_zero_only
 
 import pvnet
 
 
 def load_config(config_file):
     """
     Open yam configruation file, and get rid eof '_target_' line
@@ -55,16 +57,45 @@
         "critical",
     ):
         setattr(logger, level, rank_zero_only(getattr(logger, level)))
 
     return logger
 
 
+class GSPLocationLookup:
+    """Query object for GSP location from GSP ID"""
+
+    def __init__(self, x_osgb: xr.DataArray, y_osgb: xr.DataArray):
+        """Query object for GSP location from GSP ID
+
+        Args:
+            x_osgb: DataArray of the OSGB x-coordinate for any given GSP ID
+            y_osgb: DataArray of the OSGB y-coordinate for any given GSP ID
+
+        """
+        self.x_osgb = x_osgb
+        self.y_osgb = y_osgb
+
+    def __call__(self, gsp_id: int) -> Location:
+        """Returns the locations for the input GSP IDs.
+
+        Args:
+            gsp_id: Integer ID of the GSP
+        """
+        return Location(
+            x=self.x_osgb.sel(gsp_id=gsp_id).item(),
+            y=self.y_osgb.sel(gsp_id=gsp_id).item(),
+            id=gsp_id,
+        )
+
+
 def extras(config: DictConfig) -> None:
-    """A couple of optional utilities, controlled by main config file:
+    """A couple of optional utilities.
+
+    Controlled by main config file:
     - disabling warnings
     - easier access to debug mode
     - forcing debug friendly configuration
 
     Modifies DictConfig in place.
 
     Args:
@@ -139,14 +170,15 @@
     rich.print(tree)
 
     with open("config_tree.txt", "w") as fp:
         rich.print(tree, file=fp)
 
 
 def empty(*args, **kwargs):
+    """Returns nothing"""
     pass
 
 
 @rank_zero_only
 def log_hyperparameters(
     config: DictConfig,
     model: pl.LightningModule,
@@ -205,14 +237,16 @@
         if isinstance(lg, pl.loggers.wandb.WandbLogger):
             import wandb
 
             wandb.finish()
 
 
 def plot_batch_forecasts(batch, y_hat, batch_idx=None):
+    """Plot a batch of data and the forecast from that batch"""
+
     def _get_numpy(key):
         return batch[key].cpu().numpy().squeeze()
 
     y = batch[BatchKey.gsp].cpu().numpy()
     y_hat = y_hat.cpu().numpy()
 
     gsp_ids = batch[BatchKey.gsp_id].cpu().numpy().squeeze()
@@ -250,14 +284,16 @@
     plt.suptitle(title)
     plt.tight_layout()
 
     return fig
 
 
 def construct_ocf_ml_metrics_batch_df(batch, y, y_hat):
+    """Helper function tot construct DataFrame for ocf_ml_metrics"""
+
     def _repeat(x):
         return np.repeat(x.squeeze(), n_times)
 
     def _get_numpy(key):
         return batch[key].cpu().numpy().squeeze()
 
     t0_idx = batch[BatchKey.gsp_t0_idx]
```

### Comparing `PVNet-0.0.9/setup.py` & `PVNet-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,24 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 install_requires = (this_directory / "requirements.txt").read_text().splitlines()
 extras_require = {"all_models": ["pytorch-tabnet", "efficientnet_pytorch"]}
 
+with open("pvnet/__init__.py") as f:
+    for line in f:
+        if line.startswith("__version__"):
+            _, _, version = line.replace("'", "").split()
+            version = version.replace('"', "")
+
+
 setup(
     name="PVNet",
-    version="0.0.9",
+    version=version,
     license="MIT",
     description="PVNet",
     author="Peter Dudfield",
     author_email="info@openclimatefix.org",
     company="Open Climate Fix Ltd",
     install_requires=install_requires,
     extras_require=extras_require,
```

