# Comparing `tmp/Simba-UW-tf-dev-1.59.9.tar.gz` & `tmp/Simba-UW-tf-dev-1.60.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.59.9.tar", last modified: Fri May 19 18:36:44 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.1.tar", last modified: Fri May 19 21:16:11 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.59.9.tar` & `Simba-UW-tf-dev-1.60.1.tar`

### file list

```diff
@@ -1,503 +1,504 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.59.9/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15019 2023-05-19 18:30:31.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.59.9/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.9/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.59.9/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.59.9/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.59.9/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-18 22:17:21.000000 Simba-UW-tf-dev-1.59.9/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30677 2023-04-27 01:57:28.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-25 21:03:39.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3696 2023-05-18 20:58:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.59.9/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51865 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61153 2023-05-18 13:21:56.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.59.9/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.59.9/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.59.9/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.59.9/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.9/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.59.9/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    41533 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.59.9/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.59.9/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.59.9/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.59.9/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.59.9/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.59.9/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.59.9/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15608 2023-05-19 15:09:35.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.59.9/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.59.9/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.59.9/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.59.9/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.59.9/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.59.9/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.59.9/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.59.9/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.59.9/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.59.9/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.59.9/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19547 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-19 18:36:43.000000 Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.59.9/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.59.9/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.59.9/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-19 18:36:30.000000 Simba-UW-tf-dev-1.59.9/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-19 18:36:44.000000 Simba-UW-tf-dev-1.59.9/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.60.1/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15019 2023-05-19 18:30:31.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.60.1/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.1/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.1/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.60.1/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.1/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.60.1/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51865 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.1/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.1/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.60.1/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.1/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.1/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    41533 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.1/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.1/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.1/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.1/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.60.1/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.1/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15608 2023-05-19 15:09:35.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.1/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.1/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.1/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.1/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.1/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19618 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.1/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.1/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.1/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-19 21:16:04.000000 Simba-UW-tf-dev-1.60.1/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.59.9/PKG-INFO` & `Simba-UW-tf-dev-1.60.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.9
+Version: 1.60.1
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.60.1/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.60.1/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.60.1/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -1478,26 +1478,26 @@
 00005c50: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 00005c60: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00005c70: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00005c80: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00005c90: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00005ca0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00005cb0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00005cc0: 7208 0809 0809 5f10 187b 7b31 3132 2c20  r....._..{{112, 
-00005cd0: 3535 7d2c 207b 3131 3939 2c20 3736 397d  55}, {1199, 769}
+00005cc0: 7208 0809 0809 5f10 187b 7b33 3335 2c20  r....._..{{335, 
+00005cd0: 3139 387d 2c20 7b39 3237 2c20 3536 387d  198}, {927, 568}
 00005ce0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
 00005cf0: 9900 0000 0000 0001 0100 0000 0000 0000  ................
 00005d00: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 9a00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00005d20: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00005d30: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00005d40: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00005d50: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d60: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d70: 6d70 0000 0000 0015 6160 5863 6f6d 6d65  mp......a`Xcomme
+00005d70: 6d70 0000 0000 0015 61e0 5863 6f6d 6d65  mp......a.Xcomme
 00005d80: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
 00005d90: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
 00005da0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
 00005db0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
 00005dc0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
 00005dd0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
 00005de0: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
@@ -1579,19 +1579,19 @@
 000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
 000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
 000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00006310: 0834 1195 81d7 08c5 4100 0000 1200 6600  .4......A.....f.
