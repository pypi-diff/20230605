# Comparing `tmp/Simba-UW-tf-dev-1.62.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.62.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.62.3.tar", last modified: Thu Jun  1 16:10:09 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.62.4.tar", last modified: Mon Jun  5 18:46:57 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.62.3.tar` & `Simba-UW-tf-dev-1.62.4.tar`

### file list

```diff
@@ -1,514 +1,519 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.62.3/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.62.3/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.62.3/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.3/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.62.3/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.3/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.3/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.62.3/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.3/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-01 15:34:41.000000 Simba-UW-tf-dev-1.62.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8582 2023-05-31 20:56:05.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.62.3/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43030 2023-06-01 11:48:36.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37111 2023-06-01 14:51:22.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    71329 2023-06-01 14:07:28.000000 Simba-UW-tf-dev-1.62.3/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.62.3/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.62.3/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.62.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.62.3/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.62.3/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.62.3/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.62.3/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.62.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.62.3/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.62.3/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.3/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.3/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.3/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.62.3/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.62.3/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19109 2023-06-01 13:04:10.000000 Simba-UW-tf-dev-1.62.3/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.62.3/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.62.3/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18887 2023-06-01 13:04:10.000000 Simba-UW-tf-dev-1.62.3/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.62.3/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.62.3/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.62.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.62.3/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.62.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.62.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.62.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.62.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.3/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18993 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.62.3/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.62.3/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.62.3/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.62.3/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.3/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2977 2023-06-01 15:34:16.000000 Simba-UW-tf-dev-1.62.3/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.62.3/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.62.3/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.62.3/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.3/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/two_c57/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.62.3/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.62.3/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.62.3/tests/test_validation_clips.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.62.3/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.62.3/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-01 16:08:56.000000 Simba-UW-tf-dev-1.62.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-01 16:10:09.000000 Simba-UW-tf-dev-1.62.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.62.4/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.62.4/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.62.4/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.4/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.62.4/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35432 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.4/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.4/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.62.4/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.4/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-05 16:31:18.000000 Simba-UW-tf-dev-1.62.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.62.4/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73777 2023-06-05 18:45:46.000000 Simba-UW-tf-dev-1.62.4/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.62.4/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21017 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.4/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-05 17:20:50.000000 Simba-UW-tf-dev-1.62.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.62.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.62.4/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.62.4/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8585 2023-06-05 17:07:45.000000 Simba-UW-tf-dev-1.62.4/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.62.4/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.62.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.62.4/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.62.4/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.4/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.4/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.4/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.62.4/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.62.4/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20128 2023-06-05 18:11:07.000000 Simba-UW-tf-dev-1.62.4/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.62.4/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.62.4/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.62.4/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.62.4/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.62.4/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.62.4/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.62.4/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.62.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.62.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.62.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.62.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.4/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19265 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.62.4/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.62.4/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.62.4/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.62.4/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-06-04 19:21:28.000000 Simba-UW-tf-dev-1.62.4/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.62.4/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.62.4/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.62.4/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.62.4/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/two_c57/models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.62.4/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.62.4/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.62.4/tests/test_validation_clips.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.62.4/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.62.4/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-05 18:46:49.000000 Simba-UW-tf-dev-1.62.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-05 18:46:57.000000 Simba-UW-tf-dev-1.62.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.62.3/PKG-INFO` & `Simba-UW-tf-dev-1.62.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.62.3
+Version: 1.62.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.62.4/simba/ui/machine_model_settings_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,22 @@
         self.learning_curve_cb = Checkbutton(self.evaluations_frm, text='Create Learning Curves (Note: CPU intensive)', variable=self.learning_curve_var, command=lambda: self.enable_entrybox_from_checkbox(check_box_var=self.learning_curve_var, entry_boxes=[self.learning_curve_k_splits_entry_box, self.learning_curve_data_splits_entry_box]))
         self.create_pr_curve_cb = Checkbutton(self.evaluations_frm, text='Create Precision Recall Curves', variable=self.create_pr_curve_var)
         self.shap_present = Entry_Box(self.evaluations_frm, '# target present', '25', status=DISABLED, validation='numeric')
         self.shap_absent = Entry_Box(self.evaluations_frm, '# target absent', '25', status=DISABLED,  validation='numeric')
         self.shap_save_it_dropdown = DropDownMenu(self.evaluations_frm, 'SHAP save cadence: ', [1, 10, 100, 1000, 'ALL FRAMES'],  '25')
         self.shap_save_it_dropdown.setChoices('ALL FRAMES')
         self.shap_save_it_dropdown.disable()
+        self.shap_multiprocess_dropdown = DropDownMenu(self.evaluations_frm, 'Multi-process SHAP values: ', ['True', 'False'], '25', com=lambda x: self.change_shap_cadence_options(x))
+        self.shap_multiprocess_dropdown.setChoices('False')
+        self.shap_multiprocess_dropdown.disable()
+
+
         self.partial_dependency_cb = Checkbutton(self.evaluations_frm, text='Calculate partial dependencies (Note: CPU intensive)', variable=self.partial_dependency_var)
         self.calculate_shap_scores_cb = Checkbutton(self.evaluations_frm, text='Calculate SHAP scores', variable=self.calc_shap_scores_var, command=lambda: [self.enable_entrybox_from_checkbox(check_box_var=self.calc_shap_scores_var, entry_boxes=[self.shap_present,self.shap_absent]),
-                                                                                                                                                             self.enable_dropdown_from_checkbox(check_box_var=self.calc_shap_scores_var, dropdown_menus=[self.shap_save_it_dropdown])])
+                                                                                                                                                             self.enable_dropdown_from_checkbox(check_box_var=self.calc_shap_scores_var, dropdown_menus=[self.shap_save_it_dropdown, self.shap_multiprocess_dropdown])])
         self.save_frame = LabelFrame(self.main_frm, text='SAVE', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         save_global_btn = Button(self.save_frame, text='SAVE SETTINGS (GLOBAL ENVIRONMENT)', font=('Helvetica', 12, 'bold'), fg='blue', command=lambda: self.save_global())
         save_meta_btn = Button(self.save_frame, text='SAVE SETTINGS (SPECIFIC MODEL)', font=('Helvetica', 12, 'bold'), fg='green', command=lambda: self.save_config())
         clear_cache_btn = Button(self.save_frame,text='CLEAR CACHE', font=('Helvetica', 12, 'bold'),fg='red', command=lambda: self.clear_cache())
 
         load_meta_data_frm.grid(row=0, column=0, sticky=NW)
         self.select_config_file.grid(row=0, column=0, sticky=NW)
@@ -146,14 +151,15 @@
         self.learning_curve_data_splits_entry_box.grid(row=9, column=0, sticky=NW)
         self.create_pr_curve_cb.grid(row=10, column=0, sticky=NW)
         self.partial_dependency_cb.grid(row=11, column=0, sticky=NW)
         self.calculate_shap_scores_cb.grid(row=12, column=0, sticky=NW)
         self.shap_present.grid(row=13, column=0, sticky=NW)
         self.shap_absent.grid(row=14, column=0, sticky=NW)
         self.shap_save_it_dropdown.grid(row=15, column=0, sticky=NW)
+        self.shap_multiprocess_dropdown.grid(row=16, column=0, sticky=NW)
 
         self.save_frame.grid(row=5, column=0, sticky=NW)
         save_global_btn.grid(row=0, column=0, sticky=NW)
         save_meta_btn.grid(row=1, column=0, sticky=NW)
         clear_cache_btn.grid(row=2, column=0, sticky=NW)
 
         self.main_frm.mainloop()
@@ -233,19 +239,21 @@
         if self.clf_importance_bars:
             self.clf_importance_bars_n = self.n_features_bars_entry_box.entry_get
         self.permutation_importances = self.feature_permutation_importance_var.get()
         self.pr_curve = self.create_pr_curve_var.get()
         self.shap_scores_absent = 0
         self.shap_scores_present = 0
         self.shap_save_it = 'ALL FRAMES'
+        self.shap_multiprocess = False
         self.shap_scores = self.calc_shap_scores_var.get()
         if self.shap_scores:
             self.shap_scores_absent = self.shap_absent.entry_get
             self.shap_scores_present = self.shap_present.entry_get
             self.shap_save_it = self.shap_save_it_dropdown.getChoices()
+            self.shap_multiprocess = self.shap_multiprocess_dropdown.getChoices()
         self.learning_curve = self.learning_curve_var.get()
         self.partial_dependency = self.partial_dependency_var.get()
         self.learning_curve_k_split = 0
         self.learning_curve_data_split = 0
         if self.learning_curve:
             self.learning_curve_k_split = self.learning_curve_k_splits_entry_box.entry_get
             self.learning_curve_data_split = self.learning_curve_data_splits_entry_box.entry_get
@@ -253,14 +261,21 @@
     def find_meta_file_cnt(self):
         self.meta_file_cnt = 0
         self.total_meta_files = find_files_of_filetypes_in_directory(directory=self.configs_meta_dir, extensions=['.csv'], raise_warning=False)
         for f in os.listdir(self.configs_meta_dir):
             if f.__contains__('_meta') and f.__contains__(str(self.behavior_name)):
                 self.meta_file_cnt += 1
 
+    def change_shap_cadence_options(self, x):
+        if x == 'True':
+            self.shap_save_it_dropdown.setChoices('ALL FRAMES')
+            self.shap_save_it_dropdown.disable()
+        else:
+            self.shap_save_it_dropdown.enable()
+
     def save_global(self):
         self.__checks()
         self.__get_variables()
         self.config.set('create ensemble settings', 'model_to_run', self.algorithm)
         self.config.set('create ensemble settings', 'RF_n_estimators', str(self.n_estimators))
         self.config.set('create ensemble settings', 'RF_max_features', str(self.max_features))
         self.config.set('create ensemble settings', 'RF_criterion', self.criterion)
@@ -284,14 +299,15 @@
         self.config.set('create ensemble settings', 'LearningCurve_shuffle_k_splits',str(self.learning_curve_k_split))
         self.config.set('create ensemble settings', 'LearningCurve_shuffle_data_splits', str(self.learning_curve_data_split))
         self.config.set('create ensemble settings', 'generate_example_decision_tree_fancy',str(self.example_dtreeviz))
         self.config.set('create ensemble settings', 'generate_shap_scores', str(self.shap_scores))
         self.config.set('create ensemble settings', 'shap_target_present_no', str(self.shap_scores_present))
         self.config.set('create ensemble settings', 'shap_target_absent_no', str(self.shap_scores_absent))
         self.config.set('create ensemble settings', 'shap_save_iteration', str(self.shap_save_it))
+        self.config.set('create ensemble settings', 'shap_multiprocess', str(self.shap_multiprocess))
         self.config.set('create ensemble settings', 'partial_dependency', str(self.partial_dependency))
         self.config.set('create ensemble settings', 'class_weights', str(self.class_weight_method))
         self.config.set('create ensemble settings', 'custom_weights', str(self.class_custom_weights))
 
         with open(self.config_path, 'w') as f:
             self.config.write(f)
 
@@ -322,14 +338,15 @@
                 'generate_precision_recall_curves':self.pr_curve,
                 'learning_curve_k_splits':self.learning_curve_k_split,
                 'learning_curve_data_splits': self.learning_curve_data_split,
                 'generate_shap_scores':self.shap_scores,
                 'shap_target_present_no':self.shap_scores_present,
                 'shap_target_absent_no':self.shap_scores_absent,
                 'shap_save_iteration': self.shap_save_it,
+                'shap_multiprocess': self.shap_multiprocess,
                 'partial_dependency': self.partial_dependency,
                 'class_weights': self.class_weight_method,
                 'class_custom_weights': str(self.class_custom_weights)}
 
         meta_df = pd.DataFrame(meta, index=[0])
         meta_df.insert(0, 'Classifier_name', self.behavior_name)
         self.find_meta_file_cnt()
@@ -429,37 +446,43 @@
 
         if self.meta['generate_shap_scores']:
             self.calc_shap_scores_var.set(value=True)
             self.shap_present.set_state(NORMAL)
             self.shap_absent.set_state(NORMAL)
             self.shap_absent.set_state(NORMAL)
             self.shap_save_it_dropdown.enable()
+            self.shap_multiprocess_dropdown.enable()
             self.shap_present.entry_set(val=self.meta['shap_target_present_no'])
             self.shap_absent.entry_set(val=self.meta['shap_target_absent_no'])
             if 'shap_save_iteration' in self.meta.keys():
                 self.shap_save_it_dropdown.setChoices(self.meta['shap_save_iteration'])
             else:
                 self.shap_save_it_dropdown.setChoices('ALL FRAMES')
+            if 'shap_multiprocess' in self.meta.keys():
+                self.shap_multiprocess_dropdown.setChoices(self.meta['shap_multiprocess'])
         else:
             self.calc_shap_scores_var.set(value=False)
             self.shap_present.set_state(DISABLED)
             self.shap_absent.set_state(DISABLED)
             self.shap_save_it_dropdown.enable()
+            self.shap_multiprocess_dropdown.disable()
 
         if 'train_test_split_type' in self.meta.keys():
             self.train_test_type_dropdown.setChoices(self.meta['train_test_split_type'])
         else:
             self.train_test_type_dropdown.setChoices(Options.TRAIN_TEST_SPLIT.value[0])
         if 'shap_save_iteration' in self.meta.keys():
             self.shap_save_it_dropdown.setChoices(self.meta['shap_save_iteration'])
+        else:
+            self.shap_save_it_dropdown.setChoices('None')
+        if 'shap_save_iteration' in self.meta.keys():
+            self.shap_multiprocess_dropdown.setChoices(self.meta['shap_multiprocess'])
         if 'partial_dependency' in self.meta.keys():
             if self.meta['partial_dependency'] in Options.RUN_OPTIONS_FLAGS.value:
                 self.partial_dependency_var.set(value=True)
-        else:
-            self.shap_save_it_dropdown.setChoices('None')
         if 'class_weights' in self.meta.keys():
             if self.meta['class_weights'] not in Options.CLASS_WEIGHT_OPTIONS.value:
                 self.meta['class_weights'] = 'None'
             self.class_weights_dropdown.setChoices(self.meta['class_weights'])
             if self.meta['class_weights'] == 'custom':
                 self.create_class_weight_table()
                 weights = ast.literal_eval(self.meta['class_custom_weights'])
@@ -495,12 +518,13 @@
                                            'learning_curve_k_splits',
                                            'learning_curve_data_splits',
                                            'generate_example_decision_tree_fancy',
                                            'generate_shap_scores',
                                            'shap_target_present_no',
                                            'shap_target_absent_no',
                                            'shap_save_iteration',
+                                           'shap_multiprocess',
                                            'partial_dependency',
                                            'class_weights',
                                            'class_custom_weights']
 
 #_ = MachineModelSettingsPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.62.4/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.62.4/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.62.4/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.62.4/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.62.4/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.62.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -759,20 +759,20 @@
 00002f60: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 00002f70: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 00002f80: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 00002f90: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00002fa0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00002fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00002fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00002fd0: 0809 5f10 187b 7b33 3037 2c20 3836 7d2c  .._..{{307, 86},
+00002fd0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
 00002fe0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
 00002ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 00003000: 0000 0001 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0004 5259 0000 0005 0075  mp......RY.....u
+00003020: 6d70 0000 0000 000b 16bf 0000 0005 0075  mp.............u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,20 +848,20 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 0897 a5fc  smoDDblob.......
-00003570: 1168 14c5 4100 0000 0500 7500 7400 6900  .h..A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 086f  l.smodDblob....o
-00003590: 9b46 7beb 0fc5 4100 0000 0500 7500 7400  .F{...A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 0893 f1b8  smoDDblob.......
+00003570: ea20 17c5 4100 0000 0500 7500 7400 6900  . ..A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 0893  l.smodDblob.....
+00003590: f1b8 ea20 17c5 4100 0000 0500 7500 7400  ... ..A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 0520 0000 0000 0500 7500 7400 6900  ... ......u.t.i.
+000035b0: 0000 0cb0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -1040,15 +1040,15 @@
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0000  ._lg1Scomp......
 00004110: c933 0000 000b 005f 005f 0070 0079 0063  .3....._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
 00004130: 626c 6f62 0000 0008 68ff 13ac ef0f c541  blob....h......A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 a913 1348 cc0c c541 0000  ob.......H...A..
+00004160: 6f62 0000 0008 68ff 13ac ef0f c541 0000  ob....h......A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0000 e000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
 000041b0: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
 000041c0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 000041d0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
@@ -1489,15 +1489,15 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0901 fb09 5863 6f6d  omp.........Xcom
+00005d70: 6f6d 7000 0000 0000 0904 0e09 5863 6f6d  omp.........Xcom
 00005d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
 00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
 00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
 00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
 00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
 00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
 00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
@@ -1714,15 +1714,15 @@
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
 00006b20: 0908 095f 1018 7b7b 3330 372c 2038 367d  ..._..{{307, 86}
 00006b30: 2c20 7b31 3037 362c 2036 3231 7d7d 0908  , {1076, 621}}..
 00006b40: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
 00006b50: 0000 0000 0101 0000 0000 0000 000f 0000  ................
 00006b60: 0000 0000 0000 0000 0000 0000 009a 0000  ................
 00006b70: 0006 006d 0069 0078 0069 006e 0073 6c67  ...m.i.x.i.n.slg
-00006b80: 3153 636f 6d70 0000 0000 0008 6e5e 0000  1Scomp......n^..
+00006b80: 3153 636f 6d70 0000 0000 0009 f692 0000  1Scomp..........
 00006b90: 0006 006d 0069 0078 0069 006e 0073 6c73  ...m.i.x.i.n.sls
 00006ba0: 7643 626c 6f62 0000 0281 6270 6c69 7374  vCblob....bplist
 00006bb0: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
 00006bc0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
 00006bd0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 00006be0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 00006bf0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 dbcf 3cd1 6814 c541  blob......<.h..A
+00007020: 626c 6f62 0000 0008 c6dc 83c4 8916 c541  blob...........A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 dbcf 3cd1  modDblob......<.
-00007050: 6814 c541 0000 0006 006d 0069 0078 0069  h..A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 c6dc 83c4  modDblob........
+00007050: 8916 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0009 3000 0000 0006 006d 0069 0078 0069  ..0......m.i.x.i
+00007070: 000a d000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -2681,15 +2681,15 @@
 0000a780: 5f00 6c00 6100 6200 6500 6c00 5f00 6100  _.l.a.b.e.l._.a.
 0000a790: 7000 7000 6500 6e00 6400 6500 7200 736d  p.p.e.n.d.e.r.sm
 0000a7a0: 6f44 4462 6c6f 6200 0000 083f 8021 40a0  oDDblob....?.!@.
 0000a7b0: 12c5 4100 0000 1b00 7400 6800 6900 7200  ..A.....t.h.i.r.
 0000a7c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000a7d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000a7e0: 7000 6500 6e00 6400 6500 7200 736d 6f64  p.e.n.d.e.r.smod
-0000a7f0: 4462 6c6f 6200 0000 08cb c8d0 edcc 0cc5  Dblob...........
+0000a7f0: 4462 6c6f 6200 0000 083f 8021 40a0 12c5  Dblob....?.!@...
 0000a800: 4100 0000 1b00 7400 6800 6900 7200 6400  A.....t.h.i.r.d.
 0000a810: 5f00 7000 6100 7200 7400 7900 5f00 6c00  _.p.a.r.t.y._.l.
 0000a820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
 0000a830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
 0000a840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
 0000a850: 7400 6800 6900 7200 6400 5f00 7000 6100  t.h.i.r.d._.p.a.
 0000a860: 7200 7400 7900 5f00 6c00 6100 6200 6500  r.t.y._.l.a.b.e.
@@ -2935,15 +2935,15 @@
 0000b760: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
 0000b770: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 0000b780: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 0000b790: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 0000b7a0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 0000b7b0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 0000b7c0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-0000b7d0: 0809 5f10 187b 7b33 3037 2c20 3836 7d2c  .._..{{307, 86},
+0000b7d0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
 0000b7e0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
 0000b7f0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 0000b800: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 0000b810: 0000 0000 0000 0000 0000 0000 9a00 6c00  ..............l.
 0000b820: 6100 6200 6500 6c00 5f00 6100 7000 7000  a.b.e.l._.a.p.p.
 0000b830: 6500 6e00 6400 6500 7200 7370 6831 5363  e.n.d.e.r.sph1Sc
 0000b840: 6f6d 7000 0000 0000 02b0 0000 0000 1b00  omp.............
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 import pandas as pd
 from sklearn.ensemble import RandomForestClassifier
 from simba.utils.read_write import read_df
 from typing import List, Optional
 from simba.utils.read_write import find_core_cnt
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import SimbaTimer, stdout_success
+from itertools import repeat
 import os
 import shap
 import numpy as np
 from concurrent.futures import ProcessPoolExecutor
 from simba.utils.warnings import NotEnoughDataWarning
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
-from joblib import Parallel, delayed
-import multiprocessing
-import functools
-import concurrent
 
 
 
 
 def _create_shap_mp_helper(data: pd.DataFrame,
-                           explainer: shap.TreeExplainer,
-                           clf_name: str,
-                           rf_clf: RandomForestClassifier,
-                           expected_value: float):
+                    clf_name: str,
+                    explainer: shap.TreeExplainer,
+                    clf: RandomForestClassifier,
+                    expected_value: float):
 
     target = data.pop(clf_name).values.reshape(-1, 1)
     frame_batch_shap = explainer.shap_values(data.values, check_additivity=False)[1]
     shap_sum = np.sum(frame_batch_shap, axis=1).reshape(-1, 1)
-    proba = rf_clf.predict_proba(data)[:, 1].reshape(-1, 1)
+    proba = clf.predict_proba(data)[:, 1].reshape(-1, 1)
     frame_batch_shap = np.hstack((frame_batch_shap, np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, target))
     return frame_batch_shap, data.values[0]
 
 def create_shap_log_mp(ini_file_path: str,
                        rf_clf: RandomForestClassifier,
                        x_df: pd.DataFrame,
                        y_df: pd.DataFrame,
@@ -87,69 +84,71 @@
         cnt_absent = len(nontarget_df)
     non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
     targets_for_shap = target_df.sample(cnt_present, replace=False)
     explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
     expected_value = explainer.expected_value[1]
     cores, _ = find_core_cnt()
     shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
-    if (len(shap_data_df) / batch_size) < 1: batch_size = 1
+    if (len(shap_data_df) / batch_size) < 1:
+        batch_size = 1
+    elif (len(shap_data_df) > 100) & (save_it >= 100):
+        batch_size = 100
     shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
     shap_results, shap_raw, processed_counter = [], [], 0
-    with concurrent.futures.ProcessPoolExecutor(max_workers=cores) as executor:
-        futures = [executor.submit(_create_shap_mp_helper, data, explainer, clf_name, rf_clf, expected_value) for data in shap_data]
-        for future in concurrent.futures.as_completed(futures):
-            shap_results.append(future.result()[0])
-            shap_raw.append(future.result()[1])
-            print(shap_raw)
-            processed_counter += future.result()[0].shape[0]
+    with ProcessPoolExecutor(int(np.ceil(cores / 2))) as pool:
+        for it_cnt, res in enumerate(pool.map(_create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
+            shap_values, raw_values = res
+            shap_results.append(shap_values); shap_raw.append(raw_values)
+            processed_counter += shap_values.shape[0]
             if (processed_counter != 0) and (processed_counter % save_it == 0) or (processed_counter == len(shap_data_df)):
                 print(f'Saving SHAP data after {processed_counter} iterations...')
                 shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
                 raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
-                print(raw_save_df)
                 shap_save_df.to_csv(out_df_shap_path)
                 raw_save_df.to_csv(out_df_raw_path)
             print(f'SHAP frame: {processed_counter} / {len(shap_data_df)}...')
 
     shap_timer.stop_timer()
     stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
     _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                           classifier_name=clf_name,
                                           shap_df=shap_save_df,
                                           shap_baseline_value=int(expected_value * 100),
                                           save_path=save_path)
 
-data_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/targets_inserted/122_SA_Day_03_20200705T1429.csv'
-data_df = pd.read_csv(data_path, index_col=0)
-clf_names = ['Attack', 'Escape', 'Defensive']
-# data_cols = [x for x in data_df.columns if not 'Probability_' in x]
-# data_cols = [x for x in data_cols if not x is 'Escape']
-# data_cols = [x for x in data_cols if not x is 'Defensive']
-data_df = data_df[list(data_df.columns)[:-2]]
-
-config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
-
-x_df = data_df.drop(config.bp_col_names, axis=1)
-y_df = x_df.pop('Attack')
-
-ini_file_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini'
-rf_clf = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/models/generated_models/Attack.sav', file_type='pickle')
 
+if __name__ == '__main__':
+    data_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/targets_inserted/122_SA_Day_03_20200705T1429.csv'
+    data_df = pd.read_csv(data_path, index_col=0)
+    clf_names = ['Attack', 'Escape', 'Defensive']
+    # data_cols = [x for x in data_df.columns if not 'Probability_' in x]
+    # data_cols = [x for x in data_cols if not x is 'Escape']
+    # data_cols = [x for x in data_cols if not x is 'Defensive']
+    data_df = data_df[list(data_df.columns)[:-2]]
+
+    config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
+
+    x_df = data_df.drop(config.bp_col_names, axis=1)
+    y_df = x_df.pop('Attack')
+
+    ini_file_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini'
+    rf_clf = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/models/generated_models/Attack.sav', file_type='pickle')
 
 
-create_shap_log_mp(ini_file_path=ini_file_path,
-                rf_clf=rf_clf,
-                x_df=x_df,
-                y_df=y_df,
-                x_names=x_df.columns,
-                clf_name='Attack',
-                cnt_present=100,
-                cnt_absent=100,
-                save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models',
-                save_it=10)
+
+    create_shap_log_mp(ini_file_path=ini_file_path,
+                    rf_clf=rf_clf,
+                    x_df=x_df,
+                    y_df=y_df,
+                    x_names=x_df.columns,
+                    clf_name='Attack',
+                    cnt_present=100,
+                    cnt_absent=100,
+                    save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models',
+                    save_it=1000)
 
 
 # def create_shap_log(self,
 #                     ini_file_path: str,
 #                     rf_clf: RandomForestClassifier,
 #                     x_df: pd.DataFrame,
 #                     y_df: pd.DataFrame,
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import pandas as pd
 from sklearn.ensemble import RandomForestClassifier
 from simba.utils.read_write import read_df
 from typing import List, Optional
 from simba.utils.read_write import find_core_cnt
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.printing import SimbaTimer, stdout_success
-from itertools import repeat
 import os
 import shap
 import numpy as np
-from concurrent.futures import ProcessPoolExecutor
 from simba.utils.warnings import NotEnoughDataWarning
 from simba.plotting.shap_agg_stats_visualizer import ShapAggregateStatisticsVisualizer
-
-
-
+import multiprocessing
+import functools
 
 def _create_shap_mp_helper(data: pd.DataFrame,
-                    clf_name: str,
-                    explainer: shap.TreeExplainer,
-                    clf: RandomForestClassifier,
-                    expected_value: float):
+                           explainer: shap.TreeExplainer,
+                           clf_name: str):
 
     target = data.pop(clf_name).values.reshape(-1, 1)
-    frame_batch_shap = explainer.shap_values(data.values, check_additivity=False)[1]
-    shap_sum = np.sum(frame_batch_shap, axis=1).reshape(-1, 1)
-    proba = clf.predict_proba(data)[:, 1].reshape(-1, 1)
-    frame_batch_shap = np.hstack((frame_batch_shap, np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, target))
-    return frame_batch_shap, data.values[0]
+    group_cnt = data.pop('group').values[0]
+    shap_vals = np.full((len(data), len(data.columns)), np.nan)
+    for cnt, i in enumerate(list(data.index)):
+        shap_vals[cnt] = explainer.shap_values(data.loc[i].values, check_additivity=False)[1]
+        print(f'SHAP complete core frame: {i} (CORE BATCH: {group_cnt})')
+    return shap_vals, data.values, target
+
+def split_and_group_df(df: pd.DataFrame,
+                       splits: int,
+                       include_split_order: bool = True) -> (List[pd.DataFrame], int):
+
+    """
+    Helper to split a dataframe for multiprocessing. If include_split_order, then include the group number
+    in split data as a column. Returns split data and approximations of number of observations per split.
+    """
+    data_arr = np.array_split(df, splits)
+    if include_split_order:
+        for df_cnt in range(len(data_arr)):
+            data_arr[df_cnt]['group'] = df_cnt
+    obs_per_split = len(data_arr[0])
+    return data_arr, obs_per_split
 
 def create_shap_log_mp(ini_file_path: str,
                        rf_clf: RandomForestClassifier,
                        x_df: pd.DataFrame,
                        y_df: pd.DataFrame,
                        x_names: List[str],
                        clf_name: str,
                        cnt_present: int,
                        cnt_absent: int,
                        save_path: str,
                        batch_size: int = 10,
-                       save_it: int = 100,
                        save_file_no: Optional[int] = None) -> None:
     """
     Helper to compute SHAP values using multiprocessing.
     For single-core alternative, see  meth:`simba.mixins.train_model_mixins.TrainModelMixin.create_shap_log_mp`.
 
     .. seealso::
        `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
