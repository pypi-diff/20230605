# Comparing `tmp/pyspacer-0.3.1.tar.gz` & `tmp/pyspacer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyspacer-0.3.1.tar", last modified: Tue Nov 10 05:48:47 2020, max compression
+gzip compressed data, was "pyspacer-0.4.0.tar", last modified: Fri May  5 06:55:27 2023, max compression
```

## Comparing `pyspacer-0.3.1.tar` & `pyspacer-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 beijbom    (502) staff       (20)        0 2020-11-10 05:48:47.000000 pyspacer-0.3.1/
--rw-r--r--   0 beijbom    (502) staff       (20)     4371 2020-11-10 05:48:47.000000 pyspacer-0.3.1/PKG-INFO
-drwxr-xr-x   0 beijbom    (502) staff       (20)        0 2020-11-10 05:48:47.000000 pyspacer-0.3.1/spacer/
--rw-r--r--   0 beijbom    (502) staff       (20)     4547 2020-11-10 05:00:49.000000 pyspacer-0.3.1/spacer/tasks.py
--rw-r--r--   0 beijbom    (502) staff       (20)     8327 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/train_utils.py
--rw-r--r--   0 beijbom    (502) staff       (20)     5899 2020-10-25 02:59:31.000000 pyspacer-0.3.1/spacer/config.py
--rw-r--r--   0 beijbom    (502) staff       (20)     5931 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/extract_features.py
--rw-r--r--   0 beijbom    (502) staff       (20)       21 2020-02-28 16:53:56.000000 pyspacer-0.3.1/spacer/__init__.py
-drwxr-xr-x   0 beijbom    (502) staff       (20)        0 2020-11-10 05:48:47.000000 pyspacer-0.3.1/spacer/models/
--rw-r--r--   0 beijbom    (502) staff       (20)      405 2020-05-05 04:49:28.000000 pyspacer-0.3.1/spacer/models/__init__.py
--rw-r--r--   0 beijbom    (502) staff       (20)     9854 2020-05-05 04:49:28.000000 pyspacer-0.3.1/spacer/models/efficientnet.py
--rw-r--r--   0 beijbom    (502) staff       (20)    10959 2020-05-05 04:49:28.000000 pyspacer-0.3.1/spacer/models/effcientnet_utils.py
--rw-r--r--   0 beijbom    (502) staff       (20)     4573 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/caffe_utils.py
--rw-r--r--   0 beijbom    (502) staff       (20)     1736 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/extract_features_utils.py
--rw-r--r--   0 beijbom    (502) staff       (20)     7376 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/storage.py
--rw-r--r--   0 beijbom    (502) staff       (20)    17103 2020-10-22 16:36:28.000000 pyspacer-0.3.1/spacer/messages.py
--rw-r--r--   0 beijbom    (502) staff       (20)      840 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/task_utils.py
--rw-r--r--   0 beijbom    (502) staff       (20)     2690 2020-09-27 15:09:24.000000 pyspacer-0.3.1/spacer/train_classifier.py
--rw-r--r--   0 beijbom    (502) staff       (20)     2570 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/mailman.py
--rw-r--r--   0 beijbom    (502) staff       (20)    10880 2020-11-10 05:43:14.000000 pyspacer-0.3.1/spacer/data_classes.py
--rw-r--r--   0 beijbom    (502) staff       (20)     2809 2020-10-20 03:26:25.000000 pyspacer-0.3.1/spacer/torch_utils.py
-drwxr-xr-x   0 beijbom    (502) staff       (20)        0 2020-11-10 05:48:47.000000 pyspacer-0.3.1/pyspacer.egg-info/
--rw-r--r--   0 beijbom    (502) staff       (20)     4371 2020-11-10 05:48:46.000000 pyspacer-0.3.1/pyspacer.egg-info/PKG-INFO
--rw-r--r--   0 beijbom    (502) staff       (20)      572 2020-11-10 05:48:46.000000 pyspacer-0.3.1/pyspacer.egg-info/SOURCES.txt
--rw-r--r--   0 beijbom    (502) staff       (20)      140 2020-11-10 05:48:46.000000 pyspacer-0.3.1/pyspacer.egg-info/requires.txt
--rw-r--r--   0 beijbom    (502) staff       (20)        7 2020-11-10 05:48:46.000000 pyspacer-0.3.1/pyspacer.egg-info/top_level.txt
--rw-r--r--   0 beijbom    (502) staff       (20)        1 2020-11-10 05:48:46.000000 pyspacer-0.3.1/pyspacer.egg-info/dependency_links.txt
--rw-r--r--   0 beijbom    (502) staff       (20)     3215 2020-11-10 05:04:55.000000 pyspacer-0.3.1/README.md
--rw-r--r--   0 beijbom    (502) staff       (20)     1328 2020-11-10 05:48:39.000000 pyspacer-0.3.1/setup.py
--rw-r--r--   0 beijbom    (502) staff       (20)       38 2020-11-10 05:48:47.000000 pyspacer-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.765171 pyspacer-0.4.0/
+-rw-rw-rw-   0        0        0      320 2023-05-05 06:55:07.000000 pyspacer-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5595 2023-05-05 06:55:27.762179 pyspacer-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3764 2023-03-22 02:10:27.000000 pyspacer-0.4.0/README.md
+-rw-rw-rw-   0        0        0     1073 2023-01-18 22:46:34.000000 pyspacer-0.4.0/license.txt
+-rw-rw-rw-   0        0        0      754 2023-05-05 06:35:48.000000 pyspacer-0.4.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.727298 pyspacer-0.4.0/pyspacer.egg-info/
+-rw-rw-rw-   0        0        0     5595 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 06:55:27.000000 pyspacer-0.4.0/pyspacer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:55:27.765171 pyspacer-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.755202 pyspacer-0.4.0/spacer/
+-rw-rw-rw-   0        0        0       21 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/__init__.py
+-rw-rw-rw-   0        0        0     4570 2023-01-23 20:13:32.000000 pyspacer-0.4.0/spacer/caffe_utils.py
+-rw-rw-rw-   0        0        0     5274 2023-04-27 05:43:33.000000 pyspacer-0.4.0/spacer/config.py
+-rw-rw-rw-   0        0        0    10871 2023-01-23 20:13:32.000000 pyspacer-0.4.0/spacer/data_classes.py
+-rw-rw-rw-   0        0        0      271 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/exceptions.py
+-rw-rw-rw-   0        0        0     5931 2023-04-25 04:49:47.000000 pyspacer-0.4.0/spacer/extract_features.py
+-rw-rw-rw-   0        0        0     1573 2023-01-25 01:02:22.000000 pyspacer-0.4.0/spacer/extract_features_utils.py
+-rw-rw-rw-   0        0        0     2718 2023-04-20 05:31:47.000000 pyspacer-0.4.0/spacer/mailman.py
+-rw-rw-rw-   0        0        0    17105 2023-04-25 04:49:47.000000 pyspacer-0.4.0/spacer/messages.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:55:27.760210 pyspacer-0.4.0/spacer/models/
+-rw-rw-rw-   0        0        0      405 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/models/__init__.py
+-rw-rw-rw-   0        0        0    10959 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/models/effcientnet_utils.py
+-rw-rw-rw-   0        0        0     9854 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/models/efficientnet.py
+-rw-rw-rw-   0        0        0    10695 2023-04-15 21:20:49.000000 pyspacer-0.4.0/spacer/storage.py
+-rw-rw-rw-   0        0        0      840 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/task_utils.py
+-rw-rw-rw-   0        0        0     4547 2023-01-19 01:13:55.000000 pyspacer-0.4.0/spacer/tasks.py
+-rw-rw-rw-   0        0        0     2809 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/torch_utils.py
+-rw-rw-rw-   0        0        0     2690 2023-01-18 22:46:34.000000 pyspacer-0.4.0/spacer/train_classifier.py
+-rw-rw-rw-   0        0        0     8837 2023-01-24 22:36:53.000000 pyspacer-0.4.0/spacer/train_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyspacer-0.3.1/spacer/tasks.py` & `pyspacer-0.4.0/spacer/tasks.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.3.1/spacer/train_utils.py` & `pyspacer-0.4.0/spacer/train_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if clf_type == 'MLP':
             if len(train_set) * labels.samples_per_image >= 50000:
                 hls, lr = (200, 100), 1e-4
             else:
                 hls, lr = (100,), 1e-3
             clf = MLPClassifier(hidden_layer_sizes=hls, learning_rate_init=lr)
         else:
