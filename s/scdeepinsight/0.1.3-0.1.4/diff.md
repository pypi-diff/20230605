# Comparing `tmp/scdeepinsight-0.1.3.tar.gz` & `tmp/scdeepinsight-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdeepinsight-0.1.3.tar", max compression
+gzip compressed data, was "scdeepinsight-0.1.4.tar", max compression
```

## Comparing `scdeepinsight-0.1.3.tar` & `scdeepinsight-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.3/README.md
--rw-r--r--   0        0        0      558 2023-06-05 14:06:49.573276 scdeepinsight-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4461 2023-06-05 14:06:02.544224 scdeepinsight-0.1.3/scdeepinsight.py
--rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 scdeepinsight-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4090 2023-06-05 13:09:31.912356 scdeepinsight-0.1.4/README.md
+-rw-r--r--   0        0        0      558 2023-06-05 14:34:09.479233 scdeepinsight-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4706 2023-06-05 14:30:51.640224 scdeepinsight-0.1.4/scdeepinsight.py
+-rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 scdeepinsight-0.1.4/PKG-INFO
```

### Comparing `scdeepinsight-0.1.3/README.md` & `scdeepinsight-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `scdeepinsight-0.1.3/pyproject.toml` & `scdeepinsight-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdeepinsight"
-version = "0.1.3"
+version = "0.1.4"
 description = "An automatic cell type annotation tool for PBMC scRNA-seq data."
 authors = ["Shangru JIA <jiashangru@g.ecc.u-tokyo.ac.jp>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `scdeepinsight-0.1.3/scdeepinsight.py` & `scdeepinsight-0.1.4/scdeepinsight.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from torch import nn
 from torchvision import transforms
 from efficientnet_pytorch import EfficientNet
 from torch.utils.data import Dataset
 from PIL import Image
 import scanpy as sc
 
-
 def ImageTransform(query_path:str, barcode_path:str, image_path:str):
     # Input the absoulte path of the target scRNA-seq dataset (end with .h5ad).
     # Assign the absoulte path of the barcode file (end with .csv).
     # Assign the absoulte path of the transformed image file (end with .npy).
     query = anndata.read_h5ad(query_path)
     path = os.path.abspath(__file__) # The installation path.
     folder = os.path.dirname(path)   
@@ -40,14 +39,16 @@
     excluded_genes = list(set(gene_list) - set(genes)) 
     blank_dataframe = pd.DataFrame(np.zeros((len(sample.index.tolist()), len(excluded_genes))))
     blank_dataframe.index = sample.index.tolist()
     blank_dataframe.columns = excluded_genes
     sample = pd.concat([sample, blank_dataframe], axis=1)
     sample = sample[gene_list]
     barcode = pd.DataFrame(sample.index.tolist())
+    barcode["barcode"] = barcode[0].values
+    barcode = barcode.drop(0, axis=1) 
     barcode.to_csv(barcode_path)
     #Image convertion process.
     file = open(Path(prefolder, "img_transformer_pre.obj"),'rb')
     it = pickle.load(file)
     file.close()
     query_img = (it.transform(sample)*255).astype(np.uint8)
     #Store the generated images of the sample query dataset.
@@ -81,15 +82,18 @@
         mod = nn.DataParallel(mod)
 
     mod.to(device)
     mod = mod.to(device)
 
     # Use pre-trained model to predict cell types on the sample query dataset.
     # Input 5: Provided pre-trained model.
-    mod.load_state_dict(torch.load(Path(prefolder, "checkpoint_model_pre.pth")))
+    if (device == 'cpu'):
+        mod.load_state_dict(torch.load(Path(prefolder, "checkpoint_model_pre.pth")))
+    else:
+        mod.load_state_dict(torch.load(Path(prefolder, "checkpoint_model_pre.pth"), map_location=torch.device('cpu')))
     mod.eval()
 
     out = []
     for i, data in enumerate(test_loader):
         query = data
         query = query.to(device)
         pred= mod(query)
@@ -100,9 +104,9 @@
     pr = pred.cpu().numpy()
     file = open(Path(prefolder, "label_encoder_pre.obj"),'rb')
     le = pickle.load(file)
     file.close()
     pred_label = le.inverse_transform(pr)
     pred_label = pd.DataFrame(pred_label)
     barcode = pd.read_csv(barcode_path, index_col=0)
-    pred_label.index = barcode.index.values
+    pred_label.index = barcode["barcode"].values
     return pred_label
```

### Comparing `scdeepinsight-0.1.3/PKG-INFO` & `scdeepinsight-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdeepinsight
-Version: 0.1.3
+Version: 0.1.4
 Summary: An automatic cell type annotation tool for PBMC scRNA-seq data.
 License: MIT
 Author: Shangru JIA
 Author-email: jiashangru@g.ecc.u-tokyo.ac.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

