# Comparing `tmp/lung_analysis_pipeline-0.0.8.tar.gz` & `tmp/lung_analysis_pipeline-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lung_analysis_pipeline-0.0.8.tar", last modified: Sun Jun  4 22:20:07 2023, max compression
+gzip compressed data, was "dist/lung_analysis_pipeline-0.0.9.tar", last modified: Sun Jun  4 23:33:11 2023, max compression
```

## Comparing `lung_analysis_pipeline-0.0.8.tar` & `lung_analysis_pipeline-0.0.9.tar`

### file list

```diff
@@ -1,177 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/
--rw-r-----   0 root         (0) root         (0)     5399 2023-05-30 21:56:05.000000 lung_analysis_pipeline-0.0.8/README.md
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 18:50:05.000000 lung_analysis_pipeline-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/radiomics/
--rw-r-----   0 root         (0) root         (0)     6763 2023-06-04 21:44:18.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/radiomics/feature_extractor.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-30 23:16:38.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/radiomics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/HSCNN/
--rwxrwxrwx   0 root         (0) root         (0)     4877 2023-04-25 19:19:37.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/HSCNN/dataloader.py
--rwxrwxrwx   0 root         (0) root         (0)    23021 2023-04-25 19:23:54.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/HSCNN/train.py
--rwxrwxrwx   0 root         (0) root         (0)    13467 2023-06-04 21:24:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/HSCNN/model.py
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:33:34.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/HSCNN/__init__.py
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:32:08.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Feature_Extractor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/
--rwxr-x---   0 root         (0) root         (0)      510 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluation_updt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/dataset/
--rwxr-x---   0 root         (0) root         (0)    17508 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader.py
--rwxr-x---   0 root         (0) root         (0)    19594 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/dataset/bbox_reader_UCLA.py
--rwxr-x---   0 root         (0) root         (0)      862 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/dataset/collate.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/
--rwxr-x---   0 root         (0) root         (0)    27640 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/noduleCADEvaluationLUNA16.py
--rwxr-x---   0 root         (0) root         (0)      672 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/NoduleFinding.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/
--rwxr-x---   0 root         (0) root         (0)      791 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/csvTools.py
--rwxr-x---   0 root         (0) root         (0)      130 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/evaluationScript/tools/__init__.py
--rwxr-x---   0 root         (0) root         (0)     8924 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/test_normCnd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/utils/
--rwxr-x---   0 root         (0) root         (0)    17889 2023-05-30 03:19:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/utils/util.py
--rwxr-x---   0 root         (0) root         (0)     1474 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/utils/pybox.py
--rwxr-x---   0 root         (0) root         (0)     3777 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/utils/prepare_dataset_UCLA.py
--rw-r-----   0 root         (0) root         (0)        0 2023-06-01 16:34:25.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/utils/__init__.py
--rwxr-x---   0 root         (0) root         (0)    15175 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/
--rwxr-x---   0 root         (0) root         (0)     8483 2023-05-30 01:41:42.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/resnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/
--rwxr-x---   0 root         (0) root         (0)      799 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/build.py
--rwxr-x---   0 root         (0) root         (0)     1530 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/
--rwxr-x---   0 root         (0) root         (0)      383 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/torch_nms/extension/__init__.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/__init__.py
--rwxr-x---   0 root         (0) root         (0)     1177 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/nms/py_nms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/
--rwxr-x---   0 root         (0) root         (0)      819 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/build.py
--rwxr-x---   0 root         (0) root         (0)     1186 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/
--rwxr-x---   0 root         (0) root         (0)      383 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/torch_overlap/extension/__init__.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/overlap/__init__.py
--rwxr-x---   0 root         (0) root         (0)       83 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/__init__.py
--rwxr-x---   0 root         (0) root         (0)     9886 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/lib/box/process.py
--rwxr-x---   0 root         (0) root         (0)     8351 2023-05-30 03:05:06.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/cgnl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/
--rwxr-x---   0 root         (0) root         (0)     7357 2023-05-30 01:47:56.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_target.py
--rwxr-x---   0 root         (0) root         (0)     7120 2023-05-30 01:47:31.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_target.py
--rwxr-x---   0 root         (0) root         (0)     2424 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/util.py
--rwxr-x---   0 root         (0) root         (0)     5208 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_loss.py
--rwxr-x---   0 root         (0) root         (0)     2051 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_loss.py
--rwxr-x---   0 root         (0) root         (0)     5526 2023-05-30 22:39:08.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rcnn_nms.py
--rwxr-x---   0 root         (0) root         (0)     3534 2023-05-30 01:37:59.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/rpn_nms.py
--rwxr-x---   0 root         (0) root         (0)      169 2023-05-30 01:28:27.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/layer/__init__.py
--rwxr-x---   0 root         (0) root         (0)    20642 2023-06-03 22:05:06.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/sanet.py
--rwxr-x---   0 root         (0) root         (0)        0 2023-05-30 00:37:47.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/net/__init__.py
--rw-r-----   0 root         (0) root         (0)      650 2023-06-03 22:47:27.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/__init__.py
--rwxr-x---   0 root         (0) root         (0)     5536 2023-05-30 04:31:32.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/test.py
--rwxr-x---   0 root         (0) root         (0)     3891 2023-05-30 20:36:19.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleDetect_SANet/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/options/
--rw-r-----   0 root         (0) root         (0)     6803 2023-06-04 21:45:09.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/options/opt.py
--rw-r-----   0 root         (0) root         (0)        0 2023-04-13 03:10:53.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/options/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/
--rwxrwxrwx   0 root         (0) root         (0)     8249 2023-05-02 00:42:08.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/niiDataset_with_label.py
--rwxrwxrwx   0 root         (0) root         (0)     2996 2023-05-02 00:42:33.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/h5Dataset_with_label.py
--rw-r-----   0 root         (0) root         (0)     3094 2023-06-04 20:45:17.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/DcmDataset.py
--rwxrwxrwx   0 root         (0) root         (0)    12951 2023-05-30 03:19:35.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/util.py
--rwxrwxrwx   0 root         (0) root         (0)     2299 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/dcmDataset.py
--rwxrwxrwx   0 root         (0) root         (0)     6704 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/h5Dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     5989 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/LRHR_dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1771 2023-06-04 20:29:39.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8194 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/tmp_with_label.py
--rw-r-----   0 root         (0) root         (0)     5917 2023-06-04 20:58:54.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/dataset/nlstDataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/
--rwxrwxrwx   0 root         (0) root         (0)     4126 2023-06-03 22:09:51.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/bm3d_ht.py
--rwxrwxrwx   0 root         (0) root         (0)     3521 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/histogram_matching.py
--rw-r-----   0 root         (0) root         (0)        0 2023-04-21 04:31:56.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/non_DL/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5268 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/compute_metrics.py
--rwxrwxrwx   0 root         (0) root         (0)     8024 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_ExternalFolder.py
--rwxrwxrwx   0 root         (0) root         (0)     3262 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/norm_SingleVol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/options/
--rwxrwxrwx   0 root         (0) root         (0)     3917 2023-04-15 00:33:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/options/options.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/options/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/
--rwxrwxrwx   0 root         (0) root         (0)     8100 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm.py
--rwxrwxrwx   0 root         (0) root         (0)     9697 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_img_files.py
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/make_uids.py
--rwxrwxrwx   0 root         (0) root         (0)     1210 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_uids_for_cv.py
--rwxrwxrwx   0 root         (0) root         (0)     5414 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/get_log_values.py
--rwxrwxrwx   0 root         (0) root         (0)    20002 2023-04-19 18:34:56.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/util.py
--rwxrwxrwx   0 root         (0) root         (0)     5395 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-RetinaNet.py
--rwxrwxrwx   0 root         (0) root         (0)     6686 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/batch_hr2Toh5.py
--rwxrwxrwx   0 root         (0) root         (0)      590 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/read_tensorboard.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3214 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/process_aapm.py
--rwxrwxrwx   0 root         (0) root         (0)     4344 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/segment_lungs.py
--rwxrwxrwx   0 root         (0) root         (0)     5201 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/create_Dataset-Norm_uids.py
--rwxrwxrwx   0 root         (0) root         (0)     2277 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/utils/progress_bar.py
--rwxrwxrwx   0 root         (0) root         (0)    13690 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/train.py
--rwxrwxrwx   0 root         (0) root         (0)     2298 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/visualize_cases.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-02 03:43:26.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/
--rwxrwxrwx   0 root         (0) root         (0)    38696 2023-05-23 03:54:12.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_model.py
--rwxrwxrwx   0 root         (0) root         (0)     5731 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/lr_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/
--rwxrwxrwx   0 root         (0) root         (0)    29138 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/generators.py
--rwxrwxrwx   0 root         (0) root         (0)     7171 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/auxiliary_features.py
--rwxrwxrwx   0 root         (0) root         (0)     3367 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/loss.py
--rwxrwxrwx   0 root         (0) root         (0)     7002 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/block.py
--rwxrwxrwx   0 root         (0) root         (0)    16771 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/discriminators.py
--rwxrwxrwx   0 root         (0) root         (0)     2884 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/bam.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/modules/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9406 2023-05-02 00:27:09.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/networks.py
--rwxrwxrwx   0 root         (0) root         (0)     3590 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/build_unet_model.py
--rwxrwxrwx   0 root         (0) root         (0)    12140 2023-05-23 03:54:04.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SR_model.py
--rwxrwxrwx   0 root         (0) root         (0)    22520 2023-05-23 03:54:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/SRGAN_exp.py
--rwxrwxrwx   0 root         (0) root         (0)     3892 2023-06-01 18:44:23.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11424 2023-05-22 22:39:50.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/models/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/
--rwxrwxrwx   0 root         (0) root         (0)      805 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/
--rwxrwxrwx   0 root         (0) root         (0)     2023 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/html.py
--rwxrwxrwx   0 root         (0) root         (0)    14226 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/util.py
--rwxrwxrwx   0 root         (0) root         (0)     8602 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/visualizer.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1823 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/compute_dists_dirs.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/
--rwxrwxrwx   0 root         (0) root         (0)     7544 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/pretrained_networks.py
--rwxrwxrwx   0 root         (0) root         (0)    14721 2023-04-14 19:07:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/dist_model.py
--rwxrwxrwx   0 root         (0) root         (0)      269 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/models.py
--rwxrwxrwx   0 root         (0) root         (0)    11713 2023-04-14 19:06:50.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/networks_basic.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-07 20:47:20.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/PerceptualSimilarity/models/base_model.py
--rwxrwxrwx   0 root         (0) root         (0)     7630 2023-04-22 02:44:06.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/codes/test.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-02 03:35:30.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/Normalization_Pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/utils/
--rw-r-----   0 root         (0) root         (0)    29361 2023-06-04 21:17:38.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/utils/util.py
--rw-r-----   0 root         (0) root         (0)        0 2023-04-21 21:06:41.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/utils/__init__.py
--rw-r-----   0 root         (0) root         (0)    25935 2023-05-31 04:26:32.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/utils/patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/
--rwxrwxrwx   0 root         (0) root         (0)    11011 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/train_unet_lidc.py
--rwxrwxrwx   0 root         (0) root         (0)     2301 2023-04-25 21:29:27.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_lidc.py
--rwxrwxrwx   0 root         (0) root         (0)     5448 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_resnet34_lidc.py
--rwxrwxrwx   0 root         (0) root         (0)     5823 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/train.py
--rwxrwxrwx   0 root         (0) root         (0)     3612 2023-04-28 20:34:39.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/setting.py
--rwxrwxrwx   0 root         (0) root         (0)     4368 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/model.py
--rwxrwxrwx   0 root         (0) root         (0)     9258 2023-06-03 23:04:01.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/build_unet_model.py
--rw-r-----   0 root         (0) root         (0)        0 2023-05-30 01:25:50.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3346 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/test.py
--rwxrwxrwx   0 root         (0) root         (0)     3482 2023-04-11 19:09:49.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/NoduleSeg_MedicalNet/test_unet_norm.py
--rw-r-----   0 root         (0) root         (0)     3197 2023-06-04 21:41:39.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/model_pipeline.py
--rw-r-----   0 root         (0) root         (0)     1708 2023-05-30 04:43:18.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/__init__.py
--rw-r-----   0 root         (0) root         (0)     1072 2023-06-04 22:19:46.000000 lung_analysis_pipeline-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9190 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-04 22:20:07.000000 lung_analysis_pipeline-0.0.8/lung_analysis_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/
+-rw-r-----   0 root         (0) root         (0)     5399 2023-05-30 21:56:05.000000 lung_analysis_pipeline-0.0.9/README.md
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-01 18:50:05.000000 lung_analysis_pipeline-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/NoduleDetect_SANet/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/NoduleDetect_SANet/build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/NoduleDetect_SANet/build/box/
+-rwxr-x---   0 root         (0) root         (0)      261 2023-05-30 00:37:46.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/NoduleDetect_SANet/build/box/box.cpp
+-rw-r-----   0 root         (0) root         (0)     3197 2023-06-04 21:41:39.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/model_pipeline.py
+-rw-r-----   0 root         (0) root         (0)     1708 2023-05-30 04:43:18.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/__init__.py
+-rw-r-----   0 root         (0) root         (0)     3333 2023-06-04 23:32:47.000000 lung_analysis_pipeline-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-04 23:33:11.000000 lung_analysis_pipeline-0.0.9/lung_analysis_pipeline.egg-info/top_level.txt
```

### Comparing `lung_analysis_pipeline-0.0.8/README.md` & `lung_analysis_pipeline-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/model_pipeline.py` & `lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/model_pipeline.py`

 * *Files identical despite different names*

### Comparing `lung_analysis_pipeline-0.0.8/lung_analysis_pipeline/__init__.py` & `lung_analysis_pipeline-0.0.9/lung_analysis_pipeline/__init__.py`

 * *Files identical despite different names*