-            clf = SGDClassifier(loss='log', average=True, random_state=0)
+            clf = SGDClassifier(loss='log_loss', average=True, random_state=0)
         ref_acc = []
         for epoch in range(nbr_epochs):
             np.random.shuffle(train_set)
             mini_batches = chunkify(train_set, batches_per_epoch)
             for mb in mini_batches:
                 x, y = load_batch_data(labels, mb, classes, feature_loc)
                 clf.partial_fit(x, y, classes=classes)
@@ -132,16 +132,25 @@
     feature_loc.key = imkey  # Set the relevant key here.
     image_features = ImageFeatures.load(feature_loc)
 
     # Load row, col, labels for this image.
     image_labels = labels.data[imkey]
 
     # Sanity check
-    assert len(image_labels) == len(image_features.point_features), \
-        "number of extracted features doesn't match the number of labels!"
+    if image_features.valid_rowcol:
+        # With new data structure just check that the sets of row, col
+        # given by the labels is available in the features.
+        rc_features_set = set([(pf.row, pf.col) for pf in
+                               image_features.point_features])
+        rc_labels_set = set([(row, col) for (row, col, _) in image_labels])
+        assert rc_labels_set.issubset(rc_features_set)
+    else:
+        # With legacy data structure check that length is the same.
+        assert len(image_labels) == len(image_features.point_features), \
+            "number of extracted features doesn't match the number of labels!"
 
     x, y = [], []
     if image_features.valid_rowcol:
         for row, col, label in image_labels:
             if label not in classes:
                 # Remove samples for which the label is not in classes.
                 continue
