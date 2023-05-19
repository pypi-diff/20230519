# Comparing `tmp/Simba-UW-tf-dev-1.59.8.tar.gz` & `tmp/Simba-UW-tf-dev-1.59.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.8.tar", last modified: Thu May 18 22:19:34 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.9.tar", last modified: Fri May 19 18:36:44 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.59.8.tar` & `Simba-UW-tf-dev-1.59.9.tar`

### file list

```diff
@@ -1,502 +1,503 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.59.8/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.59.8/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.8/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.8/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.8/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-05-13 17:39:29.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-18 22:17:21.000000 Simba-UW-tf-dev-1.59.8/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3696 2023-05-18 20:58:44.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.8/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29958 2023-05-13 17:59:00.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36917 2023-05-18 13:15:22.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61153 2023-05-18 13:21:56.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.59.8/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.8/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.8/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.8/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.59.8/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    40646 2023-05-16 12:53:49.000000 Simba-UW-tf-dev-1.59.8/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.59.8/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.59.8/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.8/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.59.8/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.8/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15636 2023-05-16 20:41:20.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6695 2023-05-14 19:17:05.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    14943 2023-05-18 22:19:18.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19307 2023-05-14 15:34:06.000000 Simba-UW-tf-dev-1.59.8/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3547 2023-05-16 18:49:04.000000 Simba-UW-tf-dev-1.59.8/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18794 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.8/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3294 2023-05-17 20:36:23.000000 Simba-UW-tf-dev-1.59.8/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7464 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-17 14:05:21.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.59.8/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19390 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.8/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.8/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.8/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-18 22:19:26.000000 Simba-UW-tf-dev-1.59.8/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.59.9/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15019 2023-05-19 18:30:31.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.59.9/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.9/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.9/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.9/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-18 22:17:21.000000 Simba-UW-tf-dev-1.59.9/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3696 2023-05-18 20:58:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.9/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51865 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61153 2023-05-18 13:21:56.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.59.9/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.9/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.9/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.9/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.59.9/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    41533 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.59.9/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.59.9/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.59.9/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.9/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.59.9/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.9/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15608 2023-05-19 15:09:35.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.59.9/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.59.9/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.59.9/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.59.9/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.59.9/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19547 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.9/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.9/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.9/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-19 18:36:30.000000 Simba-UW-tf-dev-1.59.9/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.59.8/PKG-INFO` & `Simba-UW-tf-dev-1.59.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.8
+Version: 1.59.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.line_width = Entry_Box(self.style_settings_frm, 'Line width: ', '16', validation='numeric')
         self.max_lines_entry = Entry_Box(self.style_settings_frm, 'Max prior lines (ms): ', '16', validation='numeric')
         self.font_size = Entry_Box(self.style_settings_frm, 'Font size: ', '16', validation='numeric')
         self.font_thickness = Entry_Box(self.style_settings_frm, 'Font thickness: ', '16', validation='numeric')
         self.circle_size = Entry_Box(self.style_settings_frm, 'Circle size: ', '16', validation='numeric')
         self.resolution_dropdown.setChoices(self.resolutions[0])
         self.line_width.entry_set(val=6)
-        self.bg_clr_dropdown.setChoices(list(self.colors_dict.keys())[0])
+        self.bg_clr_dropdown.setChoices('White')
         self.circle_size.entry_set(val=20)
         self.font_size.entry_set(val=3)
         self.font_thickness.entry_set(val=2)
         self.max_lines_entry.entry_set(2000)
         self.resolution_dropdown.disable()
         self.line_width.set_state("disable")
         self.bg_clr_dropdown.disable()
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.59.9/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.59.9/simba/labelling/extract_labelled_frames.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     """
     Extracts all human annotated frames where behavior is annotated as present into .pngs within a SimBA project
 
     :param list clfs: Names of classifiers to extract behavior-present images from.
     :param dict settings: User-defined settings. E.g., how much to downsample the png images.
     :param str config_path: path to SimBA configparser.ConfigParser project_config.in
 
+    .. note::
+        Use settings={'downsample': 2} to downsample all .pngs to 0.5 original size for disk space savings.
+
     :example:
     >>> extractor = AnnotationFrameExtractor(config_path='project_folder/project_config.ini', clfs=['Sniffing', 'Attack'], settings={'downsample': 2})
     >>> extractor.run()
     """
 
 
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.59.9/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/requirements.txt` & `Simba-UW-tf-dev-1.59.9/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/config_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,26 +508,18 @@
         if info_df['fps'].min() <= 1:
             InvalidValueWarning(msg='Videos in your SimBA project have an FPS of 1 or less. Please use videos with more than one frame per second, or correct the inaccurate fps inside the `project_folder/logs/videos_info.csv` file')
         return info_df
 
     def read_video_info(self,
                         video_name: str) -> (pd.DataFrame, float, float):
         """
-        Helper to read the meta-data (pixels per mm, resolution, fps) from the video_info.csv for a single input file
+        Helper to read the meta-data (pixels per mm, resolution, fps) from the video_info.csv for a single input file.
 
-        Parameters
-        ----------
-        video_name: str
-            The name of the video without extension to get the meta data for.
-
-        Returns
-        -------
-        video_settings: pd.DataFrame
-        px_per_mm: float
-        fps: float
+        :param str video_name: The name of the video without extension to get the meta data for
+        :return (pd.DataFrame, float, float)
         """
 
         video_settings = self.video_info_df.loc[self.video_info_df['Video'] == video_name]
         if len(video_settings) > 1:
             raise DuplicationError(msg=f'SimBA found multiple rows in the project_folder/logs/video_info.csv named {str(video_name)}. Please make sure that each video name is represented ONCE in the video_info.csv')
         elif len(video_settings) < 1:
             raise ParametersFileError(msg=f'SimBA could not find {str(video_name)} in the video_info.csv file. Make sure all videos analyzed are represented in the project_folder/logs/video_info.csv file.')
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi` & `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/feature_extraction_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from simba.utils.enums import Paths, Options
 from simba.utils.checks import check_if_filepath_list_is_empty, check_file_exist_and_readable, check_minimum_roll_windows
 from simba.utils.read_write import (read_project_path_and_file_type,
                                     read_video_info_csv,
                                     read_config_file,
                                     get_bp_headers)
-from simba.utils.errors import CountError
+from simba.utils.errors import CountError, InvalidInputError
 import simba
 
 class FeatureExtractionMixin(object):
     """
     Methods for featurizing pose-estimation data.
 
     :param Optional[configparser.Configparser] config_path: path to SimBA project_config.ini
@@ -580,19 +580,20 @@
 
         :example:
         >>> loc_1 = np.random.randint(1, 200, size=(6, 2)).astype(np.float32)
         >>> loc_2 = np.random.randint(1, 200, size=(6, 2)).astype(np.float32)
         >>> FeatureExtractionMixin.framewise_euclidean_distance_roi(location_1=loc_1, location_2=loc_2, px_per_mm=4.56, centimeter=False)
         >>> [49.80098657, 46.54963644, 49.60650394, 70.35919993, 37.91069901, 71.95422524]
         """
-
+        # if not px_per_mm and centimeter:
+        #     raise InvalidInputError(msg='To calculate centimeters, provide a pixel per millimeter value')
         results = np.full((location_1.shape[0]), np.nan)
         for i in prange(location_1.shape[0]):
             results[i] = np.linalg.norm(location_1[i] - location_2[i]) / px_per_mm
-        if centimeter:
+        if centimeter and px_per_mm:
             results = results / 10
         return results
 
     def dataframe_gaussian_smoother(self,
                                     df: pd.DataFrame,
                                     fps: int,
                                     time_window: int=100) -> pd.DataFrame:
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.59.9/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/enums.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/checks.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/read_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,30 @@
 def read_config_entry(config: configparser.ConfigParser,
                       section: str,
                       option: str,
                       data_type: str,
                       default_value: Optional[Any] = None,
                       options: Optional[List] = None) -> Union[float, int, str]:
 
+    """
+    Helper to read entry in SimBA project_config.ini parsed by configparser.ConfigParser.
+
+    :param configparser.ConfigParser config: Parsed SimBA project_config.ini. Use :meth:`simba.utils.read_config_file` to parse file.
+    :param str section: Section name of entry to parse.
+    :param str option: Option name of entry to parse.
+    :param str data_type: Type of data to parse. E.g., `str`, `int`, `float`.
+    :param Optional[Any] default_value: If no matching entry can be found in the project_config.ini, use this as default.
+    :param Optional[List] or None options: List of valid options. If not None, checks that the returned entry value exists in this list.
+    :return Any
+
+    :example:
+    >>> read_config_entry(config='project_folder/project_config.ini', section='General settings', option='project_name', data_type='str')
+    >>> 'two_animals_14_bps'
+    """
+
 
     try:
         if config.has_option(section, option):
             if data_type == Dtypes.FLOAT.value:
                 value = config.getfloat(section, option)
             elif data_type == Dtypes.INT.value:
                 value = config.getint(section, option)
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/errors.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/data.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/utils/printing.py` & `Simba-UW-tf-dev-1.59.9/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,15 @@
     def run(self):
         """
         Method to create path plot videos and/or frames.Results are store in the
         'project_folder/frames/path_plots' directory of the SimBA project.
         """
 
         for file_cnt, file_path in enumerate(self.files_found):
-            video_timer = SimbaTimer()
-            video_timer.start_timer()
+            video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_info, _, self.fps = self.read_video_info(video_name=self.video_name)
             self.__get_styles()
             self.data_df = read_df(file_path, self.file_type)
             self.temp_folder = os.path.join(self.path_plot_dir, self.video_name, 'temp')
             self.save_frame_folder_dir = os.path.join(self.path_plot_dir, self.video_name)
             if self.frame_setting:
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.59.9/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.59.9/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.59.9/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/agg_clf_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,24 +43,14 @@
         self.chosen_measures, self.classifiers = data_measures, classifiers
         self.file_save_name = os.path.join(self.project_path, 'logs', 'data_summary_' + str(self.datetime) + '.csv')
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg='SIMBA ERROR: No data files found in the project_folder/csv/machine_results directory. Run classifiers before analysing results.')
         print(f'Analyzing {str(len(self.machine_results_paths))} file(s) for {str(len(self.clf_names))} classifiers...')
 
     def run(self):
-
-        """
-        Method to create dataframe of classifier aggregate statistics
-
-        Returns
-        -------
-        Attribute: pd.Dataframe
-            results_df
-        """
-
         self.results_df = pd.DataFrame()
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, file_name, _ = get_fn_ext(file_path)
             print('Analyzing video {}...'.format(file_name))
             _, _, fps = self.read_video_info(video_name=file_name)
             check_file_exist_and_readable(file_path)
             data_df = read_df(file_path, self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolation_smoothing.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,20 +72,22 @@
         for file_path in self.files_found:
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
             df[df < 0] = 0
             if self.initial_import_multi_index:
-                df.columns = self.bp_col_names
+                df.columns = self.bp_headers
             for animal_name, animal_bps in self.animal_bp_dict.items():
                 animal_df = df[animal_bps['X_bps'] + animal_bps['Y_bps']].fillna(0).astype(int)
                 idx = list(animal_df[animal_df.eq(animal_df.iloc[:, 0], axis=0).all(axis='columns')].index)
+                print(f'Interpolating {len(idx)} body-parts for animal {animal_name} in video {video_name}...')
                 animal_df.loc[idx, :] = np.nan
                 animal_df = animal_df.interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
+                animal_df[animal_df < 0] = 0
                 df.update(animal_df)
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
                 df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
@@ -95,22 +97,27 @@
 
     def body_part_interpolator(self):
         for file_path in self.files_found:
             video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=True)
             if self.initial_import_multi_index:
-                df.columns = self.bp_col_names
+                df.columns = self.bp_headers
             df[df < 0] = 0
             for animal in self.animal_bp_dict:
                 for x_bps_name, y_bps_name in zip(self.animal_bp_dict[animal]['X_bps'], self.animal_bp_dict[animal]['Y_bps']):
-                    idx = (df[(df[x_bps_name] <= 0) & (df[y_bps_name] <= 0)].index.tolist())
+                    df[x_bps_name] = df[x_bps_name].astype(int)
+                    df[y_bps_name] = df[y_bps_name].astype(int)
+                    idx = df.loc[(df[x_bps_name] <= 0.0) & (df[y_bps_name] <= 0.0)].index.tolist()
+                    print(f'Interpolating {len(idx)} {x_bps_name[:-2]} body-parts for animal {animal} in video {video_name}...')
                     df.loc[idx, [x_bps_name, y_bps_name]] = np.nan
                     df[x_bps_name] = df[x_bps_name].interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
+                    df[x_bps_name][df[x_bps_name] < 0] = 0
                     df[y_bps_name] = df[y_bps_name].interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
+                    df[y_bps_name][df[y_bps_name] < 0] = 0
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
                 df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
             write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
@@ -149,39 +156,47 @@
             check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg=f"SIMBA ERROR: {self.input_dir} does not contain any {self.file_type} files.")
         else:
             self.files_found = [input_path]
             self.input_dir = os.path.dirname(input_path)
         if not initial_import_multi_index:
             self.save_dir = os.path.join(self.input_dir, f'Pre_{smoothing_method}_interpolation_{self.datetime}')
             if not os.path.exists(self.save_dir): os.makedirs(self.save_dir)
-        self.time_window, self.initial_import_multi_index = time_window, initial_import_multi_index
+        self.time_window, self.initial_import_multi_index = int(time_window), initial_import_multi_index
         if smoothing_method == Methods.SAVITZKY_GOLAY.value:
             self.savgol_smoother()
         elif smoothing_method == Methods.GAUSSIAN.value:
             self.gaussian_smoother()
         self.timer.stop_timer()
         stdout_success(msg=f'{str(len(self.files_found))} data file(s) smoothened', elapsed_time=self.timer.elapsed_time_str)
 
     def savgol_smoother(self):
         for file_path in self.files_found:
             video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
             video_path = find_video_of_file(video_dir=self.video_dir, filename=video_name)
             if not video_path:
-                raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing smoothing. To perform smoothing, SimBA needs the video in order to read the video FPS.')
-            video_meta_data = get_video_meta_data(video_path=video_path)
-            frames_in_time_window = int(self.time_window / (1000 / video_meta_data['fps']))
+                try:
+                    video_meta_data = {}
+                    self.video_info_df = self.read_video_info_csv(file_path=self.video_info_path)
+                    _, _, fps = self.read_video_info(video_name=video_name)
+                    video_meta_data['fps'] = fps
+                except:
+                    raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing smoothing. To perform smoothing, SimBA needs the video fps from the video itself or the logs/video_info.csv file in order to read the video FPS.')
+            else:
+                video_meta_data = get_video_meta_data(video_path=video_path)
+            frames_in_time_window = int(self.time_window / (1000 / int(video_meta_data['fps'])))
             if (frames_in_time_window % 2) == 0:
                 frames_in_time_window = frames_in_time_window - 1
             if (frames_in_time_window % 2) <= 3:
                 frames_in_time_window = 5
             df[df < 0] = 0
             for c in df.columns:
                 df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
+                df[c][df[c] < 0] = 0
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
                 df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
             write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
@@ -194,17 +209,17 @@
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
             video_path = find_video_of_file(video_dir=self.video_dir, filename=video_name)
             if not video_path:
                 raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing Gaussian smoothing. To perform smoothing, SimBA needs the video in order to read the video FPS.')
             video_meta_data = get_video_meta_data(video_path=video_path)
             frames_in_time_window = int(self.time_window / (1000 / video_meta_data['fps']))
-            df[df < 0] = 0
             for c in df.columns:
                 df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
+                df[c][df[c] < 0] = 0
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
                 df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
             write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
@@ -213,21 +228,21 @@
 
 
 # Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/outlier_corrected_movement_location',
 #             config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #             method='Body-parts: Nearest',
 #             initial_import_multi_index=False)
 
-# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/csv/outlier_corrected_movement_location',
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/csv/input_csv',
 #             config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini',
-#             method='Body-parts: Nearest',
-#             initial_import_multi_index=False)
-# #
+#             method='Body-parts: Linear',
+#             initial_import_multi_index=True)
 #
 
+
 # Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/csv/outlier_corrected_movement_location',
 #             config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
 #             method='Body-parts: Nearest',
 #             initial_import_multi_index=False)
 
 # PostHocInterpolate(config_path='/Users/simon/Desktop/envs/troubleshooting/ddddfff/project_folder/project_config.ini',
 #                    input_dir='/Users/simon/Desktop/envs/troubleshooting/ddddfff/project_folder/csv/outlier_corrected_movement_location',
@@ -236,15 +251,19 @@
 
 # Smooth(config_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/project_config.ini',
 #               input_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/csv/input_csv',
 #               time_window=100,
 #               smoothing_method=Methods.SAVITZKY_GOLAY.value,
 #               initial_import_multi_index=True)
 
-
+# Smooth(config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini',
+#               input_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/csv/input_csv',
+#               time_window=400,
+#               smoothing_method=Methods.SAVITZKY_GOLAY.value,
+#               initial_import_multi_index=True)
 
 
 # class PostHocSmooth(ConfigReader):
 #     def __init__(self,
 #                  config_path: str,
 #                  input_dir: str,
 #                  time_window: int,
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.59.9/simba/model/train_rf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 from simba.utils.enums import (Options,
                                ConfigKey,
                                Dtypes,
                                Methods)
 
 class TrainRandomForestClassifier(ConfigReader, TrainModelMixin):
     """
-    Train a single random forest model from hyper-parameter setting and sampling methods
-    stored within the SimBA project config .ini file (`global environment`).
+    Train a single random forest model using hyperparameter setting and methods
+    stored within the SimBA project config .ini file (``global environment``).
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :param str config_path: path to SimBA project config file in Configparser format
 
-    Example
-    ----------
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#step-7-train-machine-model>`_
+
+    :example:
     >>> model_trainer = TrainRandomForestClassifier(config_path='MyConfigPath')
     >>> model_trainer.perform_sampling()
     >>> model_trainer.train_model()
     >>> model_trainer.save_model()
