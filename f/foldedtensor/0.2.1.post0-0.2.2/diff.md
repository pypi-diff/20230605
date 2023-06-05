# Comparing `tmp/foldedtensor-0.2.1.post0.tar.gz` & `tmp/foldedtensor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldedtensor-0.2.1.post0.tar", last modified: Tue May 23 14:05:18 2023, max compression
+gzip compressed data, was "foldedtensor-0.2.2.tar", last modified: Mon Jun  5 12:41:39 2023, max compression
```

## Comparing `foldedtensor-0.2.1.post0.tar` & `foldedtensor-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-05-23 14:05:18.137484 foldedtensor-0.2.1.post0/
--rw-r--r--   0 perceval   (501) staff       (20)     3889 2023-05-23 14:05:18.137324 foldedtensor-0.2.1.post0/PKG-INFO
--rw-r--r--   0 perceval   (501) staff       (20)     3465 2023-05-23 09:18:36.000000 foldedtensor-0.2.1.post0/README.md
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-05-23 14:05:18.135212 foldedtensor-0.2.1.post0/foldedtensor/
--rw-r--r--   0 perceval   (501) staff       (20)    10171 2023-05-23 14:04:26.000000 foldedtensor-0.2.1.post0/foldedtensor/__init__.py
--rw-r--r--   0 perceval   (501) staff       (20)    10144 2023-05-23 09:18:36.000000 foldedtensor-0.2.1.post0/foldedtensor/functions.cpp
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-05-23 14:05:18.136297 foldedtensor-0.2.1.post0/foldedtensor.egg-info/
--rw-r--r--   0 perceval   (501) staff       (20)     3889 2023-05-23 14:05:18.000000 foldedtensor-0.2.1.post0/foldedtensor.egg-info/PKG-INFO
--rw-r--r--   0 perceval   (501) staff       (20)      306 2023-05-23 14:05:18.000000 foldedtensor-0.2.1.post0/foldedtensor.egg-info/SOURCES.txt
--rw-r--r--   0 perceval   (501) staff       (20)        1 2023-05-23 14:05:18.000000 foldedtensor-0.2.1.post0/foldedtensor.egg-info/dependency_links.txt
--rw-r--r--   0 perceval   (501) staff       (20)       25 2023-05-23 14:05:18.000000 foldedtensor-0.2.1.post0/foldedtensor.egg-info/requires.txt
--rw-r--r--   0 perceval   (501) staff       (20)       48 2023-05-23 14:05:18.000000 foldedtensor-0.2.1.post0/foldedtensor.egg-info/top_level.txt
--rw-r--r--   0 perceval   (501) staff       (20)     1978 2023-05-23 13:57:38.000000 foldedtensor-0.2.1.post0/pyproject.toml
--rw-r--r--   0 perceval   (501) staff       (20)       38 2023-05-23 14:05:18.137535 foldedtensor-0.2.1.post0/setup.cfg
--rw-r--r--   0 perceval   (501) staff       (20)      433 2023-05-15 18:48:04.000000 foldedtensor-0.2.1.post0/setup.py
-drwxr-xr-x   0 perceval   (501) staff       (20)        0 2023-05-23 14:05:18.136933 foldedtensor-0.2.1.post0/tests/
--rw-r--r--   0 perceval   (501) staff       (20)     2587 2023-05-18 12:36:30.000000 foldedtensor-0.2.1.post0/tests/test.py
--rw-r--r--   0 perceval   (501) staff       (20)     6544 2023-05-23 10:31:13.000000 foldedtensor-0.2.1.post0/tests/test_folded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.712626 foldedtensor-0.2.2/foldedtensor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/foldedtensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/foldedtensor/functions.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/foldedtensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-05 12:41:39.000000 foldedtensor-0.2.2/foldedtensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 12:41:39.716626 foldedtensor-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-05 12:41:25.000000 foldedtensor-0.2.2/tests/test_folded_tensor.py
```

### Comparing `foldedtensor-0.2.1.post0/PKG-INFO` & `foldedtensor-0.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-Metadata-Version: 2.1
-Name: foldedtensor
-Version: 0.2.1.post0
-Summary: PyTorch extension for handling deeply nested sequences of variable length
-Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
-Project-URL: homepage, https://github.com/aphp/foldedtensor/
-Project-URL: repository, https://github.com/aphp/foldedtensor/
-Requires-Python: <4.0,>3.7.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 <div align="center">
 <p align="center">
