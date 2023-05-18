# Comparing `tmp/Simba-UW-tf-dev-1.59.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.59.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.7.tar", last modified: Wed May 17 20:38:39 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.8.tar", last modified: Thu May 18 22:19:34 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.59.7.tar` & `Simba-UW-tf-dev-1.59.8.tar`

### file list

```diff
@@ -1,501 +1,502 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.59.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2310 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.59.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-05-13 17:39:29.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.59.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.7/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-17 17:10:25.000000 Simba-UW-tf-dev-1.59.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-05-14 19:55:18.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29958 2023-05-13 17:59:00.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36916 2023-05-16 17:59:20.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61146 2023-05-16 16:43:07.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    58953 2023-05-17 20:38:27.000000 Simba-UW-tf-dev-1.59.7/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.59.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.59.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    40646 2023-05-16 12:53:49.000000 Simba-UW-tf-dev-1.59.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.59.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.59.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.59.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.7/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15636 2023-05-16 20:41:20.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8493 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8052 2023-05-17 19:13:02.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/severity_calculator_2.py
--rw-r--r--   0 simon      (501) staff       (20)     6695 2023-05-14 19:17:05.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    14002 2023-05-14 19:35:26.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12807 2023-05-14 19:22:08.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9645 2023-05-14 19:37:14.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7732 2023-05-14 19:37:49.000000 Simba-UW-tf-dev-1.59.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19307 2023-05-14 15:34:06.000000 Simba-UW-tf-dev-1.59.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3547 2023-05-16 18:49:04.000000 Simba-UW-tf-dev-1.59.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18794 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3294 2023-05-17 20:36:23.000000 Simba-UW-tf-dev-1.59.7/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7464 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-17 14:05:21.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.59.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19324 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-17 20:38:38.000000 Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.7/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-17 20:38:33.000000 Simba-UW-tf-dev-1.59.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-17 20:38:39.000000 Simba-UW-tf-dev-1.59.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.59.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15044 2023-05-03 21:12:42.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.59.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.8/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-05-13 17:39:29.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.59.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-18 22:17:21.000000 Simba-UW-tf-dev-1.59.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3696 2023-05-18 20:58:44.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29958 2023-05-13 17:59:00.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36917 2023-05-18 13:15:22.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61153 2023-05-18 13:21:56.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.59.8/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.59.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.59.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    40646 2023-05-16 12:53:49.000000 Simba-UW-tf-dev-1.59.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.59.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.59.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.59.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.8/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15636 2023-05-16 20:41:20.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6695 2023-05-14 19:17:05.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    14943 2023-05-18 22:19:18.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.59.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19307 2023-05-14 15:34:06.000000 Simba-UW-tf-dev-1.59.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3547 2023-05-16 18:49:04.000000 Simba-UW-tf-dev-1.59.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18794 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3294 2023-05-17 20:36:23.000000 Simba-UW-tf-dev-1.59.8/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-17 14:05:21.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.59.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-05-09 20:23:39.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19390 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-18 22:19:33.000000 Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.8/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.8/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.8/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-18 22:19:26.000000 Simba-UW-tf-dev-1.59.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-18 22:19:34.000000 Simba-UW-tf-dev-1.59.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.59.7/PKG-INFO` & `Simba-UW-tf-dev-1.59.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.7
+Version: 1.59.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,10 +36,11 @@
         self.chosen_bp_val = StringVar(value=self.all_body_parts[0])
         self.choose_bp_dropdown = OptionMenu(self.settings_frm, self.chosen_bp_val, *self.all_body_parts)
         self.body_part_lbl.grid(row=1, column=0, sticky=NW)
         self.choose_bp_dropdown.grid(row=1, column=1, sticky=NW)
 
         run_btn = Button(self.settings_frm,text='Create path plot',command=lambda: draw_line_plot(self.config_path, self.chosen_video_val.get(), self.chosen_bp_val.get()))
         run_btn.grid(row=2, column=1, pady=10)
+        self.main_frm.mainloop()
 
 
 #_ = QuickLineplotPopup(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.59.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.59.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.59.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.59.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.59.8/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.59.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -60,54 +60,54 @@
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0003 0000 0001 0000 000b  ................
 00000410: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00000420: 6c73 7670 626c 6f62 0000 025e 6270 6c69  lsvpblob...^bpli
+00000420: 6c73 7670 626c 6f62 0000 0266 6270 6c69  lsvpblob...fbpli
 00000430: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00000440: 1a46 470a 4458 6963 6f6e 5369 7a65 5f10  .FG.DXiconSize_.
-00000450: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00000460: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00000470: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00000480: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00000490: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-000004a0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-000004b0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-000004c0: 0009 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
-000004d0: 2d32 373c 4158 636f 6d6d 656e 7473 5e64  -27<AXcomments^d
-000004e0: 6174 654c 6173 744f 7065 6e65 645b 6461  ateLastOpened[da
-000004f0: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-00000500: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-00000510: 6e54 6e61 6d65 5c64 6174 654d 6f64 6966  nTname\dateModif
-00000520: 6965 64d4 1617 1819 1a1b 0a1d 5776 6973  ied.........Wvis
-00000530: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-00000540: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-00000550: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
-00000560: d416 1718 191a 251a 2708 10b5 0810 02d4  ......%.'.......
-00000570: 1617 1819 0a2a 1a2c 0910 6108 1003 d416  .....*.,..a.....
-00000580: 1718 191a 2f0a 3108 1064 0910 05d4 1617  ..../.1..d......
-00000590: 1819 0a34 0a36 0910 7309 1004 d416 1718  ...4.6..s.......
-000005a0: 191a 390a 3b08 104b 0910 06d4 1617 1819  ..9.;..K........
-000005b0: 0a3e 0a40 0911 01c7 0910 00d4 1617 1819  .>.@............
-000005c0: 0a25 1a44 0908 1001 0823 4028 0000 0000  .%.D.....#@(....
-000005d0: 0000 546e 616d 6509 0008 0019 0022 0034  ..Tname......".4
-000005e0: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
-000005f0: 00a9 00b2 00c1 00cd 00d2 00d8 00dd 00e5  ................
-00000600: 00ea 00f7 0100 0108 010e 0118 011e 011f  ................
-00000610: 0122 0123 0125 012e 012f 0131 0132 0134  .".#.%.../.1.2.4
-00000620: 013d 013e 0140 0141 0143 014c 014d 014f  .=.>.@.A.C.L.M.O
-00000630: 0150 0152 015b 015c 015e 015f 0161 016a  .P.R.[.\.^._.a.j
-00000640: 016b 016d 016e 0170 0179 017a 017c 017d  .k.m.n.p.y.z.|.}
-00000650: 017f 0188 0189 018c 018d 018f 0198 0199  ................
-00000660: 019a 019c 019d 01a6 01ab 0000 0000 0000  ................
-00000670: 0201 0000 0000 0000 0049 0000 0000 0000  .........I......
-00000680: 0000 0000 0000 0000 01ac 6408 08d4 0d0e  ..........d.....
-00000690: 0f10 2425 180a 5473 697a 6510 6108 09d4  ..$%..Tsize.a...
+00000440: 1a45 4647 0a5f 1012 7669 6577 4f70 7469  .EFG._..viewOpti
+00000450: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+00000460: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00000470: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00000480: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
+00000490: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
+000004a0: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
+000004b0: 6976 6544 6174 6573 1001 09d9 0c0d 0e0f  iveDates........
+000004c0: 1011 1213 1415 1e23 272b 3035 3a3f 5863  .......#'+05:?Xc
+000004d0: 6f6d 6d65 6e74 735e 6461 7465 4c61 7374  omments^dateLast
+000004e0: 4f70 656e 6564 5c64 6174 654d 6f64 6966  Opened\dateModif
+000004f0: 6965 645b 6461 7465 4372 6561 7465 6454  ied[dateCreatedT
+00000500: 7369 7a65 556c 6162 656c 546b 696e 6457  sizeUlabelTkindW
+00000510: 7665 7273 696f 6e54 6e61 6d65 d416 1718  versionTname....
+00000520: 191a 1b0a 1d57 7669 7369 626c 6555 7769  .....WvisibleUwi
+00000530: 6474 6859 6173 6365 6e64 696e 6755 696e  dthYascendingUin
+00000540: 6465 7808 1101 2c09 1007 d416 1718 191a  dex...,.........
+00000550: 201a 2208 10c8 0810 08d4 1617 1819 0a25   ."............%
+00000560: 1a09 0910 b508 d416 1718 191a 251a 2a08  ............%.*.
+00000570: 0810 02d4 1617 1819 0a2d 1a2f 0910 6108  .........-./..a.
+00000580: 1003 d416 1718 191a 320a 3408 1064 0910  ........2.4..d..
+00000590: 05d4 1617 1819 0a37 0a39 0910 7309 1004  .......7.9..s...
+000005a0: d416 1718 191a 3c0a 3e08 104b 0910 06d4  ......<.>..K....
+000005b0: 1617 1819 0a41 0a43 0911 01c7 0910 0008  .....A.C........
+000005c0: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
+000005d0: 6469 6669 6564 2340 3000 0000 0000 0009  dified#@0.......
+000005e0: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+000005f0: 0079 008c 008e 008f 00a2 00ab 00ba 00c7  .y..............
+00000600: 00d3 00d8 00de 00e3 00eb 00f0 00f9 0101  ................
+00000610: 0107 0111 0117 0118 011b 011c 011e 0127  ...............'
+00000620: 0128 012a 012b 012d 0136 0137 0139 013a  .(.*.+.-.6.7.9.:
+00000630: 0143 0144 0145 0147 0150 0151 0153 0154  .C.D.E.G.P.Q.S.T
+00000640: 0156 015f 0160 0162 0163 0165 016e 016f  .V._.`.b.c.e.n.o
+00000650: 0171 0172 0174 017d 017e 0180 0181 0183  .q.r.t.}.~......
+00000660: 018c 018d 0190 0191 0193 0194 019d 01aa  ................
+00000670: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
+00000680: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
+00000690: 01b4 2425 180a 5473 697a 6510 6108 09d4  ..$%..Tsize.a...
 000006a0: 0d0e 0f10 292a 0a0a 546b 696e 6410 7309  ....)*..Tkind.s.
 000006b0: 09d4 0d0e 0f10 2e2f 0a18 556c 6162 656c  ......./..Ulabel
 000006c0: 1064 0908 d40d 0e0f 1033 340a 1857 7665  .d.......34..Wve
 000006d0: 7273 696f 6e10 4b09 08d4 0d0e 0f10 3839  rsion.K.......89
 000006e0: 0a18 5863 6f6d 6d65 6e74 7311 012c 0908  ..Xcomments..,..
 000006f0: d40d 0e0f 103d 3e18 185e 6461 7465 4c61  .....=>..^dateLa
 00000700: 7374 4f70 656e 6564 10c8 0808 d40d 0e0f  stOpened........