-
     """
 
 
     def __init__(self,
                  config_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path)
@@ -77,25 +75,14 @@
         print('Training and evaluating model...')
         self.timer = SimbaTimer(start=True)
 
     def perform_sampling(self):
         """
         Method for sampling data for training and testing, and perform over and under-sampling of the training sets
         as indicated within the SimBA project config.
-
-        Returns
-        ----------
-        Attribute: array
-            x_train
-        Attribute: array
-            y_train
-        Attribute: array
-            x_test
-        Attribute: array
-            y_test
         """
 
         if self.split_type == Methods.SPLIT_TYPE_FRAMES.value:
             self.x_train, self.x_test, self.y_train, self.y_test = train_test_split(self.x_df, self.y_df,test_size=self.tt_size)
         elif self.split_type == Methods.SPLIT_TYPE_BOUTS.value:
             self.x_train, self.x_test, self.y_train, self.y_test = self.bout_train_test_splitter(x_df=self.x_df,y_df=self.y_df, test_size=self.tt_size)
 
@@ -105,19 +92,14 @@
             self.x_train, self.y_train = self.smoteen_oversampler(self.x_train, self.y_train, float(self.over_sample_ratio))
         elif self.over_sample_setting == Methods.SMOTE.value.lower():
             self.x_train, self.y_train = self.smote_oversampler(self.x_train, self.y_train, float(self.over_sample_ratio))
 
     def train_model(self):
         """
         Method for training single random forest model.