-  <img src="banner.png" width="70%">
+  <img src="https://github.com/aphp/foldedtensor/raw/main/banner.png" width="70%">
 </p>
 </div>
 
 ----
 
 # FoldedTensor: PyTorch extension for handling deeply nested sequences of variable length
```

### Comparing `foldedtensor-0.2.1.post0/foldedtensor/__init__.py` & `foldedtensor-0.2.2/foldedtensor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,39 +16,40 @@
     torch.float64: np.float64,
     torch.complex64: np.complex64,
     torch.complex128: np.complex128,
 }
 
 from . import _C
 
-__version__ = "0.2.1.post0"
+__version__ = "0.2.2"
 
 
 # noinspection PyMethodOverriding
 class Refold(Function):
     @staticmethod
     def forward(
         ctx,
         self: "FoldedTensor",
         dims: Tuple[int],
     ) -> "FoldedTensor":
         ctx.set_materialize_grads(False)
         ctx.lengths = self.lengths
         ctx.old_data_dims = self.data_dims
         ctx.new_data_dims = dims
-        ctx.indexer = self.indexer
+        ctx.input_indexer = self.indexer
 
         device = self.data.device
 
         np_new_indexer, shape_prefix = _C.make_refolding_indexer(
             self.lengths,
             dims,
         )
         data = self.as_tensor()
         indexer = torch.from_numpy(np_new_indexer).to(device)
+        ctx.output_indexer = indexer
         shape_suffix = data.shape[len(self.data_dims) :]
         refolded_data = torch.zeros(
             (*shape_prefix, *shape_suffix), dtype=data.dtype, device=device
         )
         refolded_data.view(-1, *shape_suffix)[indexer] = data.view(
             -1, *shape_suffix
         ).index_select(0, self.indexer)
@@ -65,24 +66,22 @@
         # Perform inverse refolding, i.e., dims = old data_dims
         device = grad_output.device
         # full_names = grad_output.full_names
         np_new_indexer, shape_prefix = _C.make_refolding_indexer(
             ctx.lengths,
             ctx.old_data_dims,
         )
-        indexer = torch.from_numpy(np_new_indexer).to(device)
         # new_data_flat.index_put_({new_indexer}, old_data_flat.index_select(0, old_indexer));
         shape_suffix = grad_output.shape[len(ctx.new_data_dims) :]
         grad_input = torch.zeros(
             (*shape_prefix, *shape_suffix), dtype=grad_output.dtype, device=device
         )
-        index_select = grad_output.reshape(-1, *shape_suffix).index_select(
-            0, ctx.indexer
-        )
-        grad_input.view(-1, *shape_suffix)[indexer] = index_select
+        grad_input.view(-1, *shape_suffix)[ctx.input_indexer] = grad_output.reshape(
+            -1, *shape_suffix
+        ).index_select(0, ctx.output_indexer)
         return grad_input, None
         # return FoldedTensor(
         #     data=refolded_data,
         #     lengths=ctx.lengths,
         #     data_dims=ctx.old_data_dims,
         #     full_names=full_names,
         #     indexer=indexer,
```

### Comparing `foldedtensor-0.2.1.post0/foldedtensor/functions.cpp` & `foldedtensor-0.2.2/foldedtensor/functions.cpp`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.2.1.post0/pyproject.toml` & `foldedtensor-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 dependencies = [
     "torch>1.0.0",
     "numpy",
 ]
 
 [project.optional-dependencies]
 dev = [
+    "black==22.6.0",
+    "pre-commit>=2.18",
+    "pytest==7.1.1",
+    "pytest-cov==3.0.0",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "foldedtensor.__version__" }
 
 [tool.setuptools.packages.find]
 where = ["."]
```

### Comparing `foldedtensor-0.2.1.post0/tests/test_folded_tensor.py` & `foldedtensor-0.2.2/tests/test_folded_tensor.py`

 * *Files identical despite different names*