@@ -1035,17 +1035,17 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 003f  ._lg1Scomp.....?
-00004110: e690 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
+00004110: e687 0000 000b 005f 005f 0070 0079 0063  ......._._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 ff8d e56c 4e07 c541  blob.......lN..A
+00004130: 626c 6f62 0000 0008 b90a 572b b90a c541  blob......W+...A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
 00004160: 6f62 0000 0008 ff8d e56c 4e07 c541 0000  ob.......lN..A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 004d c000 0000 0006 0061 0073  .....M.......a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
@@ -1351,154 +1351,154 @@
 00005460: 6200 0000 087e 81a5 d736 fec4 4100 0000  b....~...6..A...
 00005470: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
 00005480: 7070 6831 5363 6f6d 7000 0000 0000 0150  pph1Scomp......P
 00005490: 0000 0000 0800 6400 6100 7300 6800 5f00  ......d.a.s.h._.
 000054a0: 6100 7000 7076 5372 6e6c 6f6e 6700 0000  a.p.pvSrnlong...
 000054b0: 0100 0000 0f00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
 000054c0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000054d0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
+000054d0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 000054e0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 000054f0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00005500: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00005510: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00005520: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00005530: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00005540: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00005550: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00005560: 7b7b 3233 322c 2031 3931 7d2c 207b 3133  {{232, 191}, {13
-00005570: 3032 2c20 3731 347d 7d09 0817 2531 3d49  02, 714}}...%1=I
-00005580: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
-000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
-000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
-000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
-000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00005600: 0000 0004 0cde 0000 000f 0064 0061 0074  ...........d.a.t
-00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
-00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
-00005630: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
-00005640: 0405 0607 0809 0a0b 1949 4a0a 4c58 6963  .........IJ.LXic
-00005650: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00005660: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00005670: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00005680: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00005690: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-000056a0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-000056b0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-000056c0: 2340 3000 0000 0000 0009 ab0c 151d 2226  #@0..........."&
-000056d0: 2b30 353a 3f44 d40d 0e0f 1011 120a 0a5a  +05:?D.........Z
-000056e0: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
-000056f0: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00005700: 6c65 546e 616d 6511 01c7 0909 d416 1718  leTname.........
-00005710: 0d19 1a19 1c57 7669 7369 626c 6555 7769  .....WvisibleUwi
-00005720: 6474 6859 6173 6365 6e64 696e 6708 1023  dthYascending..#
-00005730: 0858 7562 6971 7569 7479 d40d 0e0f 101e  .Xubiquity......
-00005740: 1f19 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-00005750: 10b5 0809 d40d 0e0f 1023 1f19 195b 6461  .........#...[da
-00005760: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
-00005770: 2728 190a 5473 697a 6510 6108 09d4 0d0e  '(..Tsize.a.....
-00005780: 0f10 2c2d 0a0a 546b 696e 6410 7309 09d4  ..,-..Tkind.s...
-00005790: 0d0e 0f10 3132 0a19 556c 6162 656c 1064  ....12..Ulabel.d
-000057a0: 0908 d40d 0e0f 1036 370a 1957 7665 7273  .......67..Wvers
-000057b0: 696f 6e10 4b09 08d4 0d0e 0f10 3b3c 0a19  ion.K.......;<..
-000057c0: 5863 6f6d 6d65 6e74 7311 012c 0908 d40d  Xcomments..,....
-000057d0: 0e0f 1040 4119 195e 6461 7465 4c61 7374  ...@A..^dateLast
-000057e0: 4f70 656e 6564 10c8 0808 d416 1718 0d19  Opened..........
-000057f0: 1f19 4708 0859 6461 7465 4164 6465 6408  ..G..YdateAdded.
-00005800: 2340 2800 0000 0000 0054 6e61 6d65 0910  #@(......Tname..
-00005810: 0100 0800 1900 2200 3400 3c00 5000 5900  ......".4.<.P.Y.
-00005820: 6400 7700 8c00 9500 9600 a200 ab00 b600  d.w.............
-00005830: bc00 c600 ce00 d300 d600 d700 d800 e100  ................
-00005840: e900 ef00 f900 fa00 fc00 fd01 0601 0f01  ................
-00005850: 1c01 1e01 1f01 2001 2901 3501 3601 3701  ...... .).5.6.7.
-00005860: 4001 4501 4701 4801 4901 5201 5701 5901  @.E.G.H.I.R.W.Y.
-00005870: 5a01 5b01 6401 6a01 6c01 6d01 6e01 7701  Z.[.d.j.l.m.n.w.
-00005880: 7f01 8101 8201 8301 8c01 9501 9801 9901  ................
-00005890: 9a01 a301 b201 b401 b501 b601 bf01 c001  ................
-000058a0: c101 cb01 cc01 d501 da01 db00 0000 0000  ................
-000058b0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-000058c0: 0000 0000 0000 0000 0001 dd00 0000 0f00  ................
-000058d0: 6400 6100 7400 6100 5f00 7000 7200 6f00  d.a.t.a._.p.r.o.
-000058e0: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
-000058f0: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-00005900: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
-00005910: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
-00005920: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00005930: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00005940: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00005950: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00005960: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00005970: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00005980: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
-00005990: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-000059a0: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-000059b0: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-000059c0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-000059d0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-000059e0: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-000059f0: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
-00005a00: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-00005a10: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
-00005a20: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
-00005a30: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-00005a40: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-00005a50: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-00005a60: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-00005a70: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00005a80: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00005a90: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00005aa0: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00005ab0: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00005ac0: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-00005ad0: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-00005ae0: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-00005af0: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-00005b00: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-00005b10: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-00005b20: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-00005b30: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-00005b40: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-00005b50: 0000 0000 0001 ac00 0000 0f00 6400 6100  ............d.a.
-00005b60: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
-00005b70: 7300 7300 6f00 7200 736d 6f44 4462 6c6f  s.s.o.r.smoDDblo
-00005b80: 6200 0000 0826 88c2 29b9 08c5 4100 0000  b....&..)...A...
-00005b90: 0f00 6400 6100 7400 6100 5f00 7000 7200  ..d.a.t.a._.p.r.
-00005ba0: 6f00 6300 6500 7300 7300 6f00 7200 736d  o.c.e.s.s.o.r.sm
-00005bb0: 6f64 4462 6c6f 6200 0000 0826 88c2 29b9  odDblob....&..).
-00005bc0: 08c5 4100 0000 0f00 6400 6100 7400 6100  ..A.....d.a.t.a.
-00005bd0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-00005be0: 6f00 7200 7370 6831 5363 6f6d 7000 0000  o.r.sph1Scomp...
-00005bf0: 0000 0560 0000 0000 0f00 6400 6100 7400  ...`......d.a.t.
-00005c00: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
-00005c10: 7300 6f00 7200 7376 5372 6e6c 6f6e 6700  s.o.r.svSrnlong.
-00005c20: 0000 0100 0000 1200 6600 6500 6100 7400  ........f.e.a.t.
-00005c30: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
-00005c40: 6100 6300 7400 6f00 7200 7362 7773 7062  a.c.t.o.r.sbwspb
-00005c50: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
-00005c60: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00005c70: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00005c80: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00005c90: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00005ca0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00005cb0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00005cc0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00005cd0: 0808 0908 095f 1019 7b7b 3233 322c 2031  ....._..{{232, 1
-00005ce0: 3931 7d2c 207b 3133 3032 2c20 3731 347d  91}, {1302, 714}
-00005cf0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00005d00: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
-00005d10: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00005d20: 9b00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
-00005d30: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
-00005d40: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
-00005d50: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
-00005d60: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
-00005d70: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d80: 6d70 0000 0000 0015 6160 1640 0810 c808  mp......a`.@....
+00005550: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
+00005560: 7b7b 3131 322c 2035 357d 2c20 7b31 3139  {{112, 55}, {119
+00005570: 392c 2037 3639 7d7d 0908 1725 313d 4960  9, 769}}...%1=I`
+00005580: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
+00005590: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+000055a0: 0000 0000 0000 009a 0000 000f 0064 0061  .............d.a
+000055b0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
+000055c0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
+000055d0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
+000055e0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+000055f0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
+00005600: 0000 0453 9a00 0000 0f00 6400 6100 7400  ...S......d.a.t.
+00005610: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
+00005620: 7300 6f00 7200 736c 7376 4362 6c6f 6200  s.o.r.slsvCblob.
+00005630: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
+00005640: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
+00005650: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00005660: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00005670: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00005680: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00005690: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+000056a0: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+000056b0: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+000056c0: 0109 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
+000056d0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
+000056e0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+000056f0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+00005700: 01c7 0909 d410 0e0f 0d16 1716 1908 1023  ...............#
+00005710: 0858 7562 6971 7569 7479 d40d 0e0f 101b  .Xubiquity......
+00005720: 1c16 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00005730: 10b5 0809 d40d 0e0f 1020 1c16 165b 6461  ......... ...[da
+00005740: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
+00005750: 2425 160a 5473 697a 6510 6108 09d4 0d0e  $%..Tsize.a.....
+00005760: 0f10 292a 0a0a 546b 696e 6410 7309 09d4  ..)*..Tkind.s...
+00005770: 0d0e 0f10 2e2f 0a16 556c 6162 656c 1064  ...../..Ulabel.d
+00005780: 0908 d40d 0e0f 1033 340a 1657 7665 7273  .......34..Wvers
+00005790: 696f 6e10 4b09 08d4 0d0e 0f10 3839 0a16  ion.K.......89..
+000057a0: 5863 6f6d 6d65 6e74 7311 012c 0908 d40d  Xcomments..,....
+000057b0: 0e0f 103d 3e16 165e 6461 7465 4c61 7374  ...=>..^dateLast
+000057c0: 4f70 656e 6564 10c8 0808 d410 0e0f 0d16  Opened..........
+000057d0: 1c16 4408 0859 6461 7465 4164 6465 6408  ..D..YdateAdded.
+000057e0: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
+000057f0: 6469 6669 6564 2340 3000 0000 0000 0009  dified#@0.......
+00005800: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+00005810: 0079 008c 008e 008f 009b 00a4 00af 00b5  .y..............
+00005820: 00bf 00c7 00cc 00cf 00d0 00d1 00da 00db  ................
+00005830: 00dd 00de 00e7 00f0 00fd 00ff 0100 0101  ................
+00005840: 010a 0116 0117 0118 0121 0126 0128 0129  .........!.&.(.)
+00005850: 012a 0133 0138 013a 013b 013c 0145 014b  .*.3.8.:.;.<.E.K
+00005860: 014d 014e 014f 0158 0160 0162 0163 0164  .M.N.O.X.`.b.c.d
+00005870: 016d 0176 0179 017a 017b 0184 0193 0195  .m.v.y.z.{......
+00005880: 0196 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
+00005890: 01c3 01cc 0000 0000 0000 0201 0000 0000  ................
+000058a0: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+000058b0: 0000 01cd 0000 000f 0064 0061 0074 0061  .........d.a.t.a
+000058c0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+000058d0: 006f 0072 0073 6c73 7670 626c 6f62 0000  .o.r.slsvpblob..
+000058e0: 0266 6270 6c69 7374 3030 d801 0203 0405  .fbplist00......
+000058f0: 0607 0809 0a0b 1a45 4647 0a5f 1012 7669  .......EFG._..vi
+00005900: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00005910: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00005920: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00005930: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00005940: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+00005950: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+00005960: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
+00005970: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
+00005980: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
+00005990: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+000059a0: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+000059b0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+000059c0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+000059d0: 6d65 d416 1718 191a 1b0a 1d57 7669 7369  me.........Wvisi
+000059e0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+000059f0: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
+00005a00: d416 1718 191a 201a 2208 10c8 0810 08d4  ...... .".......
+00005a10: 1617 1819 0a25 1a09 0910 b508 d416 1718  .....%..........
+00005a20: 191a 251a 2a08 0810 02d4 1617 1819 0a2d  ..%.*..........-
+00005a30: 1a2f 0910 6108 1003 d416 1718 191a 320a  ./..a.........2.
+00005a40: 3408 1064 0910 05d4 1617 1819 0a37 0a39  4..d.........7.9
+00005a50: 0910 7309 1004 d416 1718 191a 3c0a 3e08  ..s.........<.>.
+00005a60: 104b 0910 06d4 1617 1819 0a41 0a43 0911  .K.........A.C..
+00005a70: 01c7 0910 0008 2340 2800 0000 0000 005c  ......#@(......\
+00005a80: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
+00005a90: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00005aa0: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
+00005ab0: 00ab 00ba 00c7 00d3 00d8 00de 00e3 00eb  ................
+00005ac0: 00f0 00f9 0101 0107 0111 0117 0118 011b  ................
+00005ad0: 011c 011e 0127 0128 012a 012b 012d 0136  .....'.(.*.+.-.6
+00005ae0: 0137 0139 013a 0143 0144 0145 0147 0150  .7.9.:.C.D.E.G.P
+00005af0: 0151 0153 0154 0156 015f 0160 0162 0163  .Q.S.T.V._.`.b.c
+00005b00: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
+00005b10: 0180 0181 0183 018c 018d 0190 0191 0193  ................
+00005b20: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
+00005b30: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00005b40: 0000 0000 0000 01b4 0000 000f 0064 0061  .............d.a
+00005b50: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
+00005b60: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
+00005b70: 6f62 0000 0008 3ebd 23b1 6d0b c541 0000  ob....>.#.m..A..
+00005b80: 000f 0064 0061 0074 0061 005f 0070 0072  ...d.a.t.a._.p.r
+00005b90: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
+00005ba0: 6d6f 6444 626c 6f62 0000 0008 b622 20d2  modDblob....." .
+00005bb0: 610b c541 0000 000f 0064 0061 0074 0061  a..A.....d.a.t.a
+00005bc0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+00005bd0: 006f 0072 0073 7068 3153 636f 6d70 0000  .o.r.sph1Scomp..
+00005be0: 0000 0005 b000 0000 000f 0064 0061 0074  ...........d.a.t
+00005bf0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
+00005c00: 0073 006f 0072 0073 7653 726e 6c6f 6e67  .s.o.r.svSrnlong
+00005c10: 0000 0001 0000 0012 0066 0065 0061 0074  .........f.e.a.t
+00005c20: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
+00005c30: 0061 0063 0074 006f 0072 0073 6277 7370  .a.c.t.o.r.sbwsp
+00005c40: 626c 6f62 0000 00c9 6270 6c69 7374 3030  blob....bplist00
+00005c50: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
+00005c60: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+00005c70: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
+00005c80: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00005c90: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00005ca0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00005cb0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00005cc0: 7208 0809 0809 5f10 187b 7b31 3132 2c20  r....._..{{112, 
+00005cd0: 3535 7d2c 207b 3131 3939 2c20 3736 397d  55}, {1199, 769}
+00005ce0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
+00005cf0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
+00005d00: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
+00005d10: 9a00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
+00005d20: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
+00005d30: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
+00005d40: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
+00005d50: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
+00005d60: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
+00005d70: 6d70 0000 0000 0015 6160 5863 6f6d 6d65  mp......a`Xcomme
+00005d80: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
 00005d90: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
 00005da0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
 00005db0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
 00005dc0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
 00005dd0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
 00005de0: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
 00005df0: c700 c800 cb00 cc00 d100 da00 db00 dd00  ................
@@ -1700,73 +1700,73 @@
 00006a30: 6444 626c 6f62 0000 0008 c446 b51b 4305  dDblob.....F..C.
 00006a40: c541 0000 0009 006c 0061 0062 0065 006c  .A.....l.a.b.e.l
 00006a50: 006c 0069 006e 0067 7068 3153 636f 6d70  .l.i.n.gph1Scomp
 00006a60: 0000 0000 0002 a000 0000 0009 006c 0061  .............l.a
 00006a70: 0062 0065 006c 006c 0069 006e 0067 7653  .b.e.l.l.i.n.gvS
 00006a80: 726e 6c6f 6e67 0000 0001 0000 0006 006d  rnlong.........m
 00006a90: 0069 0078 0069 006e 0073 6277 7370 626c  .i.x.i.n.sbwspbl
-00006aa0: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
+00006aa0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
 00006ab0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00006ac0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00006ad0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00006ae0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00006af0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00006b00: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00006b10: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00006b20: 0809 0809 5f10 197b 7b32 3332 2c20 3139  ...._..{{232, 19
-00006b30: 317d 2c20 7b31 3330 322c 2037 3134 7d7d  1}, {1302, 714}}
-00006b40: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00006b50: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00006b60: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-00006b70: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00006b80: 6c67 3153 636f 6d70 0000 0000 000f 9022  lg1Scomp......."
-00006b90: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00006ba0: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
-00006bb0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-00006bc0: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
-00006bd0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00006be0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00006bf0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00006c00: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00006c10: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00006c20: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00006c30: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00006c40: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
-00006c50: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
-00006c60: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-00006c70: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-00006c80: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
-00006c90: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-00006ca0: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
-00006cb0: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
-00006cc0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
-00006cd0: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
-00006ce0: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
-00006cf0: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
-00006d00: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
-00006d10: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
-00006d20: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
-00006d30: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
-00006d40: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
-00006d50: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
-00006d60: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
-00006d70: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-00006d80: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
-00006d90: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
-00006da0: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
-00006db0: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
-00006dc0: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
-00006dd0: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
-00006de0: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
-00006df0: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
-00006e00: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
-00006e10: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
-00006e20: da01 db00 0000 0000 0002 0100 0000 0000  ................
-00006e30: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-00006e40: 0001 dd01 7201 7b01 8401 8501 8701 8801  ....r.{.........
+00006b20: 0809 0809 5f10 187b 7b31 3332 2c20 3335  ...._..{{132, 35
+00006b30: 7d2c 207b 3131 3939 2c20 3736 397d 7d09  }, {1199, 769}}.
+00006b40: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+00006b50: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00006b60: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+00006b70: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
+00006b80: 6731 5363 6f6d 7000 0000 0000 0f9a 2d00  g1Scomp.......-.
+00006b90: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
+00006ba0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
+00006bb0: 7430 30d8 0102 0304 0506 0708 090a 0b16  t00.............
+00006bc0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+00006bd0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00006be0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00006bf0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00006c00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00006c10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+00006c20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+00006c30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+00006c40: 282d 3237 3c41 d40d 0e0f 1011 120a 0a5a  (-27<A.........Z
+00006c50: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
+00006c60: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00006c70: 6c65 546e 616d 6511 01c7 0909 d410 0e0f  leTname.........
+00006c80: 0d16 1716 1908 1023 0858 7562 6971 7569  .......#.Xubiqui
+00006c90: 7479 d40d 0e0f 101b 1c16 0a5c 6461 7465  ty.........\date
+00006ca0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+00006cb0: 1020 1c16 165b 6461 7465 4372 6561 7465  . ...[dateCreate
+00006cc0: 6408 08d4 0d0e 0f10 2425 160a 5473 697a  d.......$%..Tsiz
+00006cd0: 6510 6108 09d4 0d0e 0f10 292a 0a0a 546b  e.a.......)*..Tk
+00006ce0: 696e 6410 7309 09d4 0d0e 0f10 2e2f 0a16  ind.s......../..
+00006cf0: 556c 6162 656c 1064 0908 d40d 0e0f 1033  Ulabel.d.......3
+00006d00: 340a 1657 7665 7273 696f 6e10 4b09 08d4  4..Wversion.K...
+00006d10: 0d0e 0f10 3839 0a16 5863 6f6d 6d65 6e74  ....89..Xcomment
+00006d20: 7311 012c 0908 d40d 0e0f 103d 3e16 165e  s..,.......=>..^
+00006d30: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+00006d40: 0808 d410 0e0f 0d16 1c16 4408 0859 6461  ..........D..Yda
+00006d50: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+00006d60: 005c 6461 7465 4d6f 6469 6669 6564 2340  .\dateModified#@
+00006d70: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
+00006d80: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
+00006d90: 009b 00a4 00af 00b5 00bf 00c7 00cc 00cf  ................
+00006da0: 00d0 00d1 00da 00db 00dd 00de 00e7 00f0  ................
+00006db0: 00fd 00ff 0100 0101 010a 0116 0117 0118  ................
+00006dc0: 0121 0126 0128 0129 012a 0133 0138 013a  .!.&.(.).*.3.8.:
+00006dd0: 013b 013c 0145 014b 014d 014e 014f 0158  .;.<.E.K.M.N.O.X
+00006de0: 0160 0162 0163 0164 016d 0176 0179 017a  .`.b.c.d.m.v.y.z
+00006df0: 017b 0184 0193 0195 0196 0197 01a0 01a1  .{..............
+00006e00: 01a2 01ac 01ad 01b6 01c3 01cc 0000 0000  ................
+00006e10: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
+00006e20: 0000 0000 0000 0000 0000 01cd 4601 4801  ............F.H.
+00006e30: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
+00006e40: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
 00006e50: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
 00006e60: c400 0000 0000 0002 0100 0000 0000 0000  ................
 00006e70: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
 00006e80: c500 0000 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,15 +1788,15 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 e997 ad04 050a c541  blob...........A
+00007020: 626c 6f62 0000 0008 b5bc c412 5e0b c541  blob........^..A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00007040: 6d6f 6444 626c 6f62 0000 0008 e997 ad04  modDblob........
 00007050: 050a c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
 00007070: 0010 f000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
@@ -1811,15 +1811,15 @@
 00007120: 6261 7208 0809 0809 5f10 197b 7b32 3332  bar....._..{{232
 00007130: 2c20 3139 317d 2c20 7b31 3330 322c 2037  , 191}, {1302, 7
 00007140: 3134 7d7d 0908 1725 313d 4960 6d79 7a7b  14}}...%1=I`myz{
 00007150: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00007160: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 009b 0000 0005 006d 006f 0064 0065  .........m.o.d.e
 00007180: 006c 6c67 3153 636f 6d70 0000 0000 0001  .llg1Scomp......
-00007190: 7d9d 0000 0005 006d 006f 0064 0065 006c  }......m.o.d.e.l
+00007190: 7e99 0000 0005 006d 006f 0064 0065 006c  ~......m.o.d.e.l
 000071a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 000071b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 000071c0: 1846 470a 4958 6963 6f6e 5369 7a65 5f10  .FG.IXiconSize_.
 000071d0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 000071e0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
 000071f0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
 00007200: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
@@ -1893,15 +1893,15 @@
 00007640: 4d01 4e01 5001 5901 5a01 5b01 5d01 5f01  M.N.P.Y.Z.[.]._.
 00007650: 6801 6901 6a01 6c01 6e01 7701 7801 7901  h.i.j.l.n.w.x.y.
 00007660: 7b01 7d01 8601 8701 8801 8a01 8c01 9501  {.}.............
 00007670: 9601 9701 9a01 9c01 9d01 a601 ab00 0000  ................
 00007680: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
 00007690: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
 000076a0: 0500 6d00 6f00 6400 6500 6c6d 6f44 4462  ..m.o.d.e.lmoDDb
-000076b0: 6c6f 6200 0000 086a 5858 d003 0ac5 4100  lob....jXX....A.
+000076b0: 6c6f 6200 0000 087f 06db 23b9 0ac5 4100  lob.......#...A.
 000076c0: 0000 0500 6d00 6f00 6400 6500 6c6d 6f64  ....m.o.d.e.lmod
 000076d0: 4462 6c6f 6200 0000 08dc c0ca 73c2 04c5  Dblob.......s...
 000076e0: 4100 0000 0500 6d00 6f00 6400 6500 6c70  A.....m.o.d.e.lp
 000076f0: 6831 5363 6f6d 7000 0000 0000 01c0 0000  h1Scomp.........
 00007700: 0000 0500 6d00 6f00 6400 6500 6c76 5372  ....m.o.d.e.lvSr
 00007710: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00007720: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
@@ -2035,15 +2035,15 @@
 00007f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 00007f30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
 00007f40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
 00007f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00007f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00007f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 00007f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00007f90: 3153 636f 6d70 0000 0000 000c 94f1 0000  1Scomp..........
+00007f90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,20 +2088,20 @@
 00008270: 7901 7b01 7d01 7e01 7f01 8801 8a01 8c01  y.{.}.~.........
 00008280: 8d01 8e01 9701 9901 9b01 9c01 9d01 a601  ................
 00008290: a801 aa01 ab01 ac01 b501 b701 ba01 bb01  ................
 000082a0: bc01 bd01 c601 cf01 dc00 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 087a 937f 148d 0ac5  Dblob....z......
+000082e0: 4462 6c6f 6200 0000 086f d1b6 5abb 0ac5  Dblob....o..Z...
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 087a 937f 148d 0ac5 4100 0000 0800 7000  .z......A.....p.
+00008310: 086f d1b6 5abb 0ac5 4100 0000 0800 7000  .o..Z...A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
-00008330: 5363 6f6d 7000 0000 0000 0fc0 0000 0000  Scomp...........
+00008330: 5363 6f6d 7000 0000 0000 0fb0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
 00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
 00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
 00008390: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000083a0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
@@ -2264,15 +2264,15 @@
 00008d70: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00008d80: 0000 0000 0000 0000 0000 009a 0000 000e  ................
 00008d90: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
 00008da0: 006f 0072 0074 0065 0072 0073 6473 636c  .o.r.t.e.r.sdscl
 00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
 00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
-00008de0: 0000 03f6 d372 005f 0074 006f 006f 006c  .....r._.t.o.o.l
+00008de0: 0000 03f6 c772 005f 0074 006f 006f 006c  .....r._.t.o.o.l
 00008df0: 0073 6d6f 4444 626c 6f62 0000 0008 56b2  .smoDDblob....V.
 00008e00: f350 8b0a c541 0000 000d 006f 0075 0074  .P...A.....o.u.t
 00008e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
 00008e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
 00008e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
 00008e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00008e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
@@ -2291,15 +2291,15 @@
 00008f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 00008f30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
 00008f40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
 00008f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00008f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00008f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 00008f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00008f90: 3153 636f 6d70 0000 0000 000c 94f1 0000  1Scomp..........
+00008f90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2342,15 +2342,15 @@
 00009250: 0160 0162 0163 0165 016e 016f 0171 0172  .`.b.c.e.n.o.q.r
 00009260: 0174 017d 017e 0180 0181 0183 018c 018d  .t.}.~..........
 00009270: 0190 0191 0193 0194 019d 01aa 01b3 0000  ................
 00009280: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
 00009290: 0000 0000 0000 0000 0000 0000 01b4 0000  ................
 000092a0: 000e 0070 006f 0073 0065 005f 0069 006d  ...p.o.s.e._.i.m
 000092b0: 0070 006f 0072 0074 0065 0072 0073 6d6f  .p.o.r.t.e.r.smo
-000092c0: 4444 626c 6f62 0000 0008 c8fd 00c6 030a  DDblob..........
+000092c0: 4444 626c 6f62 0000 0008 487a 6cbc b80a  DDblob....Hzl...
 000092d0: c541 0000 000e 0070 006f 0073 0065 005f  .A.....p.o.s.e._
 000092e0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
 000092f0: 0073 6d6f 6444 626c 6f62 0000 0008 eacd  .smodDblob......
 00009300: db43 ad08 c541 0000 000e 0070 006f 0073  .C...A.....p.o.s
 00009310: 0065 005f 0069 006d 0070 006f 0072 0074  .e._.i.m.p.o.r.t
 00009320: 0065 0072 0073 7068 3153 636f 6d70 0000  .e.r.sph1Scomp..
 00009330: 0000 0004 f000 0000 000e 0070 006f 0073  ...........p.o.s
@@ -2547,15 +2547,15 @@
 00009f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 00009f30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
 00009f40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
 00009f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 00009f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 00009f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 00009f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00009f90: 3153 636f 6d70 0000 0000 000c 94f1 0000  1Scomp..........
+00009f90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
@@ -2707,15 +2707,15 @@
 0000a920: 0809 5f10 187b 7b31 3132 2c20 3535 7d2c  .._..{{112, 55},
 0000a930: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
 0000a940: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 0000a950: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 0000a960: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
 0000a970: 0200 7500 6964 7363 6c62 6f6f 6c00 0000  ..u.idsclbool...
 0000a980: 0002 0075 0069 6c67 3153 636f 6d70 0000  ...u.ilg1Scomp..
-0000a990: 0000 0009 4165 0000 0002 0075 0069 6c73  ....Ae.....u.ils
+0000a990: 0000 0009 419c 0000 0002 0075 0069 6c73  ....A......u.ils
 0000a9a0: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
 0000a9b0: 3030 d801 0203 0405 0607 0809 0a0b 1846  00.............F
 0000a9c0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
 0000a9d0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 0000a9e0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 0000a9f0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
 0000aa00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
@@ -2803,15 +2803,15 @@
 0000af20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 0000af30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
 0000af40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
 0000af50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 0000af60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 0000af70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 0000af80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-0000af90: 3153 636f 6d70 0000 0000 000c 94f1 0000  1Scomp..........
+0000af90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2963,15 +2963,15 @@
 0000b920: 0809 5f10 187b 7b31 3132 2c20 3535 7d2c  .._..{{112, 55},
 0000b930: 207b 3131 3939 2c20 3736 397d 7d09 0817   {1199, 769}}...
 0000b940: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 0000b950: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
 0000b960: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
 0000b970: 0200 7500 6964 7363 6c62 6f6f 6c00 0000  ..u.idsclbool...
 0000b980: 0002 0075 0069 6c67 3153 636f 6d70 0000  ...u.ilg1Scomp..
-0000b990: 0000 0009 4165 0000 0002 0075 0069 6c73  ....Ae.....u.ils
+0000b990: 0000 0009 419c 0000 0002 0075 0069 6c73  ....A......u.ils
 0000b9a0: 7643 626c 6f62 0000 0279 6270 6c69 7374  vCblob...ybplist
 0000b9b0: 3030 d801 0203 0405 0607 0809 0a0b 1846  00.............F
 0000b9c0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
 0000b9d0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
 0000b9e0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
 0000b9f0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
 0000ba00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
@@ -3059,15 +3059,15 @@
 0000bf20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
 0000bf30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
 0000bf40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
 0000bf50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
 0000bf60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
 0000bf70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
 0000bf80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-0000bf90: 3153 636f 6d70 0000 0000 000c 94f1 0000  1Scomp..........
+0000bf90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/perimeter_jit.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,35 +61,37 @@
             results[i] = area(x_sorted, y_sorted)
 
     return results
 
 
 @jit(nopython=True)
 def jitted_centroid(points: np.ndarray) -> np.ndarray:
-
     """
+    Compute the centroid of polygons.
+
     :param array points: 3d array FRAMESxBODY-PARTxCOORDINATE
     :param str target: Options [perimeter, area]
-    :return: 1d np.array
+    :return 1d np.array
 
-    :EXAMPLE:
+    :example:
     >>> points = np.random.randint(1, 50, size=(50, 5, 2)).astype(float)
     >>> results = jitted_centroid(points)
     """
+
     results = np.full((points.shape[0], 2), np.nan)
     for i in range(points.shape[0]):
         S = points[i, :, :]
         a, b = np.argmin(S[:,0]), np.argmax(S[:,0])
         max_index = np.argmax(S[:,0])
         idx = process(S, np.arange(S.shape[0]), a, max_index)[:-1] + process(S, np.arange(S.shape[0]), max_index, a)[:-1]
         perimeter_points = np.full((len(idx), 2), np.nan)
         for j in prange(len(idx)):
             perimeter_points[j] = points[i][j]
         results[i][0] = np.int(np.mean(perimeter_points[:, 0].flatten()))
         results[i][1] = np.int(np.mean(perimeter_points[:, 1].flatten()))
     return results
 
-points = np.random.randint(1, 10, size=(50, 5, 2)).astype(np.float32)
-results = jitted_centroid(points)
+# points = np.random.randint(1, 10, size=(50, 5, 2)).astype(np.float32)
+# results = jitted_centroid(points)
 #
 #
 # results = np.full((points.shape[0]), np.nan)
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.8/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.59.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi` & `Simba-UW-tf-dev-1.59.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/feature_extraction_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     @staticmethod
     def convex_hull_calculator_mp(arr: np.ndarray, px_per_mm: float) -> float:
         """
         Calculate single frame convex hull perimeter length in millimeters.
 
         .. seealso::
             For acceptable run-time, call using ``parallel.delayed``.
-            For large data, use meth:`simba.feature_extractors.perimeter_jit.jitted_hull`.
+            For large data, use :meth:`simba.feature_extractors.perimeter_jit.jitted_hull`.
 
         :parameter np.ndarray arr: 2D array of size len(body-parts) x 2.
         :parameter float px_per_mm: Video pixels per millimeter.
         :return float: The length of the animal perimeter in millimeters.
 
         :example:
         >>> coordinates = np.random.randint(1, 200, size=(6, 2)).astype(np.float32)
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/plotting_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,26 +122,26 @@
             rgb.reverse()
             if as_hex:
                 rgb = matplotlib.colors.to_hex(rgb)
             color_lst.append(rgb)
         return color_lst
 
     def remove_a_folder(self,
-                        folder_dir: str):
+                        folder_dir: str) -> None:
         """Helper to remove a directory, use for cleaning up smaller multiprocessed videos following concat"""
         shutil.rmtree(folder_dir, ignore_errors=True)
 
     def split_and_group_df(self,
                            df: pd.DataFrame,
                            splits: int,
                            include_split_order: bool = True) -> (List[pd.DataFrame], int):
 
         """
-        Helper to split a dataframe for multiprocessing. If include_split_order, then include the group number in split data.
-        Returns split data and approximations of number of observations per split.
+        Helper to split a dataframe for multiprocessing. If include_split_order, then include the group number
+        in split data as a column. Returns split data and approximations of number of observations per split.
         """
 
         data_arr = np.array_split(df, splits)
         if include_split_order:
             for df_cnt in range(len(data_arr)):
                 data_arr[df_cnt]['group'] = df_cnt
         obs_per_split = len(data_arr[0])
@@ -154,40 +154,30 @@
                            style_attr: Dict[str, Any],
                            fps: int,
                            save_img: bool = False,
                            save_path: Optional[str] = None) -> np.ndarray:
         """
         Helper to make a single line plot .png image with N lines.
 
-        Parameters
-        ----------
-        data: np.array
-            Two-dimensional array where rows represent frames and columns represent values.
-        line_attr: dict
-            Line color attributes.
-        style_attr: dict
-            Image attributes (size, font size, line width etc).
-        fps: int
-            Video frame rate.
-        save_path:
-            Location to store output .png image.
-
-
-        Notes
-        -----
-        `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-distance-plots>`__.
+        :param np.array data: Two-dimensional array where rows represent frames and columns represent intertwined x and y coordinates.
+        :param dict line_attr: Line color attributes.
+        :param dict style_attr: Plot attributes (size, font size, line width etc).
+        :param int fps: Video frame rate.
+        :param Optionan[str] save_path: Location to store output .png image. If None, then return image.
 
-        Examples
-        -----
+        .. note::
+           `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-distance-plots>`__.
+
+        :example:
         >>> fps = 10
         >>> data = np.random.random((100,2))
         >>> line_attr = {0: ['Blue'], 1: ['Red']}
         >>> save_path = '/_tests/final_frm.png'
         >>> style_attr = {'width': 640, 'height': 480, 'line width': 6, 'font size': 8, 'y_max': 'auto'}
-        >>> make_distance_plot(fps=fps, data=data, line_attr=line_attr, style_attr=style_attr, save_path=save_path)
+        >>> self.make_distance_plot(fps=fps, data=data, line_attr=line_attr, style_attr=style_attr, save_path=save_path)
         """
         colors = get_color_dict()
         for j in range(data.shape[1]):
             color = (colors[line_attr[j][-1]][::-1])
             color = tuple(x / 255 for x in color)
             plt.plot(data[:, j], color=color, linewidth=style_attr['line width'], alpha=style_attr['opacity'])
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.59.8/simba/mixins/train_model_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 from simba.utils.errors import (ColumnNotFoundError,
                                 FaultyTrainingSetError,
                                 MissingColumnsError,
                                 NoDataError,
                                 SamplingError,
                                 CorruptedFileError,
                                 FeatureNumberMismatchError,
-                                ClassifierInferenceError)
+                                ClassifierInferenceError,
+                                InvalidInputError)
 from simba.utils.warnings import (NotEnoughDataWarning,
                                   NoModuleWarning,
                                   MissingUserInputWarning)
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.lookups import get_meta_data_file_headers
 
 
@@ -91,16 +92,17 @@
             print(f'Reading in file {str(file_cnt + 1)}/{str(len(file_paths))}...')
             _, vid_name, _ = get_fn_ext(file)
             df = read_df(file, file_type).dropna(axis=0, how='all').fillna(0).astype(np.float32)
             df.index = [vid_name] * len(df)
             if classifier_names != None:
                 for clf_name in classifier_names:
                     if not clf_name in df.columns:
-                        raise MissingColumnsError(
-                            msg=f'Data for video {vid_name} does not contain any annotations for behavior {clf_name}. Delete classifier {clf_name} from the SimBA project, or add annotations for behavior {clf_name} to the video {vid_name}')
+                        raise MissingColumnsError(msg=f'Data for video {vid_name} does not contain any annotations for behavior {clf_name}. Delete classifier {clf_name} from the SimBA project, or add annotations for behavior {clf_name} to the video {vid_name}')
+                    elif len(set(df[clf_name].unique()) - {0, 1}) > 0:
+                        raise InvalidInputError(msg=f'The annotation column for a classifier should contain only 0 or 1 values. However, in file {file} the {clf_name} field contains additional value(s): {list(set(df[clf_name].unique()) - {0, 1})}.')
                     else:
                         df_concat = pd.concat([df_concat, df], axis=0)
             else:
                 df_concat = pd.concat([df_concat, df], axis=0)
         try:
             df_concat = df_concat.set_index('scorer')
         except KeyError:
@@ -955,15 +957,15 @@
             if model_name and data_path:
                 raise FeatureNumberMismatchError(f'Mismatch in the number of features in input file {data_path}, and what is expected by the model {model_name}. The model expects {str(clf.n_features_)} features. The data contains {len(x_df.columns)} features.')
             else:
                 raise FeatureNumberMismatchError(f'The model expects {str(clf.n_features_)} features. The data contains {len(x_df.columns)} features.')
         p_vals = clf.predict_proba(x_df)
         if p_vals.shape[1] != 2:
             raise ClassifierInferenceError(
-                msg=f'The classifier {model_name} (at path {data_path}) has not been created properly. See The SimBA GitHub FAQ page or Gitter for more information and suggested fixes.')
+                msg=f'The classifier {model_name} (data path {data_path}) has not been created properly. See The SimBA GitHub FAQ page or Gitter for more information and suggested fixes.')
         return p_vals[:, 1]
 
     def clf_fit(self,
                 clf: RandomForestClassifier,
                 x_df: pd.DataFrame,
                 y_df: pd.DataFrame) -> RandomForestClassifier:
         """
@@ -996,14 +998,16 @@
         _, vid_name, _ = get_fn_ext(file_path)
         df = read_df(file_path, file_type).dropna(axis=0, how='all').fillna(0)
         df.index = [vid_name] * len(df)
         if clf_names != None:
             for clf_name in clf_names:
                 if not clf_name in df.columns:
                     raise ColumnNotFoundError(column_name=clf_name, file_name=file_path)
+                elif len(set(df[clf_name].unique()) - {0, 1}) > 0:
+                    raise InvalidInputError(msg=f'The annotation column for a classifier should contain only 0 or 1 values. However, in file {file_path} the {clf_name} field contains additional value(s): {list(set(df[clf_name].unique()) - {0, 1})}.')
         timer.stop_timer()
         print(f'Reading complete {vid_name} (elapsed time: {timer.elapsed_time_str}s)...')
         return df
 
     def read_all_files_in_folder_mp(self,
                                     file_paths: List[str],
                                     file_type: Literal['csv', 'parquet', 'pickle'],
@@ -1053,15 +1057,14 @@
 
         """
         Helper to check column-wise NaNs in raw input data for fitting model.
 
         :param pd.DataFrame df
         :param str logs_path: The logs directory of the SimBA project
         :raise FaultyTrainingSetError: When the dataset contains NaNs
-
         """
 
         nan_cols = df.reset_index(drop=True).replace([np.inf, -np.inf, None], np.nan).columns[df.isna().any()].tolist()
         if len(nan_cols) == 0:
             return df.reset_index(drop=True)
         else:
             save_log_path = os.path.join(logs_path, f'missing_columns_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
@@ -1074,8 +1077,24 @@
                 for video in nan_videos: results[video][nan_col] = False
                 for video in non_nan_video: results[video][nan_col] = True
             results = pd.DataFrame.from_dict(data=results, orient='index')
             results.to_csv(save_log_path)
             raise FaultyTrainingSetError(
                 msg=f'{len(nan_cols)} feature columns exist in some files, but missing in others. The feature files are found in the project_folder/csv/targets_inserted directory. ' \
                     f'SimBA expects all files within the project_folder/csv/targets_inserted directory to have the same number of features: the first 10 ' \
-                    f'column names with mismatches are: {nan_cols[0:9]}. For a log of the files that contain, and not contain, the mis-matched columns, see {save_log_path}')
+                    f'column names with mismatches are: {nan_cols[0:9]}. For a log of the files that contain, and not contain, the mis-matched columns, see {save_log_path}')
+
+
+# test = TrainModelMixin()
+# test.read_all_files_in_folder(file_paths=['/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437C_c3_2022-11-01_13-16-23_color.csv', '/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437D_c4_2022-11-01_13-16-39_color.csv'],
+#                               file_type='csv', classifier_names=['attack', 'non-agresive parallel swimming'])
+
+
+# test = TrainModelMixin()
+# test.read_all_files_in_folder_mp(file_paths=['/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437C_c3_2022-11-01_13-16-23_color.csv', '/Users/simon/Desktop/envs/troubleshooting/jake/project_folder/csv/targets_inserted/22-437D_c4_2022-11-01_13-16-39_color.csv'],
+#                               file_type='csv', classifier_names=['attack', 'non-agresive parallel swimming'])
+#
+#     #
+    # def read_all_files_in_folder(self,
+    #                              file_paths: List[str],
+    #                              file_type: str,
+    #                              classifier_names: Optional[List[str]] = None) -> pd.DataFrame:
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.59.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.59.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/ez_lineplot.py`

 * *Files 20% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     img = np.uint8(img)
 
     fourcc = cv2.VideoWriter_fourcc(*'MJPG')
     out = cv2.VideoWriter(os.path.join(outputvideopath, video), 0x7634706d, fps, (width, height))
     counter = 0
     while (vcap.isOpened()):
         ret, frame = vcap.read()
-        if ret == True:
+        if ret:
             if counter != 0:
                 cv2.line(img, circletup[counter - 1], circletup[counter], 5)
 
             lineWithCircle = img.copy()
             cv2.circle(lineWithCircle, circletup[counter], 5, [0, 0, 255], -1)
 
             out.write(lineWithCircle)
@@ -136,64 +136,8 @@
             print('Frame ' + str(counter) + '/' + str(totalFrameCount))
 
         else:
             break
 
     vcap.release()
     cv2.destroyAllWindows()
-    print('Video generated.')
-
-def draw_line_plot_tools(videopath, csvfile, bodypart):
-    inputDf = pd.read_csv(csvfile)
-
-    # restructure
-    col1 = inputDf.loc[0].to_list()
-    col2 = inputDf.loc[1].to_list()
-    finalcol = [m + '_' + n for m, n in zip(col1, col2)]
-    inputDf.columns = finalcol
-    inputDf = inputDf.loc[2:]
-    print(inputDf.columns)
-    inputDf = inputDf.reset_index(drop=True)
-    # datacleaning
-    colHeads = [bodypart + '_x', bodypart + '_y', bodypart + '_likelihood']
-    df = inputDf[colHeads].copy()
-
-    widthlist = df[colHeads[0]].astype(float).astype(int)
-    heightlist = df[colHeads[1]].astype(float).astype(int)
-    circletup = tuple(zip(widthlist, heightlist))
-
-    # get resolution of video
-    vcap = cv2.VideoCapture(videopath)
-    if vcap.isOpened():
-        width = int(vcap.get(cv2.CAP_PROP_FRAME_WIDTH))  # float
-        height = int(vcap.get(cv2.CAP_PROP_FRAME_HEIGHT))  # float
-        fps = int(vcap.get(cv2.CAP_PROP_FPS))
-        totalFrameCount = int(vcap.get(cv2.CAP_PROP_FRAME_COUNT))
-
-    # make white background
-    img = np.zeros([height, width, 3])
-    img.fill(255)
-    img = np.uint8(img)
-
-    outputvideoname = os.path.join(os.path.dirname(videopath), 'line_plot' + os.path.basename(videopath))
-    fourcc = cv2.VideoWriter_fourcc(*'MJPG')
-    out = cv2.VideoWriter(outputvideoname, 0x7634706d, fps, (width, height))
-    counter = 0
-    while (vcap.isOpened()):
-        ret, frame = vcap.read()
-        if ret == True:
-            if counter != 0:
-                cv2.line(img, circletup[counter - 1], circletup[counter], 5)
-
-            lineWithCircle = img.copy()
-            cv2.circle(lineWithCircle, circletup[counter], 5, [0, 0, 255], -1)
-
-            out.write(lineWithCircle)
-            counter += 1
-            print('Frame ' + str(counter) + '/' + str(totalFrameCount))
-
-        else:
-            break
-
-    vcap.release()
-    cv2.destroyAllWindows()
-    stdout_success(msg='Video generated.')
+    print('Video generated.')
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.59.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.59.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.59.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.59.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/severity_calculator_2.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,45 +10,58 @@
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.printing import stdout_success
 from simba.utils.warnings import NoDataFoundWarning
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 
-class SeverityCalculator(ConfigReader, FeatureExtractionMixin):
+class SeverityBoutCalculator(ConfigReader, FeatureExtractionMixin):
     """
-    Computes the "severity" of classification frame events based on how much
-    the animals are moving. Frames are scored as less or more severe at lower and higher movements, respectively.
+    Computes the "severity" of classification bout events based on how much
+    the animals are moving within the bout. Bouts are scored as less or more severe at lower and higher movements, respectively.
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
 
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
 
     Examples
     ----------
     >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}
-    >>> processor = SeverityCalculator(config_path='project_folder/project_config.ini', settings=settings)
+    >>> processor = SeverityBoutCalculator(config_path='project_folder/project_config.ini', settings=settings)
     >>> processor.run()
     >>> processor.save()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  settings: Dict):
 
         ConfigReader.__init__(self, config_path=config_path)
         self.settings = settings
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg=f'SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty')
         save_name = os.path.join(f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
+        definitions_save_name = os.path.join(f'severity_bin_definitions_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv')
         self.save_path = os.path.join(self.logs_path, save_name)
+        self.definitions_path = os.path.join(self.logs_path, definitions_save_name)
         self.results = {}
 
+    @staticmethod
+    @jit(nopython=True)
+    def __movement_rolling_windows_agg(data: np.ndarray, fps: int):
+        results = np.full((40), np.nan)
+        for window_size_s in range(1, 41):
+            window_width = int(fps * window_size_s)
+            window_movement = np.full((data.shape[0]), np.nan)
+            for i in range(window_width, data.shape[0]):
+                window_movement[i] = np.sum(data[i-window_width:i])
+            results[window_size_s-1] = np.nanmean(window_movement)
+        return results
 
     def __calculate_movements(self):
         self.movements = {}
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
             print(f'Analyzing movements in {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})...')
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
@@ -58,100 +71,80 @@
                 continue
             video_movement = np.full((len(df)), 0)
             for animal_name, animal_bodyparts in self.animal_bp_dict.items():
                 animal_df = df[animal_bodyparts['X_bps'] + animal_bodyparts['Y_bps']]
                 animal_df = self.create_shifted_df(df=animal_df)
                 for (bp_x, bp_y) in zip(animal_bodyparts['X_bps'], animal_bodyparts['Y_bps']):
                     video_movement = np.add(video_movement, self.euclidean_distance(animal_df[bp_x].values, animal_df[f'{bp_x}_shifted'].values, animal_df[bp_y].values, animal_df[f'{bp_y}_shifted'].values, px_per_mm))
-            self.movements[video_name] = video_movement.astype(np.int)
+            self.__movement_rolling_windows_agg(data=video_movement, fps=fps)
 
 
-    def run(self):
-        self.__calculate_movements()
-        video_bins_info = {}
-        movements_cuts = {}
-        print('Finding bracket cut off points...')
-        if self.settings['normalization'] == 'ALL VIDEOS':
-            m = []
-            [m.extend((d.tolist())) for d in self.movements.values()]
-            _, bins = pd.qcut(x=m, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-            for video_name, video_movements in self.movements.items():
-                video_bins_info[video_name] = bins
-                data, _ = pd.cut(x=video_movements, bins=bins, labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-                movements_cuts[video_name] = np.hstack((video_movements.reshape(-1, 1), data.astype(np.int8).reshape(-1, 1)))
-        else:
-            for video_name, video_movements in self.movements.items():
-                data, bins = pd.qcut(x=video_movements, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
-                movements_cuts[video_name] = np.hstack((video_movements.reshape(-1, 1), data.astype(np.int8).reshape(-1, 1)))
-                video_bins_info[video_name] = bins
-        for file_cnt, file_path in enumerate(self.machine_results_paths):
-            _, video_name, _ = get_fn_ext(file_path)
-            self.results[video_name] = {}
-            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type)
-            df = pd.concat([df, pd.DataFrame(movements_cuts[video_name], columns=['MOVEMENT', 'BIN'])], axis=1)
-            clf_df = df['BIN'][df[self.settings['clf']] == 1].astype(int).reset_index(drop=True)
-            for i in range(0, self.settings['brackets']):
-                if self.settings['frames']:
-                    self.results[video_name][f'Grade {str(i + 1)} (frames)'] = len(clf_df[clf_df == i])
-                if self.settings['time']:
-                    self.results[video_name][f'Grade {str(i + 1)} (s)'] = round((len(clf_df[clf_df == i])/ fps), 4)
-
-
-
-            #bin_info = p[1]
-            #print(bins)
-
-            #bins = p.Categories
-
-
-
-            #print(m)
+            #self.movements[video_name] = video_movement.astype(np.int)
 
 
-
-
-
-    #
-    #
-    #
+    def run(self):
+        self.__calculate_movements()
+    #     self.video_bins_info = {}
+    #     movements_cuts = {}
+    #     print('Finding bracket cut off points...')
+    #     if self.settings['normalization'] == 'ALL VIDEOS':
+    #         m = []
+    #         [m.extend((d.tolist())) for d in self.movements.values()]
+    #         _, bins = pd.qcut(x=m, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
+    #         for video_name, video_movements in self.movements.items():
+    #             self.video_bins_info[video_name] = bins.astype(int)
+    #             data, _ = pd.cut(x=video_movements, bins=bins, labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
+    #             movements_cuts[video_name] = np.hstack((video_movements.reshape(-1, 1), data.astype(np.int8).reshape(-1, 1)))
+    #     else:
+    #         for video_name, video_movements in self.movements.items():
+    #             data, bins = pd.qcut(x=video_movements, q=self.settings['brackets'], labels=list(range(1, self.settings['brackets'] + 1)), retbins=True)
+    #             movements_cuts[video_name] = np.hstack((video_movements.reshape(-1, 1), data.astype(np.int8).reshape(-1, 1)))
+    #             self.video_bins_info[video_name] = bins.astype(int)
+    #
+    #     for file_cnt, file_path in enumerate(self.machine_results_paths):
+    #         _, video_name, _ = get_fn_ext(file_path)
+    #         print(f'Matching brackets to movements in video {video_name} ({file_cnt+1}/{len(self.machine_results_paths)}...')
     #         self.results[video_name] = {}
-    #
-    #
-    #         _, _, fps = self.read_video_info(video_name=video_name)
-    #         for animal_name, animal_bodyparts in self.animal_bp_dict.items():
-    #             animal_df = df[animal_bodyparts['X_bps'] + animal_bodyparts['Y_bps']]
-    #             shifted = animal_df.shift(periods=1).fillna(0)
-    #             movement = pd.DataFrame()
-    #             for (bp_x, bp_y) in zip(animal_bodyparts['X_bps'], animal_bodyparts['Y_bps']):
-    #                 movement[bp_x.rstrip('_x')] = self.__euclidean_distance(animal_df[bp_x].values, shifted[bp_x].values, animal_df[bp_y].values, shifted[bp_y].values)
-    #             movement['sum'] = movement.sum(axis=1)
-    #             movement['sum'].iloc[0] = 0
-    #             df[animal_name] = movement['sum']
-    #         df['movement'] = df[self.settings['animals']].sum(axis=1)
-    #         df['bin'] = pd.qcut(x=df['movement'], q=self.settings['brackets'], labels=list(range(1, self.settings['brackets']+1)))
-    #         clf_df = df['bin'][df[self.settings['clf']] == 1].astype(int).reset_index(drop=True)
+    #         _, px_per_mm, fps = self.read_video_info(video_name=video_name)
+    #         df = read_df(file_path=file_path, file_type=self.file_type)
+    #         df = pd.concat([df, pd.DataFrame(movements_cuts[video_name], columns=['MOVEMENT', 'BIN'])], axis=1)
+    #         clf_df = df['BIN'][df[self.settings['clf']] == 1].astype(int).reset_index(drop=True)
     #         for i in range(0, self.settings['brackets']):
     #             if self.settings['frames']:
     #                 self.results[video_name][f'Grade {str(i + 1)} (frames)'] = len(clf_df[clf_df == i])
     #             if self.settings['time']:
     #                 self.results[video_name][f'Grade {str(i + 1)} (s)'] = round((len(clf_df[clf_df == i])/ fps), 4)
     #
     # def save(self):
+    #     print('Saving data..')
     #     out_df = pd.DataFrame(columns=['VIDEO', 'MEASUREMENT', 'VALUE'])
     #     for video_name, video_data in self.results.items():
     #         for grade, grade_data in video_data.items():
     #             out_df.loc[len(out_df)] = [video_name, grade, grade_data]
     #     out_df.to_csv(self.save_path)
     #     self.timer.stop_timer()
     #     stdout_success(msg=f'Severity data saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
     #
+    #
+    #     if self.settings['save_bin_definitions']:
+    #         brackets_data_cols = ['VIDEO']
+    #         for i in range(0, self.settings['brackets']):
+    #             brackets_data_cols.append(f'GRADE {i+1} START'); brackets_data_cols.append(f'GRADE {i + 1} STOP')
+    #         brackets_df = pd.DataFrame(columns=brackets_data_cols)
+    #         for video_name, video_bins in self.video_bins_info.items():
+    #             video_info = [video_name]
+    #             for i in range(len(video_bins)-1):
+    #                 video_info.extend((video_bins[i], video_bins[i+1]))
+    #             brackets_df.loc[len(brackets_df)] = video_info
+    #         brackets_df.to_csv(self.definitions_path)
+    #         stdout_success(msg=f'Severity brackets definitions saved at {self.definitions_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # settings = {'brackets': 10,
 #             'clf': 'Attack',
 #             'animals': ['Simon', 'JJ'],
 #             'normalization': 'ALL VIDEOS', #BY VIDEO
 #             'time': True,
-#             'frames': True}
-# processor = SeverityCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
+#             'frames': True,
+#             'save_bin_definitions': True}
+# processor = SeverityBoutCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
 # processor.run()
-# # processor.save()
+# processor.save()
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolation_smoothing.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,27 @@
 from simba.utils.checks import check_if_filepath_list_is_empty
 from simba.utils.enums import Methods
 from simba.utils.errors import NoFilesFoundError
 
 
 class Interpolate(ConfigReader):
     """
-    Interpolate missing body-parts in pose-estimation data. "Missing" is defined as either (i) when a single body-parts is None or
+    Interpolate missing body-parts in pose-estimation data. "Missing" is defined as either (i) when a single body-parts is None, or
     when all body-parts belonging to an animal are identical (i.e., the same 2D coordinate or all None).
 
-    :parameter str input_path path to pose-estimation data in CSV or parquet format
+    :parameter str input_path: path to pose-estimation data in CSV or parquet format
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter Literal str: Type of interpolation. OPTIONS: 'Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic']
-                            See `tutorial for info/images of the different interpolation types <<https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`>__.
+                            See `tutorial for info/images of the different interpolation types <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
     :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
 
+    .. image:: _static/img/Interpolation_comparison.png
+       :width: 400
+       :align: center
+
     .. note::
        `Interpolation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
 
     Examples
     -----
     >>> _ = Interpolate(input_path=data_path, config_path=SimBaProjectConfigPath, Method='Animal(s): Nearest')
     """
@@ -66,14 +70,15 @@
 
     def animal_interpolator(self):
         for file_path in self.files_found:
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
+            df[df < 0] = 0
             if self.initial_import_multi_index:
                 df.columns = self.bp_col_names
             for animal_name, animal_bps in self.animal_bp_dict.items():
                 animal_df = df[animal_bps['X_bps'] + animal_bps['Y_bps']].fillna(0).astype(int)
                 idx = list(animal_df[animal_df.eq(animal_df.iloc[:, 0], axis=0).all(axis='columns')].index)
                 animal_df.loc[idx, :] = np.nan
                 animal_df = animal_df.interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
@@ -91,17 +96,18 @@
     def body_part_interpolator(self):
         for file_path in self.files_found:
             video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=True)
             if self.initial_import_multi_index:
                 df.columns = self.bp_col_names
+            df[df < 0] = 0
             for animal in self.animal_bp_dict:
                 for x_bps_name, y_bps_name in zip(self.animal_bp_dict[animal]['X_bps'], self.animal_bp_dict[animal]['Y_bps']):
-                    idx = (df[(df[x_bps_name] == 0) & (df[y_bps_name] == 0)].index.tolist())
+                    idx = (df[(df[x_bps_name] <= 0) & (df[y_bps_name] <= 0)].index.tolist())
                     df.loc[idx, [x_bps_name, y_bps_name]] = np.nan
                     df[x_bps_name] = df[x_bps_name].interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
                     df[y_bps_name] = df[y_bps_name].interpolate(method=self.interpolation_method, axis=0).ffill().bfill()
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
@@ -111,17 +117,17 @@
             video_timer.stop_timer()
             print(f'Video {video_name} interpolated (elapsed time {video_timer.elapsed_time_str}) ...')
 
 class Smooth(ConfigReader):
     """
     Smooth pose-estimation data according to user-defined method.
 
-    :parameter str input_path path to pose-estimation data in CSV or parquet format
+    :parameter str input_path: path to pose-estimation data in CSV or parquet format
     :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter Literal str: Type of smoothing_method. OPTIONS: '`Gaussian'`, '`Savitzky-Golay`'.
+    :parameter Literal str: Type of smoothing_method. OPTIONS: ``Gaussian``, ``Savitzky-Golay``.
     :parameter int time_window: Rolling time window in millisecond to use when smoothing. Larger time-windows and greater smoothing.
     :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
 
     .. note::
         `Smoothing tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
 
     Examples
@@ -165,14 +171,15 @@
                 raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing smoothing. To perform smoothing, SimBA needs the video in order to read the video FPS.')
             video_meta_data = get_video_meta_data(video_path=video_path)
             frames_in_time_window = int(self.time_window / (1000 / video_meta_data['fps']))
             if (frames_in_time_window % 2) == 0:
                 frames_in_time_window = frames_in_time_window - 1
             if (frames_in_time_window % 2) <= 3:
                 frames_in_time_window = 5
+            df[df < 0] = 0
             for c in df.columns:
                 df[c] = savgol_filter(x=df[c].to_numpy(), window_length=frames_in_time_window, polyorder=3, mode='nearest')
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
@@ -187,32 +194,44 @@
             _, video_name, _ = get_fn_ext(filepath=file_path)
             df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=self.initial_import_multi_index)
             video_path = find_video_of_file(video_dir=self.video_dir, filename=video_name)
             if not video_path:
                 raise NoFilesFoundError(msg=f'No video for file {video_name} found in SimBA project. Import the video before doing Gaussian smoothing. To perform smoothing, SimBA needs the video in order to read the video FPS.')
             video_meta_data = get_video_meta_data(video_path=video_path)
             frames_in_time_window = int(self.time_window / (1000 / video_meta_data['fps']))
+            df[df < 0] = 0
             for c in df.columns:
                 df[c] = df[c].rolling(window=int(frames_in_time_window), win_type='gaussian', center=True).mean(std=5).fillna(df[c]).abs()
             if not self.initial_import_multi_index:
                 shutil.move(src=file_path, dst=os.path.join(self.save_dir, os.path.basename(file_path)))
             else:
                 multi_idx_header = []
                 for i in range(len(df.columns)): multi_idx_header.append(('IMPORTED_POSE', 'IMPORTED_POSE', list(df.columns)[i]))
                 df.columns = pd.MultiIndex.from_tuples(multi_idx_header)
             write_df(df=df, file_type=self.file_type, save_path=file_path, multi_idx_header=self.initial_import_multi_index)
             video_timer.stop_timer()
             print(f'Video {video_name} smoothed (Gaussian: {str(self.time_window)}ms) (elapsed time {video_timer.elapsed_time_str})...')
 
 
-
-# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/csv/input_csv',
-#             config_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/project_config.ini',
-#             method='Animal(s):Quadratic',
-#             initial_import_multi_index=True)
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/outlier_corrected_movement_location',
+#             config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#             method='Body-parts: Nearest',
+#             initial_import_multi_index=False)
+
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/csv/outlier_corrected_movement_location',
+#             config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini',
+#             method='Body-parts: Nearest',
+#             initial_import_multi_index=False)
+# #
+#
+
+# Interpolate(input_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/csv/outlier_corrected_movement_location',
+#             config_path='/Users/simon/Desktop/envs/troubleshooting/sleap_5_animals/project_folder/project_config.ini',
+#             method='Body-parts: Nearest',
+#             initial_import_multi_index=False)
 
 # PostHocInterpolate(config_path='/Users/simon/Desktop/envs/troubleshooting/ddddfff/project_folder/project_config.ini',
 #                    input_dir='/Users/simon/Desktop/envs/troubleshooting/ddddfff/project_folder/csv/outlier_corrected_movement_location',
 #                    method='Animal(s): Nearest')
 
 
 # Smooth(config_path='/Users/simon/Desktop/envs/troubleshooting/DLC_2_Black_animals/project_folder/project_config.ini',
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/fsttc_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,19 @@
     """
     Compute forward spike-time tiling coefficients between pairs of
     classified behaviors.
 
     :parameter str config_path: path to SimBA project config file in Configparser format
     :parameter int time_window: FSTTC hyperparameter; Integer representing the time window in seconds.
     :parameter List[str] behavior_lst: Behaviors to calculate FSTTC between. FSTTC will be computed for all combinations of behaviors.
-    :parameter bool create_graphs: If True, created violin plots representing each FSTTC. Default: False.
+    :parameter bool create_graphs: If True, created violin plots (as below) representing each FSTTC. Default: False.
+
+    .. image:: _static/img/fsttc_violin.png
+       :width: 500
+       :align: center
 
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/FSTTC.md>`__.
 
     Examples
     -----
     >>> fsttc_calculator = FSTTCCalculator(config_path='MyConfigPath', time_window=2, behavior_lst=['Attack', 'Sniffing'], create_graphs=True)
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/kleinberg_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     :parameter str config_path: path to SimBA project config file in Configparser format
     :parameter List[str] classifier_names: Classifier names to apply Kleinberg smoothing to.
     :parameter float sigma: Burst detection sigma value. Higher sigma values and fewer, longer, behavioural bursts will be recognised. Default: 2.
     :parameter float gamma: Burst detection gamma value. Higher gamma values and fewer behavioural bursts will be recognised. Default: 0.3.
     :parameter int hierarchy: Burst detection hierarchy level. Higher hierarchy values and fewer behavioural bursts will to be recognised. Default: 1.
     :parameter bool hierarchical_search: See `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md#hierarchical-search-example>`_ Default: False.
 
+
+
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md>`__.
 
     Examples
     ----------
     >>> kleinberg_calculator = KleinbergCalculator(config_path='MySimBAConfigPath', classifier_names=['Attack'], sigma=2, gamma=0.3, hierarchy=2, hierarchical_search=False)
     >>> kleinberg_calculator.run()
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/data_processors/movement_calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,33 @@
 
 class MovementCalculator(ConfigReader,
                          FeatureExtractionMixin):
     """
     Compute aggregate movement statistics from pose-estimation data in SimBA project.
 
     :parameters str config_path: path to SimBA project config file in Configparser format
+    :param List[str] body_parts: Body-parts to use for movement calculations OR ``Animal_name CENTER OF GRAVITY``. If ``Animal_name CENTER OF GRAVITY``, then SimBA will approximate animal centroids through convex hull.
+    :param float threshold: Filter body-part detection below set threshold (Value 0-1). Default: 0.00
+    :param List[str] or None file_paths: Files to calucalte movements for. If None, then all files in ``project_folder/csv/outlier_corrected_movement_location`` directory.
 
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
-    Examples
-    ----------
-    >>> movement_processor = MovementCalculator(config_path='project_folder/project_config.ini')
+    :examples:
+    >>> body_parts=['Animal_1 CENTER OF GRAVITY']
+    >>> movement_processor = MovementCalculator(config_path='project_folder/project_config.ini', body_parts=body_parts)
     >>> movement_processor.run()
     >>> movement_processor.save()
 
     """
 
     def __init__(self,
                  config_path: str,
                  body_parts: List[str],
-                 threshold: float,
+                 threshold: float = 0.00,
                  file_paths: Optional[List[str]] = None):
 
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self)
         self.save_path = os.path.join(self.logs_path, 'Movement_log_{}.csv'.format(self.datetime))
         self.file_paths, self.body_parts, self.threshold = file_paths, body_parts, threshold
         if not self.file_paths:
@@ -58,24 +61,14 @@
                 pass
 
     def __find_polygons(self, data):
         print(data.shape)
 
 
     def run(self):
-        """
-        Method to run movement aggregation computations.
-
-        Returns
-        ----------
-        Attribute: dict
-            results
-
-        """
-
         self.results = pd.DataFrame(columns=['VIDEO', 'ANIMAL', 'BODY-PART', "MEASURE", 'VALUE'])
         self.movement_dfs = {}
         for file_path in self.file_paths:
             self.__find_body_part_columns()
             _, video_name, _ = get_fn_ext(file_path)
             print('Analysing {}...'.format(video_name))
             self.data_df = read_df(file_path=file_path, file_type=self.file_type)
```

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.59.8/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.59.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.59.8/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.59.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.59.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.59.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.59.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.59.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.59.8/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.59.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.59.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.59.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.59.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.59.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.59.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.59.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.59.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.59.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.59.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.59.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.7
+Version: 1.59.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,17 @@
 simba/data_processors/fsttc_calculator.py
 simba/data_processors/interpolate_pose.py
 simba/data_processors/interpolation_smoothing.py
 simba/data_processors/kleinberg_calculator.py
 simba/data_processors/movement_calculator.py
 simba/data_processors/pup_retrieval_calculator.py
 simba/data_processors/pybursts_calculator.py
+simba/data_processors/severity_bout_based_calculator.py
 simba/data_processors/severity_calculator.py
-simba/data_processors/severity_calculator_2.py
+simba/data_processors/severity_frame_based_calculator.py
 simba/data_processors/timebins_clf_calculator.py
 simba/data_processors/timebins_movement_calculator.py
 simba/feature_extractors/.DS_Store
 simba/feature_extractors/__init__.py
 simba/feature_extractors/feature_extractor_14bp.py
 simba/feature_extractors/feature_extractor_16bp.py
 simba/feature_extractors/feature_extractor_4bp.py
```

### Comparing `Simba-UW-tf-dev-1.59.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.59.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/LICENSE.md` & `Simba-UW-tf-dev-1.59.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/README.md` & `Simba-UW-tf-dev-1.59.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.7/setup.py` & `Simba-UW-tf-dev-1.59.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.59.7",
+    version="1.59.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