@@ -86,69 +96,69 @@
     targets_for_shap = target_df.sample(cnt_present, replace=False)
     explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
     expected_value = explainer.expected_value[1]
     cores, _ = find_core_cnt()
     shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
     if (len(shap_data_df) / batch_size) < 1:
         batch_size = 1
-    elif (len(shap_data_df) > 100) & (save_it >= 100):
+    if (len(shap_data_df) > 100):
         batch_size = 100
-    shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
-    shap_results, shap_raw, processed_counter = [], [], 0
-    with ProcessPoolExecutor(int(np.ceil(cores / 2))) as pool:
-        for it_cnt, res in enumerate(pool.map(_create_shap_mp_helper, shap_data, repeat(clf_name), repeat(explainer), repeat(rf_clf), repeat(expected_value))):
-            shap_values, raw_values = res
-            shap_results.append(shap_values); shap_raw.append(raw_values)
-            processed_counter += shap_values.shape[0]
-            if (processed_counter != 0) and (processed_counter % save_it == 0) or (processed_counter == len(shap_data_df)):
-                print(f'Saving SHAP data after {processed_counter} iterations...')
-                shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
-                raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
-                shap_save_df.to_csv(out_df_shap_path)
-                raw_save_df.to_csv(out_df_raw_path)
-            print(f'SHAP frame: {processed_counter} / {len(shap_data_df)}...')
-
+    shap_data, _ = split_and_group_df(df=shap_data_df, splits=int(len(shap_data_df) / batch_size))
+    shap_results, shap_raw = [], []
+    with multiprocessing.Pool(cores, maxtasksperchild=10) as pool:
+        constants = functools.partial(_create_shap_mp_helper,
+                                      explainer=explainer,
+                                      clf_name=clf_name)
+        for cnt, result in enumerate(pool.imap_unordered(constants, shap_data, chunksize=10)):
+            print(f'Concatenating multi-processed SHAP data (batch {cnt+1}/{len(shap_data)}')
+            proba = rf_clf.predict_proba(result[1])[:, 1].reshape(-1, 1)
+            shap_sum = np.sum(result[0], axis=1).reshape(-1, 1)
+            shap_results.append(np.hstack((result[0], np.full((result[0].shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, result[2])))
+            shap_raw.append(result[1])
+            shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
+            raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
+            shap_save_df.to_csv(out_df_shap_path)
+            raw_save_df.to_csv(out_df_raw_path)
+    pool.terminate()
+    pool.join()
     shap_timer.stop_timer()
     stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
     _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                           classifier_name=clf_name,
                                           shap_df=shap_save_df,
                                           shap_baseline_value=int(expected_value * 100),
                                           save_path=save_path)
 
-
-if __name__ == '__main__':
-    data_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/targets_inserted/122_SA_Day_03_20200705T1429.csv'
-    data_df = pd.read_csv(data_path, index_col=0)
-    clf_names = ['Attack', 'Escape', 'Defensive']
-    # data_cols = [x for x in data_df.columns if not 'Probability_' in x]
-    # data_cols = [x for x in data_cols if not x is 'Escape']
-    # data_cols = [x for x in data_cols if not x is 'Defensive']
-    data_df = data_df[list(data_df.columns)[:-2]]
-
-    config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
-
-    x_df = data_df.drop(config.bp_col_names, axis=1)
-    y_df = x_df.pop('Attack')
-
-    ini_file_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini'
-    rf_clf = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/models/generated_models/Attack.sav', file_type='pickle')
+data_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/targets_inserted/122_SA_Day_03_20200705T1429.csv'
+data_df = pd.read_csv(data_path, index_col=0)
+clf_names = ['Attack', 'Escape', 'Defensive']
+# data_cols = [x for x in data_df.columns if not 'Probability_' in x]
+# data_cols = [x for x in data_cols if not x is 'Escape']
+# data_cols = [x for x in data_cols if not x is 'Defensive']
+data_df = data_df[list(data_df.columns)[:-2]]
+
+config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini')
+
+x_df = data_df.drop(config.bp_col_names, axis=1)
+y_df = x_df.pop('Attack')
+
+ini_file_path = '/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini'
+rf_clf = read_df(file_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/models/generated_models/Attack.sav', file_type='pickle')
 
 
 
-    create_shap_log_mp(ini_file_path=ini_file_path,
-                    rf_clf=rf_clf,
-                    x_df=x_df,
-                    y_df=y_df,
-                    x_names=x_df.columns,
-                    clf_name='Attack',
-                    cnt_present=100,
-                    cnt_absent=100,
-                    save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models',
-                    save_it=1000)
+create_shap_log_mp(ini_file_path=ini_file_path,
+                rf_clf=rf_clf,
+                x_df=x_df,
+                y_df=y_df,
+                x_names=x_df.columns,
+                clf_name='Attack',
+                cnt_present=100,
+                cnt_absent=100,
+                save_path='/Users/simon/Desktop/envs/troubleshooting/unsupervised/dr_models')
 
 
 # def create_shap_log(self,
 #                     ini_file_path: str,
 #                     rf_clf: RandomForestClassifier,
 #                     x_df: pd.DataFrame,
 #                     y_df: pd.DataFrame,
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.62.4/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.62.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/pop_up_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,14 @@
 
     def remove_from_listbox(self,
                             list_box: Listbox):
         selection = list_box.curselection()
         if selection:
             list_box.delete(selection[0])
 
-
     def create_choose_bp_frm(self, project_body_parts, run_function):
         if hasattr(self, 'body_part_frm'):
             self.body_part_frm.destroy()
         self.body_parts_dropdowns = {}
         self.body_part_frm = LabelFrame(self.main_frm, text="CHOOSE ANIMAL BODY-PARTS", font=Formats.LABELFRAME_HEADER_FORMAT.value, name='choose animal body-parts')
         self.body_part_frm.grid(row=self.children_cnt_main(), sticky=NW)
         for bp_cnt in range(int(self.bp_cnt_dropdown.getChoices())):
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.4/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/feature_extraction_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
         :parameter int fps: The frame-rate of the video representing the data.
         :parameter int time_window: Time-window in milliseconds to use for Gaussian smoothing.
         :return pd.DataFrame: Dataframe with smoothened data
         """
 
         frames_in_time_window = int(time_window / (1000 / fps))
         for c in df.columns:
-            df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
+            df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs().astype(int)
         return df
 
 
     def dataframe_savgol_smoother(self,
                                   df: pd.DataFrame,
                                   fps: int,
                                   time_window: int = 150) -> pd.DataFrame:
@@ -625,15 +625,15 @@
         :parameter int time_window: Time-window in milliseconds to use for Gaussian smoothing.
         :return pd.DataFrame: Dataframe with smoothened data
         """
         frames_in_time_window = int(time_window / (1000 / fps))
         if (frames_in_time_window % 2) == 0: frames_in_time_window = frames_in_time_window - 1
         if (frames_in_time_window % 2) <= 3: frames_in_time_window = 5
         for c in df.columns:
-            df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
+            df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest').astype(int)
         return df
 
     def get_bp_headers(self) -> None:
         """
         Helper to create ordered list of all column header fields for SimBA project dataframes.
         """
         self.col_headers = []
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.62.4/simba/mixins/train_model_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 __author__ = "Simon Nilsson"
 
+
+import warnings
+warnings.simplefilter(action='ignore', category=FutureWarning)
+
 import os
 import numpy as np
 import pandas as pd
 from sklearn.inspection import partial_dependence
 from imblearn.combine import SMOTEENN
 from imblearn.over_sampling import SMOTE
 from sklearn.inspection import permutation_importance
-from sklearn.model_selection import learning_curve
-from sklearn.model_selection import ShuffleSplit
+from sklearn.model_selection import learning_curve, ShuffleSplit
 from sklearn.metrics import precision_recall_curve
 from sklearn.ensemble import RandomForestClassifier
 from copy import deepcopy
 from sklearn.tree import export_graphviz
 from subprocess import call
 from yellowbrick.classifier import ClassificationReport
 from datetime import datetime
@@ -25,14 +28,15 @@
 import platform
 from sklearn.utils import parallel_backend
 import pickle
 import concurrent
 from dtreeviz.trees import tree, dtreeviz
 import matplotlib.pyplot as plt
 import multiprocessing
+import functools
 from typing import List, Optional, Union, Dict, Any
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 from simba.utils.enums import ConfigKey, Dtypes, MetaKeys, Defaults
@@ -51,15 +55,16 @@
                                 CorruptedFileError,
                                 FeatureNumberMismatchError,
                                 ClassifierInferenceError,
                                 InvalidInputError)
 from simba.utils.warnings import (NotEnoughDataWarning,
                                   NoModuleWarning,
                                   MissingUserInputWarning,
-                                  MultiProcessingFailedWarning)
+                                  MultiProcessingFailedWarning,
+                                  ShapWarning)
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.lookups import get_meta_data_file_headers
 plt.switch_backend('agg')
 
 class TrainModelMixin(object):
     """ Train model methods"""
     def __init__(self):
