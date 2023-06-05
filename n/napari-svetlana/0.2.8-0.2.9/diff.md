# Comparing `tmp/napari_svetlana-0.2.8.tar.gz` & `tmp/napari_svetlana-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_svetlana-0.2.8.tar", last modified: Mon Jun  5 08:33:45 2023, max compression
+gzip compressed data, was "napari_svetlana-0.2.9.tar", last modified: Mon Jun  5 09:44:46 2023, max compression
```

## Comparing `napari_svetlana-0.2.8.tar` & `napari_svetlana-0.2.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.243998 napari_svetlana-0.2.8/
--rw-rw-r--   0 clement   (1000) clement   (1000)    35148 2022-09-02 12:18:34.000000 napari_svetlana-0.2.8/LICENSE
--rw-rw-r--   0 clement   (1000) clement   (1000)      161 2022-08-29 09:37:54.000000 napari_svetlana-0.2.8/MANIFEST.in
--rw-rw-r--   0 clement   (1000) clement   (1000)     7393 2023-06-05 08:33:45.243998 napari_svetlana-0.2.8/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)     6175 2023-06-05 08:32:47.000000 napari_svetlana-0.2.8/README.md
--rw-rw-r--   0 clement   (1000) clement   (1000)      193 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/requirements.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)     1649 2023-06-05 08:33:45.247998 napari_svetlana-0.2.8/setup.cfg
--rw-rw-r--   0 clement   (1000) clement   (1000)       84 2022-10-25 10:39:03.000000 napari_svetlana-0.2.8/setup.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.227998 napari_svetlana-0.2.8/src/
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.235998 napari_svetlana-0.2.8/src/napari_svetlana/
--rw-rw-r--   0 clement   (1000) clement   (1000)     1637 2022-11-02 08:37:10.000000 napari_svetlana-0.2.8/src/napari_svetlana/CNN2D.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1451 2022-06-29 08:18:45.000000 napari_svetlana-0.2.8/src/napari_svetlana/CNN3D.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      619 2022-08-08 10:26:12.000000 napari_svetlana-0.2.8/src/napari_svetlana/Config.json
--rw-rw-r--   0 clement   (1000) clement   (1000)      879 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/CustomDataset.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1049 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/CustomDialog.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      938 2023-06-05 08:32:47.000000 napari_svetlana-0.2.8/src/napari_svetlana/DemoDialog.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.239998 napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2022-11-21 08:50:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     8885 2022-11-02 08:37:10.000000 napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/base_cam.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      751 2022-11-02 08:37:10.000000 napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/grad_cam.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     7323 2022-11-02 08:37:10.000000 napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/image.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     2981 2022-11-21 08:50:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/Prediction3DDataset.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     3742 2022-08-05 08:27:06.000000 napari_svetlana-0.2.8/src/napari_svetlana/PredictionDataset.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     3087 2022-08-05 08:27:06.000000 napari_svetlana-0.2.8/src/napari_svetlana/PredictionMulti3DDataset.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.243998 napari_svetlana-0.2.8/src/napari_svetlana/XP/
--rw-rw-r--   0 clement   (1000) clement   (1000)     3420 2022-07-27 13:06:50.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/Predict3Dbatch.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     2381 2022-08-01 09:01:43.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/Prediction3DDataset_dilation.py
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2022-07-27 13:05:42.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     2075 2022-08-01 09:01:43.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/compute_accuracy.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     3527 2023-02-06 09:01:33.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/extract_save_patches.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1558 2022-11-21 08:50:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/modulable_CNN3D.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1196 2022-10-25 14:18:14.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/redim.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     5315 2022-06-28 13:52:43.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/reseau.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    17178 2022-08-22 08:17:34.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training-stability_test.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    16325 2022-08-01 12:15:17.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_3D_1net.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    14958 2022-08-02 08:04:36.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    13280 2022-12-09 13:59:46.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    11531 2022-03-01 15:16:57.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_test.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    28297 2022-07-27 13:17:00.000000 napari_svetlana-0.2.8/src/napari_svetlana/XP/testeur.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      123 2023-06-05 08:32:47.000000 napari_svetlana-0.2.8/src/napari_svetlana/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)   157058 2023-06-05 08:32:47.000000 napari_svetlana-0.2.8/src/napari_svetlana/_batch_dock_widget.py
--rw-rw-r--   0 clement   (1000) clement   (1000)    66687 2022-05-09 07:58:30.000000 napari_svetlana-0.2.8/src/napari_svetlana/_dock_widget.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1708 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_function.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     2771 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_reader.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.243998 napari_svetlana-0.2.8/src/napari_svetlana/_tests/
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_tests/__init__.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1249 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_tests/test_dock_widget.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      117 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_tests/test_function.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      976 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_tests/test_reader.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      127 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_tests/test_writer.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      463 2022-02-28 15:25:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/_writer.py
--rw-rw-r--   0 clement   (1000) clement   (1000)      537 2022-03-14 10:31:04.000000 napari_svetlana-0.2.8/src/napari_svetlana/areasl_susts.py
--rw-rw-r--   0 clement   (1000) clement   (1000)       77 2022-10-17 09:48:58.000000 napari_svetlana-0.2.8/src/napari_svetlana/debug.py
--rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-06-05 08:32:47.000000 napari_svetlana-0.2.8/src/napari_svetlana/line_length.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1205 2022-11-21 08:50:24.000000 napari_svetlana-0.2.8/src/napari_svetlana/mosa.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     1146 2023-06-05 08:32:47.000000 napari_svetlana-0.2.8/src/napari_svetlana/napari.yaml
--rw-rw-r--   0 clement   (1000) clement   (1000)    62329 2023-04-24 10:14:18.000000 napari_svetlana-0.2.8/src/napari_svetlana/old_dock_widget.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     5073 2023-02-06 09:01:33.000000 napari_svetlana-0.2.8/src/napari_svetlana/test_gradcam.py
--rw-rw-r--   0 clement   (1000) clement   (1000)     4837 2022-11-02 08:37:10.000000 napari_svetlana-0.2.8/src/napari_svetlana/test_gradcam3D.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 08:33:45.239998 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/
--rw-rw-r--   0 clement   (1000) clement   (1000)     7393 2023-06-05 08:33:45.000000 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)     2145 2023-06-05 08:33:45.000000 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/SOURCES.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-06-05 08:33:45.000000 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/dependency_links.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       64 2023-06-05 08:33:45.000000 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/entry_points.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)      222 2023-06-05 08:33:45.000000 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/requires.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       16 2023-06-05 08:33:45.000000 napari_svetlana-0.2.8/src/napari_svetlana.egg-info/top_level.txt
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.681003 napari_svetlana-0.2.9/
+-rw-rw-r--   0 clement   (1000) clement   (1000)    35148 2022-09-02 12:18:34.000000 napari_svetlana-0.2.9/LICENSE
+-rw-rw-r--   0 clement   (1000) clement   (1000)      161 2022-08-29 09:37:54.000000 napari_svetlana-0.2.9/MANIFEST.in
+-rw-rw-r--   0 clement   (1000) clement   (1000)     7393 2023-06-05 09:44:46.681003 napari_svetlana-0.2.9/PKG-INFO
+-rw-rw-r--   0 clement   (1000) clement   (1000)     6175 2023-06-05 08:32:47.000000 napari_svetlana-0.2.9/README.md
+-rw-rw-r--   0 clement   (1000) clement   (1000)      193 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/requirements.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1649 2023-06-05 09:44:46.681003 napari_svetlana-0.2.9/setup.cfg
+-rw-rw-r--   0 clement   (1000) clement   (1000)       84 2022-10-25 10:39:03.000000 napari_svetlana-0.2.9/setup.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.665003 napari_svetlana-0.2.9/src/
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.673003 napari_svetlana-0.2.9/src/napari_svetlana/
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1637 2022-11-02 08:37:10.000000 napari_svetlana-0.2.9/src/napari_svetlana/CNN2D.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1451 2022-06-29 08:18:45.000000 napari_svetlana-0.2.9/src/napari_svetlana/CNN3D.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      619 2022-08-08 10:26:12.000000 napari_svetlana-0.2.9/src/napari_svetlana/Config.json
+-rw-rw-r--   0 clement   (1000) clement   (1000)      879 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/CustomDataset.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1049 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/CustomDialog.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      938 2023-06-05 08:32:47.000000 napari_svetlana-0.2.9/src/napari_svetlana/DemoDialog.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.673003 napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2022-11-21 08:50:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     8885 2022-11-02 08:37:10.000000 napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/base_cam.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      751 2022-11-02 08:37:10.000000 napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/grad_cam.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     7323 2022-11-02 08:37:10.000000 napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/image.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2981 2022-11-21 08:50:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/Prediction3DDataset.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3742 2022-08-05 08:27:06.000000 napari_svetlana-0.2.9/src/napari_svetlana/PredictionDataset.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3087 2022-08-05 08:27:06.000000 napari_svetlana-0.2.9/src/napari_svetlana/PredictionMulti3DDataset.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.677003 napari_svetlana-0.2.9/src/napari_svetlana/XP/
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3420 2022-07-27 13:06:50.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/Predict3Dbatch.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2381 2022-08-01 09:01:43.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/Prediction3DDataset_dilation.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2022-07-27 13:05:42.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2075 2022-08-01 09:01:43.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/compute_accuracy.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     3527 2023-02-06 09:01:33.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/extract_save_patches.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1558 2022-11-21 08:50:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/modulable_CNN3D.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1196 2022-10-25 14:18:14.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/redim.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     5315 2022-06-28 13:52:43.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/reseau.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    17178 2022-08-22 08:17:34.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training-stability_test.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    16325 2022-08-01 12:15:17.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_3D_1net.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    14958 2022-08-02 08:04:36.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    13280 2022-12-09 13:59:46.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    11531 2022-03-01 15:16:57.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_test.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    28297 2022-07-27 13:17:00.000000 napari_svetlana-0.2.9/src/napari_svetlana/XP/testeur.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      123 2023-06-05 08:32:47.000000 napari_svetlana-0.2.9/src/napari_svetlana/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)   157058 2023-06-05 08:32:47.000000 napari_svetlana-0.2.9/src/napari_svetlana/_batch_dock_widget.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)    66687 2022-05-09 07:58:30.000000 napari_svetlana-0.2.9/src/napari_svetlana/_dock_widget.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1708 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_function.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2771 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_reader.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.677003 napari_svetlana-0.2.9/src/napari_svetlana/_tests/
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_tests/__init__.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1249 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_tests/test_dock_widget.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      117 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_tests/test_function.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      976 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_tests/test_reader.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      127 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_tests/test_writer.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      463 2022-02-28 15:25:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/_writer.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)      537 2022-03-14 10:31:04.000000 napari_svetlana-0.2.9/src/napari_svetlana/areasl_susts.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)       77 2022-10-17 09:48:58.000000 napari_svetlana-0.2.9/src/napari_svetlana/debug.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)        0 2023-06-05 08:32:47.000000 napari_svetlana-0.2.9/src/napari_svetlana/line_length.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1205 2022-11-21 08:50:24.000000 napari_svetlana-0.2.9/src/napari_svetlana/mosa.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     1146 2023-06-05 08:32:47.000000 napari_svetlana-0.2.9/src/napari_svetlana/napari.yaml
+-rw-rw-r--   0 clement   (1000) clement   (1000)    62329 2023-04-24 10:14:18.000000 napari_svetlana-0.2.9/src/napari_svetlana/old_dock_widget.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     5073 2023-02-06 09:01:33.000000 napari_svetlana-0.2.9/src/napari_svetlana/test_gradcam.py
+-rw-rw-r--   0 clement   (1000) clement   (1000)     4837 2022-11-02 08:37:10.000000 napari_svetlana-0.2.9/src/napari_svetlana/test_gradcam3D.py
+drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-06-05 09:44:46.673003 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/
+-rw-rw-r--   0 clement   (1000) clement   (1000)     7393 2023-06-05 09:44:46.000000 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/PKG-INFO
+-rw-rw-r--   0 clement   (1000) clement   (1000)     2145 2023-06-05 09:44:46.000000 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/SOURCES.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-06-05 09:44:46.000000 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/dependency_links.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       64 2023-06-05 09:44:46.000000 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/entry_points.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)      222 2023-06-05 09:44:46.000000 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/requires.txt
+-rw-rw-r--   0 clement   (1000) clement   (1000)       16 2023-06-05 09:44:46.000000 napari_svetlana-0.2.9/src/napari_svetlana.egg-info/top_level.txt
```

### Comparing `napari_svetlana-0.2.8/LICENSE` & `napari_svetlana-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/PKG-INFO` & `napari_svetlana-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_svetlana
-Version: 0.2.8
+Version: 0.2.9
 Summary: A classification plugin for the ROIs of a segmentation mask.
 Author: Clément Cazorla
 Author-email: clement.cazorla31@gmail.com
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://bitbucket.org/koopa31/napari_svetlana/issues?status=new&status=open
 Project-URL: Documentation, https://svetlana-documentation.readthedocs.io/en/latest/
 Project-URL: Source Code, https://bitbucket.org/koopa31/napari_svetlana/src/main/