```

### Comparing `pyspacer-0.3.1/spacer/config.py` & `pyspacer-0.4.0/spacer/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,15 @@
 import time
 import warnings
 from contextlib import ContextDecorator
 from typing import Tuple, Optional
 
 import boto3
 import botocore.exceptions
-from PIL import Image
-
-# Configure a simple logger that works with AWS cloudwatch
-if len(logging.getLogger().handlers) > 0:
-    # The Lambda environment pre-configures a handler logging to stderr.
-    # If a handler is already configured,
-    # `.basicConfig` does not execute. Thus we set the level directly.
-    logging.getLogger().setLevel(logging.INFO)
-else:
-    logging.basicConfig(level=logging.INFO, format='%(asctime)s %(message)s')
+from PIL import Image, ImageFile
 
 
 def filter_warnings():
     """ Filters out some verified warnings. """
 
     # Per discussion in https://github.com/boto/boto3/issues/454,
     # the boto package is raising a lot of warnings that it shouldn't.
@@ -77,28 +68,14 @@
 
     return boto3.resource('s3',
                           region_name="us-west-2",
                           aws_access_key_id=aws_key_id,
                           aws_secret_access_key=aws_key_secret)
 
 
-def get_sqs_conn():
-    """
-    Returns a connection to SQS.
-    - It first looks for credentials in the environmental vars.
-    - If not found there it looks in secrets.json
-    - If not found there it will default to credentials in ~/.aws/credentials
-    """
-    aws_key_id, aws_key_secret = get_aws_credentials()
-    return boto3.resource('sqs',
-                          region_name="us-west-2",
-                          aws_access_key_id=aws_key_id,
-                          aws_secret_access_key=aws_key_secret)
-
-
 def get_local_model_path():
     local_model_path = os.getenv('SPACER_LOCAL_MODEL_PATH')
     if local_model_path is None:
         return get_secret('SPACER_LOCAL_MODEL_PATH')  # pragma: no cover
     return local_model_path
 
 