@@ -139,15 +144,15 @@
                 annotation_cols_to_remove.append(model_name)
         return annotation_cols_to_remove
 
     def delete_other_annotation_columns(self,
                                         df: pd.DataFrame,
                                         annotations_lst: List[str]) -> pd.DataFrame:
         """
-        Helper to delete fields that contain annotations which are not the target.
+        Helper to drop fields that contain annotations which are not the target.
 
         :parameter pd.DataFrame df: Dataframe holding features and annotations.
         :parameter List[str] annotations_lst: column fields to be removed from df
         :return pd.DataFrame: Dataframe without non-target annotation columns
 
         :examples:
         >>> self.delete_other_annotation_columns(df=df, annotations_lst=['Sniffing'])
@@ -541,14 +546,31 @@
                                 label_fontsize=12, ticks_fontsize=8, fontname="Arial")
             save_path = os.path.join(save_dir, clf_name + '_fancy_decision_tree_example.svg')
             svg_tree.save(save_path)
         except:
             NoModuleWarning(
                 msg='Skipping dtreeviz example decision tree visualization. Make sure "graphviz" is installed.')
 
+    @staticmethod
+    def split_and_group_df(df: pd.DataFrame,
+                           splits: int,
+                           include_split_order: bool = True) -> (List[pd.DataFrame], int):
+
+        """
+        Helper to split a dataframe for multiprocessing. If include_split_order, then include the group number
+        in split data as a column. Returns split data and approximations of number of observations per split.
+        """
+        data_arr = np.array_split(df, splits)
+        if include_split_order:
+            for df_cnt in range(len(data_arr)):
+                data_arr[df_cnt]['group'] = df_cnt
+        obs_per_split = len(data_arr[0])
+        return data_arr, obs_per_split
+
+
     def create_shap_log(self,
                         ini_file_path: str,
                         rf_clf: RandomForestClassifier,
                         x_df: pd.DataFrame,
                         y_df: pd.DataFrame,
                         x_names: List[str],
                         clf_name: str,
@@ -581,15 +603,15 @@
         :param int cnt_absent: Number of behavior-absent frames to calculate SHAP values for.
         :param str save_path: Directory where to save output in csv file format.
         :param Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
 
         """
 