```

### Comparing `napari_svetlana-0.2.8/README.md` & `napari_svetlana-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/setup.cfg` & `napari_svetlana-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari_svetlana
-version = 0.2.8
+version = 0.2.9
 author = Clément Cazorla
 author_email = clement.cazorla31@gmail.com
 license = GPL-3.0-only
 description = A classification plugin for the ROIs of a segmentation mask.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -31,15 +31,15 @@
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
 	napari-plugin-engine>=0.1.4
 	numpy
 	albumentations==1.0.3
-	joblib==1.1.0
+	joblib==1.2.0
 	light-the-torch
 	matplotlib
 	opencv-python==4.5.5.62
 	PyQt5
 	cucim==22.6.0;platform_system=='Linux'
 	cupy-cuda102==10.6.0
 	xlsxwriter
```

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/CNN2D.py` & `napari_svetlana-0.2.9/src/napari_svetlana/CNN2D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/CNN3D.py` & `napari_svetlana-0.2.9/src/napari_svetlana/CNN3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/Config.json` & `napari_svetlana-0.2.9/src/napari_svetlana/Config.json`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/CustomDataset.py` & `napari_svetlana-0.2.9/src/napari_svetlana/CustomDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/CustomDialog.py` & `napari_svetlana-0.2.9/src/napari_svetlana/CustomDialog.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/DemoDialog.py` & `napari_svetlana-0.2.9/src/napari_svetlana/DemoDialog.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/base_cam.py` & `napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/base_cam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/grad_cam.py` & `napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/grad_cam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/Grad_Cam/image.py` & `napari_svetlana-0.2.9/src/napari_svetlana/Grad_Cam/image.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/Prediction3DDataset.py` & `napari_svetlana-0.2.9/src/napari_svetlana/Prediction3DDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/PredictionDataset.py` & `napari_svetlana-0.2.9/src/napari_svetlana/PredictionDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/PredictionMulti3DDataset.py` & `napari_svetlana-0.2.9/src/napari_svetlana/PredictionMulti3DDataset.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/Predict3Dbatch.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/Predict3Dbatch.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/Prediction3DDataset_dilation.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/Prediction3DDataset_dilation.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/compute_accuracy.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/compute_accuracy.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/extract_save_patches.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/extract_save_patches.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/modulable_CNN3D.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/modulable_CNN3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/redim.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/redim.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/reseau.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/reseau.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training-stability_test.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training-stability_test.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_3D_1net.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_3D_1net.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_3D_dilatation_mask.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_3D_patch_size_norm.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/script_training_test.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/script_training_test.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/XP/testeur.py` & `napari_svetlana-0.2.9/src/napari_svetlana/XP/testeur.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/_batch_dock_widget.py` & `napari_svetlana-0.2.9/src/napari_svetlana/_batch_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/_dock_widget.py` & `napari_svetlana-0.2.9/src/napari_svetlana/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/_function.py` & `napari_svetlana-0.2.9/src/napari_svetlana/_function.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/_reader.py` & `napari_svetlana-0.2.9/src/napari_svetlana/_reader.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/_tests/test_dock_widget.py` & `napari_svetlana-0.2.9/src/napari_svetlana/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/_tests/test_reader.py` & `napari_svetlana-0.2.9/src/napari_svetlana/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/areasl_susts.py` & `napari_svetlana-0.2.9/src/napari_svetlana/areasl_susts.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/mosa.py` & `napari_svetlana-0.2.9/src/napari_svetlana/mosa.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/napari.yaml` & `napari_svetlana-0.2.9/src/napari_svetlana/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/old_dock_widget.py` & `napari_svetlana-0.2.9/src/napari_svetlana/old_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/test_gradcam.py` & `napari_svetlana-0.2.9/src/napari_svetlana/test_gradcam.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana/test_gradcam3D.py` & `napari_svetlana-0.2.9/src/napari_svetlana/test_gradcam3D.py`

 * *Files identical despite different names*

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana.egg-info/PKG-INFO` & `napari_svetlana-0.2.9/src/napari_svetlana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-svetlana
-Version: 0.2.8
+Version: 0.2.9
 Summary: A classification plugin for the ROIs of a segmentation mask.
 Author: Clément Cazorla
 Author-email: clement.cazorla31@gmail.com
 License: GPL-3.0-only
 Project-URL: Bug Tracker, https://bitbucket.org/koopa31/napari_svetlana/issues?status=new&status=open
 Project-URL: Documentation, https://svetlana-documentation.readthedocs.io/en/latest/
 Project-URL: Source Code, https://bitbucket.org/koopa31/napari_svetlana/src/main/
```

### Comparing `napari_svetlana-0.2.8/src/napari_svetlana.egg-info/SOURCES.txt` & `napari_svetlana-0.2.9/src/napari_svetlana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