-
-        Returns
-        ----------
-        Attribute: object
-            rf_clf
         """
 
         if self.algo == 'RF':
             n_estimators = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.RF_ESTIMATORS.value, data_type=Dtypes.INT.value)
             max_features = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, ConfigKey.RF_MAX_FEATURES.value, data_type=Dtypes.STR.value)
             if max_features == 'None':
                 max_features = None
@@ -228,22 +210,18 @@
                                  generate_features_importance_log, generate_precision_recall_curve, save_meta_data,
                                  generate_learning_curve, dataset_splits, shuffle_splits, feature_importance_bars,
                                  self.over_sample_ratio, self.over_sample_setting, self.tt_size, self.split_type,
                                  self.under_sample_ratio, self.under_sample_setting, str(class_weights)]
 
                 self.create_meta_data_csv_training_one_model(meta_data_lst, self.clf_name, self.eval_out_path)
 
-    def save_model(self):
+    def save_model(self) -> None:
         """
         Method for saving pickled RF model. The model is saved in the `models/generated_models` directory
         of the SimBA project tree.
-
-        Returns
-        ----------
-        None
         """
 
         self.timer.stop_timer()
         self.save_rf_model(self.rf_clf, self.clf_name, self.model_dir_out)
         stdout_success(msg=f'Classifier {self.clf_name} saved in models/generated_models directory', elapsed_time=self.timer.elapsed_time_str)
         stdout_success(msg=f'Evaluation files are in models/generated_models/model_evaluations folders')
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.59.9/simba/model/inference_batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,14 @@
     Example
     ----------
     >>> _ = InferenceBatch(config_path='MyConfigPath').run()
     """
 
     def __init__(self,
                  config_path: str):