-        print('Calculating SHAP values...')
+        print('Calculating SHAP values (SINGLE CORE)...')
         shap_timer = SimbaTimer(start=True)
         data_df = pd.concat([x_df, y_df], axis=1)
         if save_file_no == None:
             out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
             out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
         else:
             out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
@@ -695,15 +717,14 @@
 
         :parameter RandomForestClassifier rf_clf: sklearn random forest classifier
         :parameter str clf_name: Classifier name
         :parameter str save_dir: Directory where to save output in csv file format.
         :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
         """
-
         if save_file_no != None:
             save_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no) + '.sav')
         else:
             save_path = os.path.join(save_dir, clf_name + '.sav')
         pickle.dump(rf_clf, open(save_path, 'wb'))
 
     def get_model_info(self,
@@ -1161,26 +1182,38 @@
         target = data.pop(clf_name).values.reshape(-1, 1)
         frame_batch_shap = explainer.shap_values(data.values, check_additivity=False)[1]
         shap_sum = np.sum(frame_batch_shap, axis=1).reshape(-1, 1)
         proba = rf_clf.predict_proba(data)[:, 1].reshape(-1, 1)
         frame_batch_shap = np.hstack((frame_batch_shap, np.full((frame_batch_shap.shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, target))
         return frame_batch_shap, data.values
 
+    @staticmethod
+    def _create_shap_mp_helper(data: pd.DataFrame,
+                               explainer: shap.TreeExplainer,
+                               clf_name: str):
+
+        target = data.pop(clf_name).values.reshape(-1, 1)
+        group_cnt = data.pop('group').values[0]
+        shap_vals = np.full((len(data), len(data.columns)), np.nan)
+        for cnt, i in enumerate(list(data.index)):
+            shap_vals[cnt] = explainer.shap_values(data.loc[i].values, check_additivity=False)[1]
+            print(f'SHAP complete core frame: {i} (CORE BATCH: {group_cnt})')
+        return shap_vals, data.values, target
+
     def create_shap_log_mp(self,
                            ini_file_path: str,
                            rf_clf: RandomForestClassifier,
                            x_df: pd.DataFrame,
                            y_df: pd.DataFrame,
                            x_names: List[str],
                            clf_name: str,
                            cnt_present: int,
                            cnt_absent: int,
                            save_path: str,
                            batch_size: int = 10,
-                           save_it: int = 100,
                            save_file_no: Optional[int] = None) -> None:
         """
         Helper to compute SHAP values using multiprocessing.
         For single-core alternative, see  meth:`simba.mixins.train_model_mixins.TrainModelMixin.create_shap_log_mp`.
 
         .. seealso::
            `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
@@ -1198,67 +1231,83 @@
         :param int cnt_present: Number of behavior-present frames to calculate SHAP values for.
         :param int cnt_absent: Number of behavior-absent frames to calculate SHAP values for.
         :param str save_dir: Directory where to save output in csv file format.
         :param Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
 
         """
-
-        print('Calculating SHAP values...')
+        print(f'Computing {len(x_df)} SHAP values (MULTI-CORE, FOLLOW PROGRESS IN OS TERMINAL)...')
         shap_timer = SimbaTimer(start=True)
         data_df = pd.concat([x_df, y_df], axis=1)
         if save_file_no == None:
             out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
             out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
         else:
             out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
             out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
         target_df, nontarget_df = data_df[data_df[y_df.name] == 1], data_df[data_df[y_df.name] == 0]
         if len(target_df) < cnt_present:
-            NotEnoughDataWarning(
-                msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
+            NotEnoughDataWarning(msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
             cnt_present = len(target_df)
         if len(nontarget_df) < cnt_absent:
-            NotEnoughDataWarning(
-                msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
+            NotEnoughDataWarning(msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
             cnt_absent = len(nontarget_df)
         non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
         targets_for_shap = target_df.sample(cnt_present, replace=False)
-        explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw',
-                                       feature_perturbation='tree_path_dependent')
+        explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
         expected_value = explainer.expected_value[1]
         cores, _ = find_core_cnt()
         shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
         if (len(shap_data_df) / batch_size) < 1:
             batch_size = 1
-        elif (len(shap_data_df) > 100) & (save_it >= 100):
+        if (len(shap_data_df) > 100):
             batch_size = 100
-
-        shap_data = np.array_split(shap_data_df, len(shap_data_df) / batch_size)
-        shap_results, shap_raw, processed_counter = [], [], 0
-        with concurrent.futures.ProcessPoolExecutor(max_workers=cores) as executor:
-            futures = [executor.submit(self._create_shap_mp_helper, data, explainer, clf_name, rf_clf, expected_value) for data in shap_data]
-            for future in concurrent.futures.as_completed(futures):
-                shap_results.append(future.result()[0]); shap_raw.append(future.result()[1])
-                processed_counter += future.result()[0].shape[0]
-                if (processed_counter != 0) and (processed_counter % save_it == 0) or (processed_counter == len(shap_data_df)):
-                    print(f'Saving SHAP data after {processed_counter} iterations...')
-                    shap_save_df = pd.DataFrame(data=np.row_stack(shap_results), columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability', clf_name])
+        shap_data, _ = self.split_and_group_df(df=shap_data_df, splits=int(len(shap_data_df) / batch_size))
+        shap_results, shap_raw = [], []
+        try:
+            with multiprocessing.Pool(cores, maxtasksperchild=10) as pool:
+                constants = functools.partial(self._create_shap_mp_helper,
+                                              explainer=explainer,
+                                              clf_name=clf_name)
+                for cnt, result in enumerate(pool.imap_unordered(constants, shap_data, chunksize=10)):
+                    print(f'Concatenating multi-processed SHAP data (batch {cnt+1}/{len(shap_data)})')
+                    proba = rf_clf.predict_proba(result[1])[:, 1].reshape(-1, 1)
+                    shap_sum = np.sum(result[0], axis=1).reshape(-1, 1)
+                    shap_results.append(np.hstack((result[0], np.full((result[0].shape[0]), expected_value).reshape(-1, 1),
+                                                   shap_sum, proba, result[2])))
+                    shap_raw.append(result[1])
+                    shap_save_df = pd.DataFrame(data=np.row_stack(shap_results),
+                                                columns=list(x_names) + ['Expected_value', 'Sum', 'Prediction_probability',
+                                                                         clf_name])
                     raw_save_df = pd.DataFrame(data=np.row_stack(shap_raw), columns=list(x_names))
                     shap_save_df.to_csv(out_df_shap_path)
                     raw_save_df.to_csv(out_df_raw_path)
-                print(f'SHAP frame: {processed_counter} / {len(shap_data_df)}...')
+            pool.terminate()
+            pool.join()
+            shap_timer.stop_timer()
+            stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
+            _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
+                                                  classifier_name=clf_name,
+                                                  shap_df=shap_save_df,
+                                                  shap_baseline_value=int(expected_value * 100),
+                                                  save_path=save_path)
+        except:
+            ShapWarning(msg='Multiprocessing SHAP values failed. Revert to single core. This will negatively affect run-time. ')
+            self.create_shap_log(ini_file_path=ini_file_path,
+                                 rf_clf=rf_clf,
+                                 x_df=x_df,
+                                 y_df=y_df,
+                                 x_names=x_names,
+                                 clf_name=clf_name,
+                                 cnt_present=cnt_present,
+                                 cnt_absent=cnt_absent,
+                                 save_path=save_path,
+                                 save_it=len(x_df),
+                                 save_file_no=save_file_no)
 
-        shap_timer.stop_timer()
-        stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
-        _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
-                                              classifier_name=clf_name,
-                                              shap_df=shap_save_df,
-                                              shap_baseline_value=int(expected_value * 100),
-                                              save_path=save_path)
 
 # test = TrainModelMixin()
 # test.read_all_files_in_folder(file_paths=['/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437C_c3_2022-11-01_13-16-23_color.csv', '/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437D_c4_2022-11-01_13-16-39_color.csv'],
 #                               file_type='csv', classifier_names=['attack', 'non-agresive parallel swimming'])
 
 
 # test = TrainModelMixin()
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.62.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/enums.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     RF_METADATA = 'RF_meta_data'
     LEARNING_CURVE_K_SPLITS = 'LearningCurve_shuffle_k_splits'
     LEARNING_DATA_SPLITS = 'LearningCurve_shuffle_data_splits'
     IMPORTANCE_BARS_N = 'N_feature_importance_bars'
     SHAP_PRESENT = 'shap_target_present_no'
     SHAP_ABSENT = 'shap_target_absent_no'
     SHAP_SAVE_ITERATION = 'shap_save_iteration'
+    SHAP_MULTIPROCESS = 'shap_multiprocess'
     POSE_SETTING = 'pose_estimation_body_parts'
     RF_JOBS = 'RF_n_jobs'
     VALIDATION_VIDEO = 'generate_validation_video'
     MOVEMENT_CRITERION = 'movement_criterion'
     LOCATION_CRITERION = 'location_criterion'
     ROI_ANIMAL_CNT = 'no_of_animals'
     DISTANCE_MM = 'distance_mm'
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/utils/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
-00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
+00000000: 0000 0001 4275 6431 0000 2000 0000 0800  ....Bud1.. .....
+00000010: 0000 2000 0000 100c 0000 0000 0000 0000  .. .............
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 000a  ................
-00000050: 0000 0001 0000 1000 7370 626c 6f62 0000  ........spblob..
-00000060: 00ca 6270 0000 0000 0000 0000 0000 0000  ..bp............
+00000040: 0000 0000 0000 0002 0000 0000 0000 000e  ................
+00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
+00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,144 +250,144 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 000a 0000 0003  ................
-00001010: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
-00001020: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-00001030: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-00001040: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00001050: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00001060: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001070: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00001080: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00001090: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-000010a0: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
-000010b0: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
-000010c0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
-000010d0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-000010e0: 0000 0000 0000 0000 0000 009b 0000 0003  ................
-000010f0: 0063 006c 0069 6c67 3153 636f 6d70 0000  .c.l.ilg1Scomp..
-00001100: 0000 0000 0c9b 0000 0003 0063 006c 0069  ...........c.l.i
-00001110: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
-00001120: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00001130: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
-00001140: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001150: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001160: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00001170: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00001180: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00001190: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-000011a0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-000011b0: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
-000011c0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
-000011d0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-000011e0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-000011f0: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
-00001200: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-00001210: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
-00001220: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
-00001230: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
-00001240: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
-00001250: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
-00001260: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
-00001270: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
-00001280: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
-00001290: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
-000012a0: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
-000012b0: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
-000012c0: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
-000012d0: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
-000012e0: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-000012f0: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
-00001300: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
-00001310: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
-00001320: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
-00001330: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
-00001340: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
-00001350: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
-00001360: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
-00001370: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
-00001380: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
-00001390: da01 db00 0000 0000 0002 0100 0000 0000  ................
-000013a0: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-000013b0: 0001 dd00 0000 0300 6300 6c00 696c 7376  ........c.l.ilsv
-000013c0: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-000013d0: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
-000013e0: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
-000013f0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00001400: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00001410: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00001420: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00001430: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00001440: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001450: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
-00001460: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-00001470: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00001480: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-00001490: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-000014a0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-000014b0: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-000014c0: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
-000014d0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-000014e0: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
-000014f0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
-00001500: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-00001510: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-00001520: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-00001530: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-00001540: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00001550: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00001560: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00001570: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00001580: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00001590: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-000015a0: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-000015b0: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-000015c0: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-000015d0: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-000015e0: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-000015f0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-00001600: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-00001610: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-00001620: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
-00001630: 696d 6f44 4462 6c6f 6200 0000 0855 3191  imoDDblob....U1.
-00001640: f9a1 0cc5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
-00001650: 6f64 4462 6c6f 6200 0000 0855 3191 f9a1  odDblob....U1...
-00001660: 0cc5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
-00001670: 5363 6f6d 7000 0000 0000 0010 0000 0000  Scomp...........
-00001680: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
-00001690: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
-000016a0: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
-000016b0: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
-000016c0: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
-000016d0: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
-000016e0: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
-000016f0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
-00001700: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
-00001710: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
-00001720: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
-00001730: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
-00001740: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
-00001750: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
-00001760: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
-00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
-00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
+00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
+00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00001030: 0000 0002 021a 0000 000b 005f 005f 0070  ..........._._.p
+00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00001050: 6d6f 4444 626c 6f62 0000 0008 0879 c913  moDDblob.....y..
+00001060: 6814 c541 0000 000b 005f 005f 0070 0079  h..A....._._.p.y
+00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00001080: 6444 626c 6f62 0000 0008 0879 c913 6814  dDblob.....y..h.
+00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000010b0: 636f 6d70 0000 0000 0002 5000 0000 0003  comp......P.....
+000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
+000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00001100: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00001110: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001120: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001130: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00001140: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+00001150: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
+00001160: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
+00001170: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
+00001180: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+00001190: 0000 0000 0000 0000 0000 009b 0000 0003  ................
+000011a0: 0063 006c 0069 6c67 3153 636f 6d70 0000  .c.l.ilg1Scomp..
+000011b0: 0000 0000 22e5 0000 0003 0063 006c 0069  ...."......c.l.i
+000011c0: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
+000011d0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+000011e0: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
+000011f0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00001200: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00001210: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00001220: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00001230: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001240: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00001250: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+00001260: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
+00001270: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
+00001280: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+00001290: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+000012a0: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
+000012b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+000012c0: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
+000012d0: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
+000012e0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+000012f0: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
+00001300: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
+00001310: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
+00001320: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
+00001330: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
+00001340: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
+00001350: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
+00001360: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
+00001370: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+00001380: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
+00001390: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+000013a0: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
+000013b0: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
+000013c0: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
+000013d0: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
+000013e0: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
+000013f0: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
+00001400: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
+00001410: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
+00001420: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
+00001430: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
+00001440: da01 db00 0000 0000 0002 0100 0000 0000  ................
+00001450: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
+00001460: 0001 dd00 0000 0300 6300 6c00 696c 7376  ........c.l.ilsv
+00001470: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
+00001480: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
+00001490: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
+000014a0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+000014b0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+000014c0: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+000014d0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+000014e0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000014f0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001500: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
+00001510: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
+00001520: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
+00001530: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
+00001540: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+00001550: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+00001560: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
+00001570: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
+00001580: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+00001590: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
+000015a0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
+000015b0: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
+000015c0: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
+000015d0: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
+000015e0: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
+000015f0: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
+00001600: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
+00001610: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
+00001620: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
+00001630: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
+00001640: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
+00001650: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
+00001660: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
+00001670: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
+00001680: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
+00001690: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
+000016a0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
+000016b0: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
+000016c0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+000016d0: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
+000016e0: 696d 6f44 4462 6c6f 6200 0000 0834 2b08  imoDDblob....4+.
+000016f0: c0c8 11c5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
+00001700: 6f64 4462 6c6f 6200 0000 0834 2b08 c0c8  odDblob....4+...
+00001710: 11c5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
+00001720: 5363 6f6d 7000 0000 0000 0040 0000 0000  Scomp......@....
+00001730: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
+00001740: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
+00001750: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
+00001760: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
+00001770: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
+00001780: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
+00001790: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
+000017a0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
+000017b0: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
+000017c0: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
+000017d0: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
+000017e0: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
+000017f0: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
+00001800: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
+00001810: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -442,72 +442,200 @@
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001c50: 0100 0002 0000 0000 0100 0004 0000 0000  ................
-00001c60: 0100 0008 0000 0000 0000 0000 0100 0020  ............... 
-00001c70: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
-00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
-00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
-00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
-00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
-00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
-00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
-00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 00d4 1617  .....@..........
-00001d00: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-00001d10: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-00001d20: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-00001d30: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-00001d40: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00001d50: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00001d60: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00001d70: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00001d80: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00001d90: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-00001da0: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-00001db0: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-00001dc0: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-00001dd0: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-00001de0: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-00001df0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-00001e00: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-00001e10: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-00001e20: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
-00001e30: 696d 6f44 4462 6c6f 6200 0000 0855 3191  imoDDblob....U1.
-00001e40: f9a1 0cc5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
-00001e50: 6f64 4462 6c6f 6200 0000 0855 3191 f9a1  odDblob....U1...
-00001e60: 0cc5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
-00001e70: 5363 6f6d 7000 0000 0000 0010 0000 0000  Scomp...........
-00001e80: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
-00001e90: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
-00001ea0: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
-00001eb0: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
-00001ec0: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
-00001ed0: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
-00001ee0: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
-00001ef0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
-00001f00: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
-00001f10: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
-00001f20: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
-00001f30: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
-00001f40: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
-00001f50: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
-00001f60: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
+00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000                                ....
+00002000: 0000 0000 0000 0003 0000 0000 0000 200b  .............. .
+00002010: 0000 0045 0000 100c 0000 0000 0000 0000  ...E............
+00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000020f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000022f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000023f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00002410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00002420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+00002440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00002450: 0100 0002 0000 0000 0100 0004 0000 0000  ................
+00002460: 0200 0008 0000 0028 0000 0000 0100 0030  .......(.......0
+00002470: 0000 0000 0000 0000 0100 0040 0000 0000  ...........@....
+00002480: 0100 0080 0000 0000 0100 0100 0000 0000  ................
+00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
+000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
+000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
+000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
+000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
+000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
+000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
+00002500: 0073 696f 6e23 4030 0000 0000 0000 09d9  .sion#@0........
+00002510: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
+00002520: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
+00002530: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
+00002540: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+00002550: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+00002560: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
+00002570: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
+00002580: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+00002590: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
+000025a0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
+000025b0: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
+000025c0: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
+000025d0: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
+000025e0: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
+000025f0: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
+00002600: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
+00002610: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
+00002620: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
+00002630: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
+00002640: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
+00002650: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
+00002660: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
+00002670: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
+00002680: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
+00002690: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
+000026a0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
+000026b0: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
+000026c0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
+000026d0: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
+000026e0: 696d 6f44 4462 6c6f 6200 0000 0834 2b08  imoDDblob....4+.
+000026f0: c0c8 11c5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
+00002700: 6f64 4462 6c6f 6200 0000 0834 2b08 c0c8  odDblob....4+...
+00002710: 11c5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
+00002720: 5363 6f6d 7000 0000 0000 0040 0000 0000  Scomp......@....
+00002730: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
+00002740: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
+00002750: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
+00002760: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
+00002770: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
+00002780: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
+00002790: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
+000027a0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
+000027b0: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
+000027c0: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
+000027d0: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
+000027e0: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
+000027f0: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
+00002800: 0b00 7700                                ..w.
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/checks.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/lookups.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,30 @@
 import re
 import struct
 import simba
 from typing import List
 from simba.utils.enums import Paths, Methods
 from simba.utils.checks import check_file_exist_and_readable, check_if_dir_exists
 from simba.utils.read_write import get_fn_ext
+from multiprocessing import Process, Value, Lock
 
 
+class SharedCounter(object):
+    def __init__(self, initval=0):
+        self.val = Value('i', initval)
+        self.lock = Lock()
+
+    def increment(self):
+        with self.lock:
+            self.val.value += 1
+
+    def value(self):
+        with self.lock:
+            return self.val.value
+
 def get_body_part_configurations() -> dict:
 
     """
     Return dict with named body-part schematics of pose-estimation schemas in SimBA installation as keys,
     and paths to the images representing those body-part schematics as values.
     """
 
@@ -230,8 +244,10 @@
             'darkgoldenrod',
             'olive',
             'seagreen',
             'dodgerblue',
             'springgreen',
             'firebrick',
             'indigo'
-            'white']
+            'white']
+
+
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/data.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.62.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/single_run_model_validation_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 from typing import Dict, Any
 
 from simba.utils.data import plug_holes_shortest_bout
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import read_df, write_df, get_fn_ext, get_video_meta_data
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
+from simba.mixins.train_model_mixin import TrainModelMixin
 
 plt.interactive(True)
 plt.ioff()
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
-class ValidateModelOneVideo(ConfigReader, PlottingMixin):
+class ValidateModelOneVideo(ConfigReader, PlottingMixin, TrainModelMixin):
     """
     Create classifier validation video for a single input video. Results are stored in the
     `project_folder/frames/output/validation directory`.
 
     .. note::
        For improved run-time, see :meth:`simba.sing_run_model_validation_video_mp.ValidateModelOneVideoMultiprocess` for multiprocess class.
 
@@ -57,30 +58,32 @@
                  discrimination_threshold: float,
                  shortest_bout: int,
                  create_gantt: str,
                  settings: Dict[str, Any]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
+        TrainModelMixin.__init__(self)
         _, self.feature_filename, ext = get_fn_ext(feature_file_path)
         self.discrimination_threshold, self.shortest_bout, self.create_gantt, self.settings = float(discrimination_threshold), shortest_bout, create_gantt, settings
         if not os.path.exists(self.single_validation_video_save_dir): os.makedirs(self.single_validation_video_save_dir)
         _, _, self.fps = self.read_video_info(video_name=self.feature_filename)
-        self.clf_name = os.path.basename(model_path).replace('.sav', '')
+        self.clf_name, self.feature_file_path = os.path.basename(model_path).replace('.sav', ''), feature_file_path
         self.video_path = self.find_video_of_file(self.video_dir, self.feature_filename)
         self.video_meta_data = get_video_meta_data(video_path=self.video_path)
         self.vid_output_path = os.path.join(self.single_validation_video_save_dir, f'{self.feature_filename} {self.clf_name}.avi')
         self.clf_data_save_path = os.path.join(self.clf_data_validation_dir, self.feature_filename + '.csv')
         self.clf = read_df(file_path=model_path, file_type='pickle')
+        print(feature_file_path)
         self.in_df = read_df(feature_file_path, self.file_type)
 
     def __run_clf(self):
         self.data_df = self.drop_bp_cords(df=self.in_df)
         self.prob_col_name = f'Probability_{self.clf_name}'
-        self.data_df[self.prob_col_name] = self.clf.predict_proba(self.data_df)[:, 1]
+        self.data_df[self.prob_col_name] = self.clf_predict_proba(clf=self.clf, x_df=self.data_df, model_name=self.clf_name, data_path=self.feature_file_path)
         self.data_df[self.clf_name] = np.where(self.data_df[self.prob_col_name] > self.discrimination_threshold, 1, 0)
 
     def __plug_bouts(self):
         self.data_df = plug_holes_shortest_bout(data_df=self.data_df, clf_name=self.clf_name, fps=self.fps, shortest_bout=self.shortest_bout)
 
     def __save(self):
         write_df(df=self.data_df, file_type=self.file_type, save_path=self.clf_data_save_path)
@@ -183,19 +186,14 @@
 #                              discrimination_threshold=0.6,
 #                              shortest_bout=50,
 #                              settings={'pose': True, 'animal_names': True, 'styles': None},
 #                              create_gantt='Gantt chart: final frame only (slightly faster)')
 # test.run()
 
 
-
-
-
-
-
 # test.perform_clf()
 # test.plug_small_bouts()
 # test.save_classification_data()
 # test.create_video()
 
 # test = ValidateModelOneVideo(ini_path='/Users/simon/Desktop/troubleshooting/Zebrafish/project_folder/project_config.ini',
 #                  feature_file_path=r'/Users/simon/Desktop/troubleshooting/Zebrafish/project_folder/csv/features_extracted/20200730_AB_7dpf_850nm_0002.csv',
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 import platform
 import functools
 import multiprocessing
 from typing import Dict, Any
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.plotting_mixin import PlottingMixin
+from simba.mixins.train_model_mixin import TrainModelMixin
 from simba.utils.data import plug_holes_shortest_bout
 from simba.utils.read_write import get_fn_ext, read_df, write_df, get_video_meta_data, concatenate_videos_in_folder
 from simba.utils.printing import stdout_success
 
 class ValidateModelOneVideoMultiprocess(ConfigReader,
-                                        PlottingMixin):
+                                        PlottingMixin,
+                                        TrainModelMixin):
     """
     Create classifier validation video for a single input video. Results are stored in the
     ``project_folder/frames/output/validation`` directory.
 
     :param str config_path: path to SimBA project config file in Configparser format
     :param str feature_file_path: path to SimBA file (parquet or CSV) containing pose-estimation and feature fields.
     :param str model_path: path to pickled classifier object
@@ -54,40 +56,38 @@
                  shortest_bout: int,
                  cores: int,
                  create_gantt: str,
                  settings: Dict[str, Any]):
 
         ConfigReader.__init__(self, config_path=config_path)
         PlottingMixin.__init__(self)
+        TrainModelMixin.__init__(self)
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
-
-
-
         _, self.feature_filename, ext = get_fn_ext(feature_file_path)
         self.discrimination_threshold, self.cores, self.shortest_bout, self.create_gantt, self.settings = float(discrimination_threshold), cores, shortest_bout, create_gantt, settings
         if self.create_gantt == 'None': self.create_gantt = None
         if not os.path.exists(self.single_validation_video_save_dir): os.makedirs(self.single_validation_video_save_dir)
         _, _, self.fps = self.read_video_info(video_name=self.feature_filename)
         self.clf_name = os.path.basename(model_path).replace('.sav', '')
         self.video_path = self.find_video_of_file(self.video_dir, self.feature_filename)
         self.clf_data_save_path = os.path.join(self.clf_data_validation_dir, self.feature_filename + '.csv')
         self.video_meta_data = get_video_meta_data(video_path=self.video_path)
         self.clf = read_df(file_path=model_path, file_type='pickle')
         self.in_df = read_df(feature_file_path, self.file_type)
+        self.feature_file_path = feature_file_path
         self.temp_dir = os.path.join(self.single_validation_video_save_dir, 'temp')
         self.video_save_path = os.path.join(self.single_validation_video_save_dir, self.feature_filename + '.mp4')
         if not os.path.exists(self.temp_dir): os.makedirs(self.temp_dir)
 
     def __run_clf(self):
         self.prob_col_name = f'Probability_{self.clf_name}'
-        self.in_df[self.prob_col_name] = self.clf.predict_proba(self.drop_bp_cords(df=self.in_df))[:, 1]
+        self.in_df[self.prob_col_name] = self.clf_predict_proba(clf=self.clf, x_df=self.in_df, model_name=self.clf_name, data_path=self.feature_file_path)
         self.in_df[self.clf_name] = np.where(self.in_df[self.prob_col_name] > self.discrimination_threshold, 1, 0)
 
-
     def __plug_bouts(self):
         self.data_df = plug_holes_shortest_bout(data_df=self.in_df, clf_name=self.clf_name, fps=self.fps, shortest_bout=self.shortest_bout)
 
     def __save(self):
         write_df(df=self.data_df, file_type=self.file_type, save_path=self.clf_data_save_path)
         print(f'Predictions created for video {self.feature_filename}...')
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.62.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.62.4/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.62.4/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.62.4/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.62.4/simba/model/train_rf.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,19 +136,20 @@
             else:
                 shuffle_splits, dataset_splits = Dtypes.NAN.value, Dtypes.NAN.value
             if generate_features_importance_bar_graph in Options.PERFORM_FLAGS.value:
                 feature_importance_bars = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.IMPORTANCE_BARS_N.value, Dtypes.INT.value, Dtypes.NAN.value)
                 check_int(name=ConfigKey.IMPORTANCE_BARS_N.value, value=feature_importance_bars, min_value=1)
             else:
                 feature_importance_bars = Dtypes.NAN.value
-            shap_target_present_cnt, shap_target_absent_cnt, shap_save_n = None, None, None
+            shap_target_present_cnt, shap_target_absent_cnt, shap_save_n, shap_multiprocess = None, None, None, None
             if generate_shap_scores in Options.PERFORM_FLAGS.value:
                 shap_target_present_cnt = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_PRESENT.value, data_type=Dtypes.INT.value, default_value=0)
                 shap_target_absent_cnt = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_ABSENT.value, data_type=Dtypes.INT.value, default_value=0)
                 shap_save_n = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_SAVE_ITERATION.value, data_type=Dtypes.STR.value, default_value=Dtypes.NONE.value)
+                shap_multiprocess = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.SHAP_MULTIPROCESS.value, data_type=Dtypes.STR.value, default_value='False')
                 try:
                     shap_save_n = int(shap_save_n)
                 except ValueError:
                     shap_save_n = shap_target_present_cnt + shap_target_absent_cnt
                 check_int(name=ConfigKey.SHAP_PRESENT.value, value=shap_target_present_cnt)
                 check_int(name=ConfigKey.SHAP_ABSENT.value, value=shap_target_absent_cnt)
 
@@ -185,24 +186,36 @@
             if generate_features_importance_log in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_log(self.rf_clf, self.feature_names, self.clf_name, self.eval_out_path)
             if generate_features_importance_bar_graph in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_bar_chart(self.rf_clf, self.feature_names, self.clf_name, self.eval_out_path, feature_importance_bars)
             if generate_example_decision_tree_fancy in Options.PERFORM_FLAGS.value:
                 self.dviz_classification_visualization(self.x_train, self.y_train, self.clf_name, self.class_names, self.eval_out_path)
             if generate_shap_scores in Options.PERFORM_FLAGS.value:
-                self.create_shap_log_mp(ini_file_path=self.config_path,
-                                        rf_clf=self.rf_clf,
-                                        x_df=self.x_train,
-                                        y_df=self.y_train,
-                                        x_names=self.feature_names,
-                                        clf_name=self.clf_name,
-                                        cnt_present=shap_target_present_cnt,
-                                        cnt_absent=shap_target_absent_cnt,
-                                        save_it=shap_save_n,
-                                        save_path=self.eval_out_path)
+                print(shap_multiprocess)
+                if not shap_multiprocess in Options.PERFORM_FLAGS.value:
+                    self.create_shap_log(ini_file_path=self.config_path,
+                                         rf_clf=self.rf_clf,
+                                         x_df=self.x_train,
+                                         y_df=self.y_train,
+                                         x_names=self.feature_names,
+                                         clf_name=self.clf_name,
+                                         cnt_present=shap_target_present_cnt,
+                                         cnt_absent=shap_target_absent_cnt,
+                                         save_it=shap_save_n,
+                                         save_path=self.eval_out_path)
+                else:
+                    self.create_shap_log_mp(ini_file_path=self.config_path,
+                                            rf_clf=self.rf_clf,
+                                            x_df=self.x_train,
+                                            y_df=self.y_train,
+                                            x_names=self.feature_names,
+                                            clf_name=self.clf_name,
+                                            cnt_present=shap_target_present_cnt,
+                                            cnt_absent=shap_target_absent_cnt,
+                                            save_path=self.eval_out_path)
 
             if compute_partial_dependency in Options.PERFORM_FLAGS.value:
                 self.partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.eval_out_path)
 
             if save_meta_data in Options.PERFORM_FLAGS.value:
                 meta_data_lst = [self.clf_name, criterion, max_features, min_sample_leaf,
                                  n_estimators, compute_permutation_importance, generate_classification_report,
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.62.4/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.62.4/simba/model/grid_search_rf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __author__ = "Simon Nilsson"
 
 import os
 from sklearn.model_selection import train_test_split
 from sklearn.ensemble import RandomForestClassifier
 
 from simba.utils.checks import check_int, check_str, check_float, check_if_filepath_list_is_empty, check_if_valid_input
-from simba.utils.read_write import read_config_entry, read_meta_file, read_simba_meta_files, get_fn_ext
+from simba.utils.read_write import read_config_entry, read_meta_file, read_simba_meta_files, get_fn_ext, str_2_bool
 from simba.ui.tkinter_functions import TwoOptionQuestionPopUp
 from simba.utils.printing import stdout_success
 from simba.utils.errors import InvalidInputError, NoDataError
 from simba.utils.enums import (Options,
                                ConfigKey,
                                Dtypes,
                                Methods,
@@ -111,17 +111,20 @@
             errors.append(check_if_valid_input(MetaKeys.IMPORTANCE_LOG.value, input=meta_dict[MetaKeys.IMPORTANCE_LOG.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
             errors.append(check_if_valid_input(MetaKeys.IMPORTANCE_BAR_CHART.value, input=meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
             errors.append(check_if_valid_input(MetaKeys.PERMUTATION_IMPORTANCE.value, input=meta_dict[MetaKeys.PERMUTATION_IMPORTANCE.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
             errors.append(check_if_valid_input(MetaKeys.LEARNING_CURVE.value, input=meta_dict[MetaKeys.LEARNING_CURVE.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
             errors.append(check_if_valid_input(MetaKeys.PRECISION_RECALL.value, input=meta_dict[MetaKeys.PRECISION_RECALL.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
             if MetaKeys.PARTIAL_DEPENDENCY.value in meta_dict.keys():
                 errors.append(check_if_valid_input(MetaKeys.PARTIAL_DEPENDENCY.value, input=meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value],options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
-
-            if meta_dict[MetaKeys.RF_MAX_FEATURES.value] == Dtypes.NONE.value: meta_dict[MetaKeys.RF_MAX_FEATURES.value] = None
-            if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value not in meta_dict.keys(): meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value] = Methods.SPLIT_TYPE_FRAMES.value
+            if ConfigKey.SHAP_MULTIPROCESS.value in meta_dict.keys():
+                errors.append(check_if_valid_input(ConfigKey.SHAP_MULTIPROCESS.value, input=meta_dict[ConfigKey.SHAP_MULTIPROCESS.value], options=Options.RUN_OPTIONS_FLAGS.value, raise_error=False)[1])
+            if meta_dict[MetaKeys.RF_MAX_FEATURES.value] == Dtypes.NONE.value:
+                meta_dict[MetaKeys.RF_MAX_FEATURES.value] = None
+            if MetaKeys.TRAIN_TEST_SPLIT_TYPE.value not in meta_dict.keys():
+                meta_dict[MetaKeys.TRAIN_TEST_SPLIT_TYPE.value] = Methods.SPLIT_TYPE_FRAMES.value
 
             if ConfigKey.CLASS_WEIGHTS.value in meta_dict.keys():
                 if meta_dict[ConfigKey.CLASS_WEIGHTS.value] not in Options.CLASS_WEIGHT_OPTIONS.value:
                     meta_dict[ConfigKey.CLASS_WEIGHTS.value] = None
                 if meta_dict[ConfigKey.CLASS_WEIGHTS.value] == 'custom':
                     meta_dict[ConfigKey.CLASS_WEIGHTS.value] = literal_eval(meta_dict['class_custom_weights'])
                     for k, v in meta_dict[ConfigKey.CLASS_WEIGHTS.value].items():
@@ -187,21 +190,48 @@
                 self.create_clf_report(self.rf_clf, self.x_test, self.y_test, self.class_names, self.model_dir_out, save_file_no=config_cnt)
             if meta_dict[MetaKeys.IMPORTANCE_LOG.value] in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_log(self.rf_clf, self.feature_names, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             if meta_dict[MetaKeys.IMPORTANCE_BAR_CHART.value] in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_bar_chart(self.rf_clf, self.feature_names, self.clf_name, self.model_dir_out, meta_dict[MetaKeys.N_FEATURE_IMPORTANCE_BARS.value], save_file_no=config_cnt)
             if MetaKeys.SHAP_SCORES.value in meta_dict.keys():
                 save_n = meta_dict[MetaKeys.SHAP_PRESENT.value] + meta_dict[MetaKeys.SHAP_ABSENT.value]
+                shap_multiprocess = False
                 if MetaKeys.SHAP_SAVE_ITERATION.value in meta_dict.keys():
                     try:
                         save_n = int(meta_dict[MetaKeys.SHAP_SAVE_ITERATION.value])
                     except ValueError:
                         save_n = meta_dict[MetaKeys.SHAP_PRESENT.value] + meta_dict[MetaKeys.SHAP_ABSENT.value]
+                if ConfigKey.SHAP_MULTIPROCESS.value in meta_dict.keys():
+                    shap_multiprocess = meta_dict[ConfigKey.SHAP_MULTIPROCESS.value]
+
                 if meta_dict[MetaKeys.SHAP_SCORES.value] in Options.PERFORM_FLAGS.value:
-                    self.create_shap_log_mp(self.config_path, self.rf_clf, self.x_train, self.y_train, self.feature_names, self.clf_name, meta_dict[MetaKeys.SHAP_PRESENT.value], meta_dict[MetaKeys.SHAP_ABSENT.value], self.model_dir_out, save_it=save_n, save_file_no=config_cnt)
+                    if not shap_multiprocess in Options.PERFORM_FLAGS.value:
+                        self.create_shap_log(ini_file_path=self.config_path,
+                                             rf_clf=self.rf_clf,
+                                             x_df=self.x_train,
+                                             y_df=self.y_train,
+                                             x_names=self.feature_names,
+                                             clf_name=self.clf_name,
+                                             cnt_present=meta_dict[MetaKeys.SHAP_PRESENT.value],
+                                             cnt_absent=meta_dict[MetaKeys.SHAP_ABSENT.value],
+                                             save_path=self.model_dir_out,
+                                             save_it=save_n,
+                                             save_file_no=config_cnt)
+                    else:
+                        self.create_shap_log_mp(ini_file_path=self.config_path,
+                                                rf_clf=self.rf_clf,
+                                                x_df=self.x_train,
+                                                y_df=self.y_train,
+                                                x_names=self.feature_names,
+                                                clf_name=self.clf_name,
+                                                cnt_present=meta_dict[MetaKeys.SHAP_PRESENT.value],
+                                                cnt_absent=meta_dict[MetaKeys.SHAP_ABSENT.value],
+                                                save_path=self.model_dir_out,
+                                                save_file_no=config_cnt)
+
             if MetaKeys.PARTIAL_DEPENDENCY.value in meta_dict.keys():
                 if meta_dict[MetaKeys.PARTIAL_DEPENDENCY.value] in Options.PERFORM_FLAGS.value:
                     self.partial_dependence_calculator(clf=self.rf_clf, x_df=self.x_train, clf_name=self.clf_name, save_dir=self.model_dir_out)
             self.create_meta_data_csv_training_multiple_models(meta_dict, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             self.save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out, save_file_no=config_cnt)
             print('Classifier {} saved in models/validations/model_files directory ...'.format(str(self.clf_name + '_' + str(config_cnt))))
         stdout_success(msg='All models and evaluations complete. The models/evaluation files are in models/validations folders')
```