@@ -117,14 +94,17 @@
 
 
 LOCAL_MODEL_PATH = get_local_model_path()
 
 HAS_LOCAL_MODEL_PATH = LOCAL_MODEL_PATH is not None and \
                        os.path.exists(LOCAL_MODEL_PATH)
 
+# Filesystem dir to use for temporary files from unit tests and downloads.
+TMP_PATH = get_secret('TMP_PATH') or 'tmp'
+
 TASKS = [
     'extract_features',
     'train_classifier',
     'classify_features',
     'classify_image'
 ]
 
@@ -191,7 +171,12 @@
         botocore.exceptions.NoCredentialsError):  # pragma: no cover
     logging.info("No connection to spacer-tools bucket, "
                  "can't run remote tests")
     HAS_S3_MODEL_ACCESS = False
 
 # Add margin to avoid warnings when running unit-test.
 Image.MAX_IMAGE_PIXELS = MAX_IMAGE_PIXELS + 20000
+
+# Configure Pillow to be tolerant of image files that are truncated (missing
+# data from the last block).
+# https://stackoverflow.com/a/23575424/
+ImageFile.LOAD_TRUNCATED_IMAGES = True
```

### Comparing `pyspacer-0.3.1/spacer/extract_features.py` & `pyspacer-0.4.0/spacer/extract_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 class VGG16CaffeExtractor(FeatureExtractor):
 
     def __init__(self):
 
         # Cache models and prototxt locally.
         self.modeldef_path, _ = download_model(
             'vgg16_coralnet_ver1.deploy.prototxt')
-        self.modelweighs_path, self.model_was_cashed = download_model(
+        self.modelweighs_path, self.model_was_cached = download_model(
             'vgg16_coralnet_ver1.caffemodel')
 
     def __call__(self, im, rowcols):
 
         # We should only reach this line if it is confirmed caffe is available
         from spacer.caffe_utils import classify_from_patchlist
 
@@ -101,29 +101,29 @@
                                               col=rc[1],
                                               data=ft.tolist())
                                 for rc, ft in zip(rowcols, feats)],
                 valid_rowcol=True,
                 feature_dim=len(feats[0]),
                 npoints=len(feats)
             ), ExtractFeaturesReturnMsg(
-                model_was_cashed=self.model_was_cashed,
+                model_was_cached=self.model_was_cached,
                 runtime=time.time() - start_time
             )
 
     @property
     def feature_dim(self):
         return 4096
 
 
 class EfficientNetExtractor(FeatureExtractor):
 
     def __init__(self):
 
         # Cache models locally.
-        self.modelweighs_path, self.model_was_cashed = download_model(
+        self.modelweighs_path, self.model_was_cached = download_model(
            'efficientnet_b0_ver1.pt')
 
     def __call__(self, im, rowcols):
 
         start_time = time.time()
 
         # Set torch parameters
@@ -143,15 +143,15 @@
         feats = extract_feature(patch_list, torch_params)
 
         return ImageFeatures(
             point_features=[PointFeatures(row=rc[0], col=rc[1], data=ft)
                             for rc, ft in zip(rowcols, feats)],
             valid_rowcol=True, feature_dim=len(feats[0]), npoints=len(feats)
         ), ExtractFeaturesReturnMsg(
-            model_was_cashed=self.model_was_cashed,
+            model_was_cached=self.model_was_cached,
             runtime=time.time() - start_time
         )
 
     @property
     def feature_dim(self):
         return 1280
```

### Comparing `pyspacer-0.3.1/spacer/models/efficientnet.py` & `pyspacer-0.4.0/spacer/models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.3.1/spacer/models/effcientnet_utils.py` & `pyspacer-0.4.0/spacer/models/effcientnet_utils.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.3.1/spacer/caffe_utils.py` & `pyspacer-0.4.0/spacer/caffe_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             for i in range(batch_size):
                 pos = b * batch_size + i
                 if pos < len(im_list):
                     net.blobs['data'].data[i, :, :, :] = \
                         transformer.preprocess(im_list[pos])
             net.forward(start=startlayer)
             scorelist.extend(list(copy(net.blobs[scorelayer].data).
-                                  astype(np.float)))
+                                  astype(float)))
 
         scorelist = scorelist[:len(im_list)]
 
     return scorelist
 
 
 @lru_cache(maxsize=1)