-        """
-        Method to run classifier inference. Results are stored in the ``project_folder/csv/machine_results`` directory
-        of the SimBA project.
-
-        Returns
-        ----------
-        None
-        """
-
         ConfigReader.__init__(self, config_path=config_path)
         TrainModelMixin.__init__(self)
         if len(self.feature_file_paths) == 0:
             raise NoFilesFoundError('Zero files found in the project_folder/csv/features_extracted directory. Create features before running classifier.')
         print(f'Analyzing {len(self.feature_file_paths)} file(s) with {self.clf_cnt} classifier(s)')
         self.timer = SimbaTimer(start=True)
         self.model_dict = self.get_model_info(config=self.config, model_cnt=self.clf_cnt)
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.59.9/simba/model/grid_search_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,20 +22,17 @@
 class GridSearchRandomForestClassifier(ConfigReader, TrainModelMixin):
     """
     Grid-searching random forest models from hyperparameter setting and sampling methods
     stored within the `project_folder/configs` directory of a SimBA project.
 
     .. note::
        Searches you SimBA project `project_folder/configs` directory for files and builds
-       one model per file.
+       one model per config file. `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#step-7-train-machine-model>`__.
 
-    Parameters
-    ----------
-    config_path: str
-        path to SimBA project config file in Configparser format
+    :param str config_path: path to SimBA project config file in Configparser format
 
     Example
     ----------
     >>> _ = GridSearchRandomForestClassifier(config_path='MyConfigPath').run()
     """
 
     def __init__(self,
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.59.9/simba/model/inference_validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,29 +15,22 @@
 from simba.mixins.train_model_mixin import TrainModelMixin
 
 class InferenceValidation(ConfigReader, TrainModelMixin):
     """
     Run a single classifier on a single featurized input file. Results are saved within the
     ``project_folder/csv/validation`` directory of the SimBA project.
 
-    Parameters
-    ----------
-    config_file_path: str
-        path to SimBA project config file in Configparser format
-    input_file_path: str
-        path to file containing features
-    clf_path: str
-        path to pickled rf sklearn classifier.
+    :param str config_file_path: path to SimBA project config file in Configparser format
+    :param str input_file_path: path to file containing features
+    :param str clf_path: path to pickled rf sklearn classifier.
 
-    Notes
-    -----
-
-    Examples
-    -----
+    .. note::
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-3-run-the-classifier-on-new-data>`_
 
+    :example:
     >>> InferenceValidation(config_path=r"MyProjectConfigPath", input_file_path=r"FeatureFilePath", clf_path=r"ClassifierPath")
 
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  input_file_path: Union[str, os.PathLike],
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.59.9/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     :parameter str config_path: path to SimBA project config file in Configparser format
 
     Examples
     ----------
     >>> _ = OutlierCorrecterLocation(config_path='MyProjectConfig').run()
     """
+
     def __init__(self,
                  config_path: str):
 
         super().__init__(config_path=config_path)
         if not os.path.exists(self.outlier_corrected_dir): os.makedirs(self.outlier_corrected_dir)
         if self.animal_cnt == 1:
             self.animal_id = read_config_entry(self.config, ConfigKey.MULTI_ANIMAL_ID_SETTING.value, ConfigKey.MULTI_ANIMAL_IDS.value, Dtypes.STR.value)
@@ -120,13 +121,13 @@
                     out_df_lst.append(pd.DataFrame([[video_name, animal_name, bp_name, len(vid_idx_lst), correction_ratio]], columns=['Video', 'Animal', 'Body-part', 'Corrections', 'Correction ratio (%)']))
         out_df = pd.concat(out_df_lst, axis=0).reset_index(drop=True)
         log_fn = os.path.join(self.logs_path, 'Outliers_location_{}.csv'.format(self.datetime))
         out_df.to_csv(log_fn)
         self.timer.stop_timer()
         stdout_success(msg='Log for corrected "location outliers" saved in project_folder/logs', elapsed_time=self.timer.elapsed_time_str)
 
-#
+
 # test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
 # test.run()
 
 # test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 # test.correct_location_outliers()
```

### Comparing `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/SimBA.py` & `Simba-UW-tf-dev-1.59.9/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.59.9/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.9/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.59.9/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.59.9/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.59.9/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.8
+Version: 1.59.9
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 simba/assets/icons/concat_icons/vertical.png
 simba/assets/img/.DS_Store
 simba/assets/img/about_me.png
 simba/assets/img/bg.png
 simba/assets/img/bg_2.png
 simba/assets/img/splash.mp4
 simba/assets/img/splash.pptx
-simba/assets/img/~$splash.pptx
 simba/assets/lookups/.DS_Store
 simba/assets/lookups/feature_extraction_headers.csv
 simba/assets/lookups/features.csv
 simba/assets/lookups/model_names.parquet
 simba/assets/lookups/unsupervised_example_x.csv
 simba/assets/shap/.DS_Store
 simba/assets/shap/UbuntuMono-Regular.ttf
@@ -218,14 +217,16 @@
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
 simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
 simba/model/grid_search_rf.py
 simba/model/inference_batch.py
 simba/model/inference_validation.py
 simba/model/train_rf.py
 simba/outlier_tools/.DS_Store
 simba/outlier_tools/__init__.py
 simba/outlier_tools/outlier_corrector_location.py
```

### Comparing `Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/LICENSE.md` & `Simba-UW-tf-dev-1.59.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/README.md` & `Simba-UW-tf-dev-1.59.9/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.8/setup.py` & `Simba-UW-tf-dev-1.59.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.59.8",
+    version="1.59.9",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