### Comparing `Simba-UW-tf-dev-1.62.3/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.62.4/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.62.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.62.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.62.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.62.4/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.62.4/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.62.4/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.62.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.62.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.62.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.62.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.62.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.62.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.62.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.62.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.62.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.62.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.62.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.62.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.62.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.62.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.62.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.62.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.62.3
+Version: 1.62.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,16 @@
 simba/mixins/train_model_mixin.py
 simba/mixins/unsupervised_mixin.py
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
 simba/model/.DS_Store
 simba/model/grid_search_rf.py
 simba/model/inference_batch.py
 simba/model/inference_validation.py
 simba/model/train_rf.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
@@ -438,16 +440,18 @@
 tests/__init__.py
 tests/test_data_processors.py
 tests/test_distance_plotter.py
 tests/test_feature_extraction_mixin.py
 tests/test_featurizers.py
 tests/test_outlier_correctors.py
 tests/test_thirdparty_appenders.py
+tests/test_train_model_mixin.py
 tests/test_validation_clips.py
 tests/test_visualize_directing_animals.py
 tests/data/__init__.py
 tests/data/test_projects/__init__.py
 tests/data/test_projects/mouse_open_field/__init__.py
 tests/data/test_projects/two_c57/__init__.py
+tests/data/test_projects/two_c57/models/__init__.py
 tests/data/test_projects/zebrafish/__init__.py
 tests/data/test_projects/zebrafish/feature_file/__init__.py
 tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
```

### Comparing `Simba-UW-tf-dev-1.62.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.62.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/LICENSE.md` & `Simba-UW-tf-dev-1.62.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.62.4/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.62.4/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.62.4/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.62.4/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.62.4/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.62.4/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.62.4/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.62.4/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/README.md` & `Simba-UW-tf-dev-1.62.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.3/setup.py` & `Simba-UW-tf-dev-1.62.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.62.3",
+    version="1.62.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