+00006310: 086f ba2a 3a04 0cc5 4100 0000 1200 6600  .o.*:...A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 083d 8fc4  smodDblob....=..
-00006350: 12f3 05c5 4100 0000 1200 6600 6500 6100  ....A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 086f ba2a  smodDblob....o.*
+00006350: 3a04 0cc5 4100 0000 1200 6600 6500 6100  :...A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
 00006380: 5363 6f6d 7000 0000 0000 1820 0000 0000  Scomp...... ....
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
```

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from __future__ import division
 import numpy as np
 import math
 import pandas as pd
-from simba.read_config_unit_tests import (read_project_path_and_file_type,
+from simba.utils.read_write import (read_project_path_and_file_type,
                                           check_if_filepath_list_is_empty)
 from scipy import stats
 from statsmodels.stats.diagnostic import lilliefors
 from scipy.signal import find_peaks
 from scipy.spatial import ConvexHull
 from scipy.spatial.qhull import QhullError
 from scipy.stats import zscore
 from numba import jit, prange
 import os, glob
-from simba.enums import Paths
+from simba.utils.enums import Paths
 from simba.utils.read_write import get_fn_ext, read_video_info, read_config_file, write_df, read_df
 from simba.utils.printing import SimbaTimer
 from itertools import combinations
 from joblib import Parallel, delayed
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 
-TAIL_BP_NAMES = ['objectA', 'peduncle_base']
-CENTER_BP_NAMES = ['midpoint']
-MOUTH = ['mouth']
+TAIL_BP_NAMES = ['tail']
+CENTER_BP_NAMES = ['trunk1']
+MOUTH = ['head']
 
 ANGULAR_DISPERSION_S = [10, 5, 2, 1, 0.5, 0.25]
 
 class FishFeatureExtractor(ConfigReader, FeatureExtractionMixin):
     def __init__(self,
                  config_path: str):
+
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self, config_path=config_path)
         self.timer = SimbaTimer()
         self.timer.start_timer()
         self.compass_brackets = ["N", "NE", "E", "SE", "S", "SW", "W", "NW", "N"]
         self.compass_brackets_long = ["Direction_N", "Direction_NE", "Direction_E", "Direction_SE", "Direction_S", "Direction_SW", "Direction_W", "Direction_NW"]
         self.compass_brackets_digits = ["0", "1", "2", "3", "4", "5", "6", "7", "0"]
@@ -56,27 +57,27 @@
 
         self.roll_windows_values = [75, 50, 25, 20, 15, 10, 4, 2, ]
         self.files_found = glob.glob(self.input_file_dir + '/*.{}'.format(self.file_type))
         check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg='SIMBA ERROR: No file in {} directory'.format(self.input_file_dir))
         print('Extracting features from {} {}...'.format(str(len(self.files_found)), 'file(s)'))
 
         for file_path in self.files_found:
-            video_timer = SimbaTimer()
+            video_timer = SimbaTimer(start=True)
             video_timer.start_timer()
             dir_name, file_name, ext = get_fn_ext(file_path)
             self.save_path = os.path.join(self.save_dir, os.path.basename(file_path))
             video_info, self.px_per_mm, self.fps = read_video_info(self.video_info_df, file_name)
             self.video_width, self.video_height = video_info['Resolution_width'].values, video_info['Resolution_height'].values
             self.angular_dispersion_windows = []
             for i in range(len(ANGULAR_DISPERSION_S)):
                 self.angular_dispersion_windows.append(int(self.fps * ANGULAR_DISPERSION_S[i]))
 
             self.csv_df = read_df(file_path, self.file_type).fillna(0).apply(pd.to_numeric)
             try:
-                self.csv_df.columns = self.bp_col_names
+                self.csv_df.columns = self.bp_headers
             except ValueError:
                 msg = f'ERROR: Data contains the following fields: {self.csv_df.columns}. \n SimBA wants to use the following field names {self.bp_header_list}'
                 print(msg)
                 raise ValueError(msg)
 
             csv_df_shifted = self.csv_df.shift(periods=1)
             csv_df_shifted.columns = self.col_headers_shifted
@@ -198,16 +199,14 @@
 
         columns = [f'{feature_name}_KS', f'{feature_name}_TTEST', f'{feature_name}_LILLEFORS',
                    f'{feature_name}_SHAPIRO', f'{feature_name}_PEAK_CNT']
         return pd.DataFrame(
             np.column_stack((ks_results, t_test_results, lillefors_results, shapiro_results, peak_cnt_results)),
             columns=columns).round(4)
 
-
-
     @staticmethod
     @jit(nopython=True)
     def consecutive_frames_in_same_compass_direction(direction: np.array):
         results = np.full((direction.shape[0], 1), -1)
         cnt, results[0], last_direction = 0, 0, direction[0]
         for i in prange(1, direction.shape[0]):
             if direction[i] == last_direction:
```

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -276,138 +276,138 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 000b dbb7 0000 000b 005f 005f 0070  ..........._._.p
+000011a0: 0000 000e 1fa4 0000 000b 005f 005f 0070  ..........._._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 47b4 5787  moDDblob....G.W.
-000011d0: 2cfc c441 0000 000b 005f 005f 0070 0079  ,..A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 2360 98ff  moDDblob....#`..
+000011d0: 040c c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-000011f0: 6444 626c 6f62 0000 0008 9edb 857b 6efb  dDblob.......{n.
-00001200: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000011f0: 6444 626c 6f62 0000 0008 2360 98ff 040c  dDblob....#`....
+00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-00001220: 636f 6d70 0000 0000 000c 8000 0000 000b  comp............
+00001220: 636f 6d70 0000 0000 000f 1000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
-00001260: 7370 626c 6f62 0000 00c8 6270 6c69 7374  spblob....bplist
+00001260: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000012a0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 000012b0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 000012c0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000012e0: 6261 7208 0809 0809 5f10 177b 7b33 342c  bar....._..{{34,
-000012f0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
-00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
-00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00001330: 0099 0000 0004 006d 0069 0073 0063 6473  .......m.i.s.cds
-00001340: 636c 626f 6f6c 0000 0000 0400 6d00 6900  clbool......m.i.
-00001350: 7300 636c 6731 5363 6f6d 7000 0000 0000  s.clg1Scomp.....
-00001360: 0306 2e00 0000 0400 6d00 6900 7300 636c  ........m.i.s.cl
-00001370: 7376 4362 6c6f 6200 0002 b862 706c 6973  svCblob....bplis
-00001380: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
-00001390: 0d18 4849 484a 0c4c 5869 636f 6e53 697a  ..HIHJ.LXiconSiz
-000013a0: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
-000013b0: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-000013c0: 6c63 756c 6174 6541 6c6c 5369 7a65 735f  lculateAllSizes_
-000013d0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-000013e0: 5958 7465 7874 5369 7a65 5f10 0f73 6372  YXtextSize_..scr
-000013f0: 6f6c 6c50 6f73 6974 696f 6e58 5a73 6f72  ollPositionXZsor
-00001400: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-00001410: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
-00001420: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
-00001430: 4030 0000 0000 0000 09ab 0e17 1c21 252a  @0...........!%*
-00001440: 2f34 393e 43d4 0f10 1112 1314 0c0c 5a69  /49>C.........Zi
-00001450: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
-00001460: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00001470: 6554 6e61 6d65 1101 a609 09d4 1210 110f  eTname..........
-00001480: 1819 181b 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00001490: 79d4 1210 110f 0c1e 1820 0910 b508 5c64  y........ ....\d
-000014a0: 6174 654d 6f64 6966 6965 64d4 1210 110f  ateModified.....
-000014b0: 181e 1824 0808 5b64 6174 6543 7265 6174  ...$..[dateCreat
-000014c0: 6564 d412 1011 0f0c 2718 2909 1061 0854  ed......'.)..a.T
-000014d0: 7369 7a65 d412 1011 0f0c 2c0c 2e09 1073  size......,....s
-000014e0: 0954 6b69 6e64 d412 1011 0f18 310c 3308  .Tkind......1.3.
-000014f0: 1064 0955 6c61 6265 6cd4 1210 110f 1836  .d.Ulabel......6
-00001500: 0c38 0810 4b09 5776 6572 7369 6f6e d412  .8..K.Wversion..
-00001510: 1011 0f18 3b0c 3d08 1101 2c09 5863 6f6d  ....;.=...,.Xcom
-00001520: 6d65 6e74 73d4 1210 110f 1840 1842 0810  ments......@.B..
-00001530: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00001540: 64d4 1210 110f 181e 1846 0808 5964 6174  d........F..Ydat
-00001550: 6541 6464 6564 0823 0000 0000 0000 0000  eAdded.#........
-00001560: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
-00001570: 6469 6669 6564 0910 0100 0800 1d00 2600  dified........&.
-00001580: 3800 4000 5400 6600 6f00 8100 8c00 9f00  8.@.T.f.o.......
-00001590: b400 bd00 be00 ca00 d300 de00 e400 ee00  ................
-000015a0: f600 fb00 fe00 ff01 0001 0901 0a01 0c01  ................
-000015b0: 0d01 1601 1f01 2001 2201 2301 3001 3901  ...... .".#.0.9.
-000015c0: 3a01 3b01 4701 5001 5101 5301 5401 5901  :.;.G.P.Q.S.T.Y.
-000015d0: 6201 6301 6501 6601 6b01 7401 7501 7701  b.c.e.f.k.t.u.w.
-000015e0: 7801 7e01 8701 8801 8a01 8b01 9301 9c01  x.~.............
-000015f0: 9d01 a001 a101 aa01 b301 b401 b601 b701  ................
-00001600: c601 cf01 d001 d101 db01 dc01 e501 ee01  ................
-00001610: fb01 fc00 0000 0000 0002 0100 0000 0000  ................
-00001620: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-00001630: 0001 fe00 0000 0400 6d00 6900 7300 636c  ........m.i.s.cl
-00001640: 7376 7062 6c6f 6200 0002 9d62 706c 6973  svpblob....bplis
-00001650: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
-00001660: 0d1f 4849 484a 0c26 5869 636f 6e53 697a  ..HIHJ.&XiconSiz
-00001670: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
-00001680: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00001690: 6c63 756c 6174 6541 6c6c 5369 7a65 735f  lculateAllSizes_
-000016a0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-000016b0: 5958 7465 7874 5369 7a65 5f10 0f73 6372  YXtextSize_..scr
-000016c0: 6f6c 6c50 6f73 6974 696f 6e58 5a73 6f72  ollPositionXZsor
-000016d0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-000016e0: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
-000016f0: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
-00001700: 4030 0000 0000 0000 09d9 0e0f 1011 1213  @0..............
-00001710: 1415 1617 2025 2a2e 3338 3d42 5863 6f6d  .... %*.38=BXcom
-00001720: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
-00001730: 656e 6564 5c64 6174 654d 6f64 6966 6965  ened\dateModifie
-00001740: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
-00001750: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
-00001760: 7273 696f 6e54 6e61 6d65 d418 191a 1b1c  rsionTname......
-00001770: 1d0c 1f55 696e 6465 7855 7769 6474 6859  ...UindexUwidthY
-00001780: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00001790: 6510 0711 012c 0908 d418 191a 1b21 221f  e....,.......!".
-000017a0: 1f10 0810 c808 08d4 1819 1a1b 2627 1f0c  ............&'..
-000017b0: 1001 10b5 0809 d418 191a 1b2b 271f 1f10  ...........+'...
-000017c0: 0208 08d4 1819 1a1b 2f30 1f0c 1003 1061  ......../0.....a
-000017d0: 0809 d418 191a 1b34 350c 1f10 0510 6409  .......45.....d.
-000017e0: 08d4 1819 1a1b 393a 0c0c 1004 1073 0909  ......9:.....s..
-000017f0: d418 191a 1b3e 3f0c 1f10 0610 4b09 08d4  .....>?.....K...
-00001800: 1b19 1a18 0c44 0c46 0911 01a6 0910 0008  .....D.F........
-00001810: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
-00001820: 0000 5c64 6174 654d 6f64 6966 6965 6409  ..\dateModified.
-00001830: 0008 001d 0026 0038 0040 0054 0066 006f  .....&.8.@.T.f.o
-00001840: 0081 008c 009f 00b4 00bd 00be 00d1 00da  ................
-00001850: 00e9 00f6 0102 0107 010d 0112 011a 011f  ................
-00001860: 0128 012e 0134 013e 0146 0148 014b 014c  .(...4.>.F.H.K.L
-00001870: 014d 0156 0158 015a 015b 015c 0165 0167  .M.V.X.Z.[.\.e.g
-00001880: 0169 016a 016b 0174 0176 0177 0178 0181  .i.j.k.t.v.w.x..
-00001890: 0183 0185 0186 0187 0190 0192 0194 0195  ................
-000018a0: 0196 019f 01a1 01a3 01a4 01a5 01ae 01b0  ................
-000018b0: 01b2 01b3 01b4 01bd 01be 01c1 01c2 01c4  ................
-000018c0: 01c5 01ce 01d7 01e4 0000 0000 0000 0201  ................
-000018d0: 0000 0000 0000 004c 0000 0000 0000 0000  .......L........
-000018e0: 0000 0000 0000 01e5 0000 0004 006d 0069  .............m.i
-000018f0: 0073 0063 6d6f 4444 626c 6f62 0000 0008  .s.cmoDDblob....
-00001900: 52c2 c56a fdfa c441 0000 0004 006d 0069  R..j...A.....m.i
-00001910: 0073 0063 6d6f 6444 626c 6f62 0000 0008  .s.cmodDblob....
-00001920: e799 1006 35fa c441 0000 0004 006d 0069  ....5..A.....m.i
-00001930: 0073 0063 7068 3153 636f 6d70 0000 0000  .s.cph1Scomp....
-00001940: 0004 0000 0000 0004 006d 0069 0073 0063  .........m.i.s.c
-00001950: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
+000012e0: 6261 7208 0809 0809 5f10 187b 7b33 3335  bar....._..{{335
+000012f0: 2c20 3139 387d 2c20 7b39 3237 2c20 3536  , 198}, {927, 56
+00001300: 387d 7d09 0817 2531 3d49 606d 797a 7b7c  8}}...%1=I`myz{|
+00001310: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
+00001320: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+00001330: 0000 9a00 0000 0400 6d00 6900 7300 6364  ........m.i.s.cd
+00001340: 7363 6c62 6f6f 6c00 0000 0004 006d 0069  sclbool......m.i
+00001350: 0073 0063 6c67 3153 636f 6d70 0000 0000  .s.clg1Scomp....
+00001360: 0003 616b 0000 0004 006d 0069 0073 0063  ..ak.....m.i.s.c
+00001370: 6c73 7643 626c 6f62 0000 02b8 6270 6c69  lsvCblob....bpli
+00001380: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00001390: 0c0d 1848 4948 4a0c 4c58 6963 6f6e 5369  ...HIHJ.LXiconSi
+000013a0: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+000013b0: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+000013c0: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000013d0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000013e0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000013f0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+00001400: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+00001410: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+00001420: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00001430: 2340 3000 0000 0000 0009 ab0e 171c 2125  #@0...........!%
+00001440: 2a2f 3439 3e43 d40f 1011 1213 140c 0c5a  */49>C.........Z
+00001450: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
+00001460: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00001470: 6c65 546e 616d 6511 01a6 0909 d412 1011  leTname.........
+00001480: 0f18 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
+00001490: 7479 d412 1011 0f0c 1e18 2009 10b5 085c  ty........ ....\
+000014a0: 6461 7465 4d6f 6469 6669 6564 d412 1011  dateModified....
+000014b0: 0f18 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
+000014c0: 7465 64d4 1210 110f 0c27 1829 0910 6108  ted......'.)..a.
+000014d0: 5473 697a 65d4 1210 110f 0c2c 0c2e 0910  Tsize......,....
+000014e0: 7309 546b 696e 64d4 1210 110f 1831 0c33  s.Tkind......1.3
+000014f0: 0810 6409 556c 6162 656c d412 1011 0f18  ..d.Ulabel......
+00001500: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
+00001510: 1210 110f 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
+00001520: 6d6d 656e 7473 d412 1011 0f18 4018 4208  mments......@.B.
+00001530: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+00001540: 6564 d412 1011 0f18 1e18 4608 0859 6461  ed........F..Yda
+00001550: 7465 4164 6465 6408 2300 0000 0000 0000  teAdded.#.......
+00001560: 0023 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
+00001570: 6f64 6966 6965 6409 1001 0008 001d 0026  odified........&
+00001580: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
+00001590: 00b4 00bd 00be 00ca 00d3 00de 00e4 00ee  ................
+000015a0: 00f6 00fb 00fe 00ff 0100 0109 010a 010c  ................
+000015b0: 010d 0116 011f 0120 0122 0123 0130 0139  ....... .".#.0.9
+000015c0: 013a 013b 0147 0150 0151 0153 0154 0159  .:.;.G.P.Q.S.T.Y
+000015d0: 0162 0163 0165 0166 016b 0174 0175 0177  .b.c.e.f.k.t.u.w
+000015e0: 0178 017e 0187 0188 018a 018b 0193 019c  .x.~............
+000015f0: 019d 01a0 01a1 01aa 01b3 01b4 01b6 01b7  ................
+00001600: 01c6 01cf 01d0 01d1 01db 01dc 01e5 01ee  ................
+00001610: 01fb 01fc 0000 0000 0000 0201 0000 0000  ................
+00001620: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+00001630: 0000 01fe 0000 0004 006d 0069 0073 0063  .........m.i.s.c
+00001640: 6c73 7670 626c 6f62 0000 029d 6270 6c69  lsvpblob....bpli
+00001650: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00001660: 0c0d 1f48 4948 4a0c 2658 6963 6f6e 5369  ...HIHJ.&XiconSi
+00001670: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00001680: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001690: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000016a0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000016b0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000016c0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000016d0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000016e0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+000016f0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00001700: 2340 3000 0000 0000 0009 d90e 0f10 1112  #@0.............
+00001710: 1314 1516 1720 252a 2e33 383d 4258 636f  ..... %*.38=BXco
+00001720: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+00001730: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+00001740: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00001750: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00001760: 6572 7369 6f6e 546e 616d 65d4 1819 1a1b  ersionTname.....
+00001770: 1c1d 0c1f 5569 6e64 6578 5577 6964 7468  ....UindexUwidth
+00001780: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00001790: 6c65 1007 1101 2c09 08d4 1819 1a1b 2122  le....,.......!"
+000017a0: 1f1f 1008 10c8 0808 d418 191a 1b26 271f  .............&'.
+000017b0: 0c10 0110 b508 09d4 1819 1a1b 2b27 1f1f  ............+'..
+000017c0: 1002 0808 d418 191a 1b2f 301f 0c10 0310  ........./0.....
+000017d0: 6108 09d4 1819 1a1b 3435 0c1f 1005 1064  a.......45.....d
+000017e0: 0908 d418 191a 1b39 3a0c 0c10 0410 7309  .......9:.....s.
+000017f0: 09d4 1819 1a1b 3e3f 0c1f 1006 104b 0908  ......>?.....K..
+00001800: d41b 191a 180c 440c 4609 1101 a609 1000  ......D.F.......
+00001810: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
+00001820: 0000 005c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00001830: 0900 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
+00001840: 6f00 8100 8c00 9f00 b400 bd00 be00 d100  o...............
+00001850: da00 e900 f601 0201 0701 0d01 1201 1a01  ................
+00001860: 1f01 2801 2e01 3401 3e01 4601 4801 4b01  ..(...4.>.F.H.K.
+00001870: 4c01 4d01 5601 5801 5a01 5b01 5c01 6501  L.M.V.X.Z.[.\.e.
+00001880: 6701 6901 6a01 6b01 7401 7601 7701 7801  g.i.j.k.t.v.w.x.
+00001890: 8101 8301 8501 8601 8701 9001 9201 9401  ................
+000018a0: 9501 9601 9f01 a101 a301 a401 a501 ae01  ................
+000018b0: b001 b201 b301 b401 bd01 be01 c101 c201  ................
+000018c0: c401 c501 ce01 d701 e400 0000 0000 0002  ................
+000018d0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
+000018e0: 0000 0000 0000 0001 e500 0000 0400 6d00  ..............m.
+000018f0: 6900 7300 636d 6f44 4462 6c6f 6200 0000  i.s.cmoDDblob...
+00001900: 080b 77ae c006 0cc5 4100 0000 0400 6d00  ..w.....A.....m.
+00001910: 6900 7300 636d 6f64 4462 6c6f 6200 0000  i.s.cmodDblob...
+00001920: 080b 77ae c006 0cc5 4100 0000 0400 6d00  ..w.....A.....m.
+00001930: 6900 7300 6370 6831 5363 6f6d 7000 0000  i.s.cph1Scomp...
+00001940: 0000 0460 0000 0000 0400 6d00 6900 7300  ...`......m.i.s.
+00001950: 6376 5372 6e6c 6f6e 6700 0000 0100 0000  cvSrnlong.......
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0038 0810 4b09 5776 6572 7369 6f6e d412  .8..K.Wversion..
-00002510: 1011 0f18 3b0c 3d08 1101 2c09 5863 6f6d  ....;.=...,.Xcom
-00002520: 6d65 6e74 73d4 1210 110f 1840 1842 0810  ments......@.B..
-00002530: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-00002540: 64d4 1210 110f 181e 1846 0808 5964 6174  d........F..Ydat
-00002550: 6541 6464 6564 0823 0000 0000 0000 0000  eAdded.#........
-00002560: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
-00002570: 6469 6669 6564 0910 0100 0800 1d00 2600  dified........&.
-00002580: 3800 4000 5400 6600 6f00 8100 8c00 9f00  8.@.T.f.o.......
-00002590: b400 bd00 be00 ca00 d300 de00 e400 ee00  ................
-000025a0: f600 fb00 fe00 ff01 0001 0901 0a01 0c01  ................
-000025b0: 0d01 1601 1f01 2001 2201 2301 3001 3901  ...... .".#.0.9.
-000025c0: 3a01 3b01 4701 5001 5101 5301 5401 5901  :.;.G.P.Q.S.T.Y.
-000025d0: 6201 6301 6501 6601 6b01 7401 7501 7701  b.c.e.f.k.t.u.w.
-000025e0: 7801 7e01 8701 8801 8a01 8b01 9301 9c01  x.~.............
-000025f0: 9d01 a001 a101 aa01 b301 b401 b601 b701  ................
-00002600: c601 cf01 d001 d101 db01 dc01 e501 ee01  ................
-00002610: fb01 fc00 0000 0000 0002 0100 0000 0000  ................
-00002620: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-00002630: 0001 fe00 0000 0400 6d00 6900 7300 636c  ........m.i.s.cl
-00002640: 7376 7062 6c6f 6200 0002 9d62 706c 6973  svpblob....bplis
-00002650: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
-00002660: 0d1f 4849 484a 0c26 5869 636f 6e53 697a  ..HIHJ.&XiconSiz
-00002670: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
-00002680: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00002690: 6c63 756c 6174 6541 6c6c 5369 7a65 735f  lculateAllSizes_
-000026a0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-000026b0: 5958 7465 7874 5369 7a65 5f10 0f73 6372  YXtextSize_..scr
-000026c0: 6f6c 6c50 6f73 6974 696f 6e58 5a73 6f72  ollPositionXZsor
-000026d0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-000026e0: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
-000026f0: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
-00002700: 4030 0000 0000 0000 09d9 0e0f 1011 1213  @0..............
-00002710: 1415 1617 2025 2a2e 3338 3d42 5863 6f6d  .... %*.38=BXcom
-00002720: 6d65 6e74 735e 6461 7465 4c61 7374 4f70  ments^dateLastOp
-00002730: 656e 6564 5c64 6174 654d 6f64 6966 6965  ened\dateModifie
-00002740: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
-00002750: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
-00002760: 7273 696f 6e54 6e61 6d65 d418 191a 1b1c  rsionTname......
-00002770: 1d0c 1f55 696e 6465 7855 7769 6474 6859  ...UindexUwidthY
-00002780: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00002790: 6510 0711 012c 0908 d418 191a 1b21 221f  e....,.......!".
-000027a0: 1f10 0810 c808 08d4 1819 1a1b 2627 1f0c  ............&'..
-000027b0: 1001 10b5 0809 d418 191a 1b2b 271f 1f10  ...........+'...
-000027c0: 0208 08d4 1819 1a1b 2f30 1f0c 1003 1061  ......../0.....a
-000027d0: 0809 d418 191a 1b34 350c 1f10 0510 6409  .......45.....d.
-000027e0: 08d4 1819 1a1b 393a 0c0c 1004 1073 0909  ......9:.....s..
-000027f0: d418 191a 1b3e 3f0c 1f10 0610 4b09 08d4  .....>?.....K...
-00002800: 1b19 1a18                                ....
+00002500: 000c 3808 104b 0957 7665 7273 696f 6ed4  ..8..K.Wversion.
+00002510: 1210 110f 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
+00002520: 6d6d 656e 7473 d412 1011 0f18 4018 4208  mments......@.B.
+00002530: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+00002540: 6564 d412 1011 0f18 1e18 4608 0859 6461  ed........F..Yda
+00002550: 7465 4164 6465 6408 2300 0000 0000 0000  teAdded.#.......
+00002560: 0023 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
+00002570: 6f64 6966 6965 6409 1001 0008 001d 0026  odified........&
+00002580: 0038 0040 0054 0066 006f 0081 008c 009f  .8.@.T.f.o......
+00002590: 00b4 00bd 00be 00ca 00d3 00de 00e4 00ee  ................
+000025a0: 00f6 00fb 00fe 00ff 0100 0109 010a 010c  ................
+000025b0: 010d 0116 011f 0120 0122 0123 0130 0139  ....... .".#.0.9
+000025c0: 013a 013b 0147 0150 0151 0153 0154 0159  .:.;.G.P.Q.S.T.Y
+000025d0: 0162 0163 0165 0166 016b 0174 0175 0177  .b.c.e.f.k.t.u.w
+000025e0: 0178 017e 0187 0188 018a 018b 0193 019c  .x.~............
+000025f0: 019d 01a0 01a1 01aa 01b3 01b4 01b6 01b7  ................
+00002600: 01c6 01cf 01d0 01d1 01db 01dc 01e5 01ee  ................
+00002610: 01fb 01fc 0000 0000 0000 0201 0000 0000  ................
+00002620: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+00002630: 0000 01fe 0000 0004 006d 0069 0073 0063  .........m.i.s.c
+00002640: 6c73 7670 626c 6f62 0000 029d 6270 6c69  lsvpblob....bpli
+00002650: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00002660: 0c0d 1f48 4948 4a0c 2658 6963 6f6e 5369  ...HIHJ.&XiconSi
+00002670: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00002680: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00002690: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+000026a0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000026b0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000026c0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000026d0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000026e0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+000026f0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00002700: 2340 3000 0000 0000 0009 d90e 0f10 1112  #@0.............
+00002710: 1314 1516 1720 252a 2e33 383d 4258 636f  ..... %*.38=BXco
+00002720: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+00002730: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+00002740: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+00002750: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+00002760: 6572 7369 6f6e 546e 616d 65d4 1819 1a1b  ersionTname.....
+00002770: 1c1d 0c1f 5569 6e64 6578 5577 6964 7468  ....UindexUwidth
+00002780: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00002790: 6c65 1007 1101 2c09 08d4 1819 1a1b 2122  le....,.......!"
+000027a0: 1f1f 1008 10c8 0808 d418 191a 1b26 271f  .............&'.
+000027b0: 0c10 0110 b508 09d4 1819 1a1b 2b27 1f1f  ............+'..
+000027c0: 1002 0808 d418 191a 1b2f 301f 0c10 0310  ........./0.....
+000027d0: 6108 09d4 1819 1a1b 3435 0c1f 1005 1064  a.......45.....d
+000027e0: 0908 d418 191a 1b39 3a0c 0c10 0410 7309  .......9:.....s.
+000027f0: 09d4 1819 1a1b 3e3f 0c1f 1006 104b 0908  ......>?.....K..
+00002800: d41b 191a                                ....
```

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/perimeter_jit.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     :param str target: Options [perimeter, area]
     :return: 1d np.array representing perimeter length or area of polygon on each frame
 
     .. note::
     Modified from `Jérôme Richard <https://stackoverflow.com/questions/74812556/computing-quick-convex-hull-using-numba/74817179#74817179>`_
 
     :example:
-    >>> points = np.random.randint(1, 50, size=(50, 5, 2)).astype(float)
+    >>> points = np.random.randint(1, 50, size=(50, 5, 2)).astype(np.float32)
     >>> results = jitted_hull(points, target='area')
     """
 
     def perimeter(xy):
         perimeter = np.linalg.norm(xy[0] - xy[-1])
         for i in prange(xy.shape[0]-1):
             p = np.linalg.norm(xy[i] - xy[i+1])
@@ -86,12 +86,20 @@
         perimeter_points = np.full((len(idx), 2), np.nan)
         for j in prange(len(idx)):
             perimeter_points[j] = points[i][j]
         results[i][0] = np.int(np.mean(perimeter_points[:, 0].flatten()))
         results[i][1] = np.int(np.mean(perimeter_points[:, 1].flatten()))
     return results
 
+# points = np.random.randint(1, 5, size=(1, 10, 2)).astype(np.float32)
+# points[0][1] = np.nan
+# results = jitted_hull(points, target='area')
+# print(results)
+
+
+
+
 # points = np.random.randint(1, 10, size=(50, 5, 2)).astype(np.float32)
 # results = jitted_centroid(points)
 #
 #
 # results = np.full((points.shape[0]), np.nan)
```

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/requirements.txt` & `Simba-UW-tf-dev-1.60.1/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi` & `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/plotting_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import matplotlib
 import shutil
 import random
 from matplotlib import cm
 import imutils
 import itertools
 from matplotlib.backends.backend_agg import FigureCanvasAgg as FigureCanvas
-from typing import List, Tuple, Optional, Dict, Any
+from typing import List, Tuple, Optional, Dict, Any, Union
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 import simba
 from simba.utils.lookups import get_color_dict, get_named_colors
@@ -37,33 +37,22 @@
     def create_gantt_img(self,
                          bouts_df: pd.DataFrame,
                          clf_name: str,
                          image_index: int,
                          fps: int,
                          gantt_img_title: str):
         """
-        Helper to create a single gantt plot based on the data preceeding the input image.
-
-        Parameters
-        ----------
-        bouts_df: pd.DataFrame
-            Pandas dataframe holding information on individual bouts created by ``simba.misc_tools.get_bouts_for_gantt``.
-        clf_name: str
-            Name of the classifier.
-        image_index: int
-            The count of the image.
-        fps: int
-            The fps of the input video.
-        gantt_img_title: str
-            Title of the output image
-
-        Returns
-        -------
-        open_cv_image: np.array
+        Helper to create a single gantt plot based on the data preceeding the input image
 
+        :param pd.DataFrame bouts_df: ataframe holding information on individual bouts created by :meth:`simba.misc_tools.get_bouts_for_gantt`.
+        :param str clf_name: Name of the classifier.
+        :param int image_index: The count of the image. E.g., ``1000`` will create a gantt image representing frame 1-1000.
+        :param int fps: The fps of the input video.
+        :param str gantt_img_title: Title of the image.
+        :return np.ndarray
         """
 
         fig, ax = plt.subplots()
         fig.suptitle(gantt_img_title, fontsize=24)
         relRows = bouts_df.loc[bouts_df['End_frame'] <= image_index]
         for i, event in enumerate(relRows.groupby("Event")):
             data_event = event[1][["Start_time", "Bout_time"]]
@@ -92,27 +81,28 @@
 
         return open_cv_image
 
     def create_single_color_lst(self,
                                 pallete_name: Literal[Options.PALETTE_OPTIONS],
                                 increments: int,
                                 as_rgb_ratio: bool = False,
-                                as_hex: bool = False) -> List[int]:
+                                as_hex: bool = False) -> List[Union[str, int, float]]:
+
         """
         Helper to create a color palette of bgr colors in a list.
-        Parameters
-        ----------
-        pallete_name: str
-            Palette name (e.g., 'jet')
-        increments: int
-            Numbers of colors in the color palette to create.
-
-        Returns
-        -------
-        list
+
+        :param str pallete_name: Palette name (e.g., 'jet')
+        :param int increments: Numbers of colors in the color palette to create.
+        :param bool as_rgb_ratio: If True returns the colors as RGB ratios (0-1).
+        :param bool as_hex: If True, returns the colors as HEX.
+        :return list
+
+        .. note::
+           If as_rgb_ratio **AND** as_hex, then returns HEX.
+
 
         """
         if as_hex:
             as_rgb_ratio = True
         cmap = cm.get_cmap(pallete_name, increments + 1)
         color_lst = []
         for i in range(cmap.N):
@@ -215,43 +205,36 @@
     def make_probability_plot(self,
                               data: pd.Series,
                               style_attr: dict,
                               clf_name: str,
                               fps: int,
                               save_path: str) -> np.ndarray:
         """
-        Helper to make a single classifier probability plot png image.
+        Make a single classifier probability plot png image.
+
+        :param pd.Series data: row representing frames and field representing classification probabilities.
+        :param dict line_attr: Line color attributes.
+        :param dict style_attr: Image attributes (size, font size, line width etc).
+        :param int fps: Video frame rate.
+        :param str ot
+        :param str save_path: Location to store output .png image.
 
-        Parameters
-        ----------
-        data: pd.Series
-            With row representing frames and field representing classification probabilities.
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
-        `GitHub tutorial/documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-classification-probabilities>`__.
 
-        Examples
-        -----
+
+        .. notes::
+          `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#visualizing-classification-probabilities>`__.
+
+        :example:
         >>> data = pd.Series(np.random.random((100, 1)).flatten())
         >>> style_attr = {'width': 640, 'height': 480, 'font size': 10, 'line width': 6, 'color': 'blue', 'circle size': 20}
         >>> clf_name='Attack'
         >>> fps=10
         >>> save_path = '/_test/frames/output/probability_plots/Together_1_final_frame.png'
 
-        >>> _ = make_probability_plot(data=data, style_attr=style_attr, clf_name=clf_name, fps=fps, save_path=save_path)
+        >>> _ = self.make_probability_plot(data=data, style_attr=style_attr, clf_name=clf_name, fps=fps, save_path=save_path)
         """
 
         timer = SimbaTimer()
         timer.start_timer()
         if style_attr['y_max'] == 'auto':
             max_y = float(data.max().round(2))
         else:
@@ -275,26 +258,36 @@
         buffer_.seek(0)
         image = PIL.Image.open(buffer_)
         ar = np.asarray(image)
         img = cv2.cvtColor(ar, cv2.COLOR_RGB2BGR)
         img = np.uint8(cv2.resize(img, (style_attr['width'], style_attr['height'])))
         buffer_.close()
         plt.close()
-
         timer.stop_timer()
         cv2.imwrite(save_path, img)
         stdout_success(msg=f'Final distance plot saved at {save_path}', elapsed_time=timer.elapsed_time_str)
 
     def make_path_plot(self,
                        data_df: pd.DataFrame,
                        video_info: pd.DataFrame,
                        style_attr: dict,
                        deque_dict: dict,
                        clf_attr: dict,
-                       save_path: Optional[str] = None) -> np.ndarray:
+                       save_path: str) -> None:
+
+        """
+        Helper to make a path plot.
+
+        :param pd.DataFrame data_df: Dataframe holding body-part coordinates
+        :param pd.DataFrame video_info: Video info dataframe (parsed project_folder/logs/video_info.csv)
+        :param dict style_attr: Dict holding image style attributes. E.g., {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
+        :param dict deque_dict: Dict with deque holsing all paths to visualize
+        :param dict clf_attr: Dict holding image classifictaion attributes e.g., {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
+        :param str save_path: Location to save image
+        """
 
         video_timer = SimbaTimer(start=True)
         for frm_cnt in range(len(data_df)):
             for animal_cnt, (animal_name, animal_data) in enumerate(deque_dict.items()):
                 bp_x = int(data_df.loc[frm_cnt, '{}_{}'.format(animal_data['bp'], 'x')])
                 bp_y = int(data_df.loc[frm_cnt, '{}_{}'.format(animal_data['bp'], 'y')])
                 deque_dict[animal_name]['deque'].appendleft((bp_x, bp_y))
@@ -334,15 +327,15 @@
     def make_gantt_plot(self,
                         data_df: pd.DataFrame,
                         bouts_df: pd.DataFrame,
                         clf_names: List[str],
                         fps: int,
                         style_attr: dict,
                         video_name: str,
-                        save_path: str) -> np.ndarray:
+                        save_path: str) -> None:
 
         video_timer = SimbaTimer(start=True)
         colours = get_named_colors()
         colour_tuple_x = list(np.arange(3.5, 203.5, 5))
         fig, ax = plt.subplots()
         for i, event in enumerate(bouts_df.groupby("Event")):
             for x in clf_names:
@@ -474,27 +467,18 @@
     def get_bouts_for_gantt(self,
                             data_df: pd.DataFrame,
                             clf_name: str,
                             fps: int) -> np.ndarray:
         """
         Helper to detect all behavior bouts for a specific classifier.
 
-        Parameters
-        ----------
-        data_df: pd.DataFrame
-            Pandas Dataframe with classifier prediction data.
-        clf_name: str
-            Name of the classifier
-        fps: int
-            The fps of the input video.
-
-        Returns
-        -------
-        pd.DataFrame:
-            Holding the start time, end time, end frame, bout time etc of each classified bout.
+        :param pd.DataFrame data_df: Pandas Dataframe with classifier prediction data.
+        :param str clf_name: Name of the classifier
+        :param int fps: The fps of the input video.
+        :return  pd.DataFrame: Holding the start time, end time, end frame, bout time etc of each classified bout.
         """
 
         boutsList, nameList, startTimeList, endTimeList, endFrameList = [], [], [], [], []
         groupDf = pd.DataFrame()
         v = (data_df[clf_name] != data_df[clf_name].shift()).cumsum()
         u = data_df.groupby(v)[clf_name].agg(['all', 'count'])
         m = u['all'] & u['count'].ge(1)
@@ -514,15 +498,15 @@
         return pd.DataFrame(list(zip(nameList, startTimeList, endTimeList, endFrameList, boutsList)),
                             columns=['Event', 'Start_time', 'End Time', 'End_frame', 'Bout_time'])
 
     def resize_gantt(self,
                      gantt_img: np.array,
                      img_height: int) -> np.ndarray:
         """
-        Helper to resize image.
+        Helper to resize image while retaining aspect ratio.
         """
 
         return imutils.resize(gantt_img, height=img_height)
 
     @staticmethod
     def roi_feature_visualizer_mp(data: pd.DataFrame,
                                   text_locations: dict,
```

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.60.1/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/enums.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/checks.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/errors.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/data.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/utils/printing.py` & `Simba-UW-tf-dev-1.60.1/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.60.1/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.60.1/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.60.1/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.60.1/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.60.1/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.60.1/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.60.1/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.60.1/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/SimBA.py` & `Simba-UW-tf-dev-1.60.1/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.60.1/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.1/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.60.1/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.60.1/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.60.1/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.59.9
+Version: 1.60.1
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,15 @@
 simba/feature_extractors/misc/count_values_in_range.py
 simba/feature_extractors/misc/doctests.py
 simba/feature_extractors/misc/egocentrical_aligner.py
 simba/feature_extractors/misc/fish_feature_extractor_2022.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
 simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/peaks.py
 simba/feature_extractors/misc/read_in_mp.py
 simba/feature_extractors/misc/termite_rois.csv
```

### Comparing `Simba-UW-tf-dev-1.59.9/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/LICENSE.md` & `Simba-UW-tf-dev-1.60.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/README.md` & `Simba-UW-tf-dev-1.60.1/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.59.9/setup.py` & `Simba-UW-tf-dev-1.60.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.59.9",
+    version="1.60.1",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