```

### Comparing `pyspacer-0.3.1/spacer/messages.py` & `pyspacer-0.4.0/spacer/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,24 +95,24 @@
         )
 
 
 class ExtractFeaturesReturnMsg(DataClass):
     """ Return message for extract_features task. """
 
     def __init__(self,
-                 model_was_cashed: bool,
+                 model_was_cached: bool,
                  runtime: float):
 
-        self.model_was_cashed = model_was_cashed
+        self.model_was_cached = model_was_cached
         self.runtime = runtime
 
     @classmethod
     def example(cls) -> 'ExtractFeaturesReturnMsg':
         return ExtractFeaturesReturnMsg(
-            model_was_cashed=True,
+            model_was_cached=True,
             runtime=2.1
         )
 
 
 class TrainClassifierMsg(DataClass):
     """ Specifies the train classifier task. """
 
@@ -237,20 +237,20 @@
         self.classifier_loc = classifier_loc
 
     @classmethod
     def example(cls):
         return ClassifyFeaturesMsg(
             job_token='my_job',
             feature_loc=DataLocation(storage_type='url',
-                                     key='https://spacer-test.s3-us-west-2.'
-                                         'amazonaws.com/08bfc10v7t.png.'
+                                     key='https://my-bucket.s3-my-region.'
+                                         'amazonaws.com/01234aeiou.png.'
                                          'featurevector'),
             classifier_loc=DataLocation(storage_type='url',
-                                        key='https://spacer-test.s3-us-west-2.'
-                                        'amazonaws.com/legacy.model')
+                                        key='https://my-bucket.s3-my-region.'
+                                        'amazonaws.com/my_model_id.model')
         )
 
     def serialize(self):
         return {
             'job_token': self.job_token,
             'feature_loc': self.feature_loc.serialize(),
             'classifier_loc': self.classifier_loc.serialize(),
@@ -282,21 +282,21 @@
         self.classifier_loc = classifier_loc
 
     @classmethod
     def example(cls):
         return ClassifyImageMsg(
             job_token='my_job',
             image_loc=DataLocation(storage_type='url',
-                                   key='https://spacer-test.s3-us-west-2.'
-                                   'amazonaws.com/08bfc10v7t.png'),
+                                   key='https://my-bucket.s3-my-region.'
+                                   'amazonaws.com/01234aeiou.png'),
             feature_extractor_name='vgg16_coralnet_ver1',
             rowcols=[(1, 1), (2, 2)],
             classifier_loc=DataLocation(storage_type='url',
-                                        key='https://spacer-test.s3-us-west-2.'
-                                        'amazonaws.com/legacy.model')
+                                        key='https://my-bucket.s3-my-region.'
+                                        'amazonaws.com/my_model_id.model')
         )
 
     def serialize(self):
         return {
             'job_token': self.job_token,
             'image_loc': self.image_loc.serialize(),
             'feature_extractor_name': self.feature_extractor_name,
```

### Comparing `pyspacer-0.3.1/spacer/task_utils.py` & `pyspacer-0.4.0/spacer/task_utils.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.3.1/spacer/train_classifier.py` & `pyspacer-0.4.0/spacer/train_classifier.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.3.1/spacer/mailman.py` & `pyspacer-0.4.0/spacer/mailman.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 """
-Defines the highest-level method for task handling through AWS SQS.
+Defines the highest-level method for task handling through AWS Batch.
 """
 
 import json
 import logging
 import os
 
 import fire
 
 from spacer import config
 from spacer.messages import JobMsg, DataLocation
-from spacer.tasks import \
-    process_job
+from spacer.tasks import process_job
+
+
+# Configure a simple logger that works with AWS CloudWatch.
+if len(logging.getLogger().handlers) > 0:
+    # The Lambda environment pre-configures a handler logging to stderr.
+    # If a handler is already configured,
+    # `.basicConfig` does not execute. Thus we set the level directly.
+    logging.getLogger().setLevel(logging.INFO)
+else:
+    logging.basicConfig(level=logging.INFO, format='%(asctime)s %(message)s')
 
 
 def env_job(): # pragma: no cover
-    """ Runs a job defined in environmental variables. Setup to play
-    nicely with AWS Batch.
-    Expects JOB_MSG_LOC to contain the json-serialized DataLocation of JobMgs.
-    Expects OUT_QUEUE to contain the name of the desired results queue.
+    """
+    Runs a job defined in environment variables.
+    This is set up to be used in AWS Batch, using a job definition with
+    a command such as: ["python3","spacer/mailman.py","env_job"]
+
+    Expects JOB_MSG_LOC to contain the json-serialized DataLocation of the
+    job msg.
+    Expects RES_MSG_LOC to contain the json-serialized DataLocation of the
+    job return msg.
     """
 
     job_msg_loc = os.getenv('JOB_MSG_LOC')
     if job_msg_loc is None:
         raise ValueError('JOB_MSG_LOC env. variable not set. '
                          'Can not process job.')
 
@@ -44,23 +58,14 @@
             'original_job': job_msg.serialize(),
             'ok': False,
             'results': None,
             'error_message': 'Error deserializing message: ' + repr(e)
         }
 
     # Return
-    out_queue_name = os.getenv('RES_SQS_QUEUE')
-    if out_queue_name is not None:
-        with config.log_entry_and_exit('writing results to {}'.format(
-                out_queue_name)):
-            conn = config.get_sqs_conn()
-            out_queue = conn.get_queue(out_queue_name)
-            m_out = out_queue.new_message(body=json.dumps(job_return_msg_dict))
-            out_queue.write(m_out)
-
     out_msg_loc = os.getenv('RES_MSG_LOC')
     if out_msg_loc is not None:
         with config.log_entry_and_exit('out message location deserialization'):
             out_msg_loc = DataLocation.deserialize(json.loads(out_msg_loc))
 
         with config.log_entry_and_exit('writing res to {}'.format(
                 out_msg_loc.key)):
```

### Comparing `pyspacer-0.3.1/spacer/data_classes.py` & `pyspacer-0.4.0/spacer/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,22 @@
     def __init__(self,
                  row: Optional[int],  # Row where feature was extracted
                  col: Optional[int],  # Column where feature was extracted
                  data: np.array,  # Feature vector with 32 bit precision.
                  ):
         self.row = row
         self.col = col
-        self.data = np.array(data, dtype=np.float)
+        self.data = np.array(data, dtype=float)
 
     @classmethod
     def example(cls):
         return cls(
             row=100,
             col=100,
-            data=np.array([1.1, 1.3, 1.12], dtype=np.float)
+            data=np.array([1.1, 1.3, 1.12], dtype=float)
         )
 
     def __eq__(self, other):
         return self.row == other.row and self.col == other.col and \
                np.allclose(self.data, other.data)
 
 
@@ -260,15 +260,15 @@
         storage = storage_factory(loc.storage_type, loc.bucket_name)
         if self.valid_rowcol:
             rows = np.array([p.row for p in self.point_features], dtype=np.uint16)
             cols = np.array([p.col for p in self.point_features], dtype=np.uint16)
         else:
             rows = np.array([])
             cols = np.array([])
-        feat = np.array([p.data for p in self.point_features], dtype=np.float)
+        feat = np.array([p.data for p in self.point_features], dtype=float)
         meta = np.array([self.valid_rowcol, self.npoints, self.feature_dim])
         output = BytesIO()
         np.savez_compressed(output, meta=meta, rows=rows, cols=cols, feat=feat)
         output.seek(0)
         storage.store(loc.key, output)
```

### Comparing `pyspacer-0.3.1/spacer/torch_utils.py` & `pyspacer-0.4.0/spacer/torch_utils.py`

 * *Files identical despite different names*

### Comparing `pyspacer-0.3.1/pyspacer.egg-info/SOURCES.txt` & `pyspacer-0.4.0/pyspacer.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+MANIFEST.in
 README.md
-setup.py
+license.txt
+pyproject.toml
 pyspacer.egg-info/PKG-INFO
 pyspacer.egg-info/SOURCES.txt
 pyspacer.egg-info/dependency_links.txt
 pyspacer.egg-info/requires.txt
 pyspacer.egg-info/top_level.txt
 spacer/__init__.py
 spacer/caffe_utils.py
 spacer/config.py
 spacer/data_classes.py
+spacer/exceptions.py
 spacer/extract_features.py
 spacer/extract_features_utils.py
 spacer/mailman.py
 spacer/messages.py
 spacer/storage.py
 spacer/task_utils.py
 spacer/tasks.py
```

### Comparing `pyspacer-0.3.1/README.md` & `pyspacer-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # PySpacer
 
-[![Build Status](https://travis-ci.com/beijbom/pyspacer.svg?branch=master)](https://travis-ci.com/beijbom/pyspacer)
+[![CI Status](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml/badge.svg)](https://github.com/beijbom/pyspacer/actions/workflows/python-app.yml)
 [![PyPI version](https://badge.fury.io/py/pyspacer.svg)](https://badge.fury.io/py/pyspacer)
 
 This repository provide utilities to extract features from random point 
 locations in images and then training classifiers over those features.
 It is used in the vision backend of `https://github.com/beijbom/coralnet`.
 
-Spacer currently supports python >=3.5.
+Spacer currently supports python >=3.8.
 
 ### Overview
 Spacer executes tasks as defined in messages. The messages types are defined
 in `messages.py` and the tasks in `tasks.py`. We also define several data-types
 in `data_classes.py` which define input and output types. 
 
 Refer to the unit-test in `test_tasks.py` for examples on how to create tasks.
 
 Tasks can be executed directly by calling the methods in tasks.py. 
-However, spacer also supports an interface with SQS 
-handled by `sqs_fetch()` in `mailman.py`. 
+However, spacer also supports an interface with AWS Batch 
+handled by `env_job()` in `mailman.py`. 
 
 Spacer supports four storage types: `s3`, `filesystem`, `memory` and `url`.
  Refer to `storage.py` for details. The Memory storage is mostly used for 
  testing, and the `url` storage is read only.
 
 Also take a look at `config.py` for settings and configuration. 
 
@@ -41,15 +41,17 @@
 The `secrets.json` should look like this.
 ```json
 {
   "SPACER_AWS_ACCESS_KEY_ID": "YOUR_AWS_KEY_ID",
   "SPACER_AWS_SECRET_ACCESS_KEY": "YOUR_AWS_SECRET_KEY",
   "SPACER_LOCAL_MODEL_PATH": "/path/to/your/local/models"
 }
-``` 
+```
+
+There is also an optional `TMP_PATH` setting: a filesystem directory to use for temporary files from unit tests and downloads. It defaults to the relative path `tmp`.
 
 #### Docker build
 The docker build is the preferred build and the one used in deployment.
 * Install docker on your system
 * Create `secrets.json` as detailed above.
 * Create folder `/path/to/your/local/models` for caching model files.
 * Build image: `docker build -t spacer:test .`
@@ -60,24 +62,26 @@
 which makes rerunning stuff much faster.
 
 The `-v ${PWD}:/workspace/spacer/` mounts your current folder including 
 `secrets.json` so that the container has the right permissions.
 
 The last step will run the default CMD command specified in the dockerfile 
 (unit-test with coverage). If you want to enter the docker container 
-run the same command but append `bash` in the end: 
+run the same command but append `bash` in the end.
 
 #### Pip install
 * `pip install spacer`
 * Set environmental variables.
 
 #### Local clone
 * Clone this repo
 * `pip install -r requirements.txt`
 
+If using Windows: turn Git's `autocrlf` setting off before your initial checkout. Otherwise, pickled classifiers in `spacer/tests/fixtures` will get checked out with `\r\n` newlines, and the pickle module will fail to load them, leading to test failures. However, autocrlf should be left on when adding any new non-pickle files.
+
 ### Code coverage
 If you are using the docker build or local install, 
 you can check code coverage like so:
 ```
     coverage run --source=spacer --omit=spacer/tests/* -m unittest    
     coverage report -m
     coverage html
```

