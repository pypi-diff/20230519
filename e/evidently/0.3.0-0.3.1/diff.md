# Comparing `tmp/evidently-0.3.0.tar.gz` & `tmp/evidently-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evidently-0.3.0.tar", last modified: Wed Apr 12 10:10:18 2023, max compression
+gzip compressed data, was "evidently-0.3.1.tar", last modified: Thu Apr 27 10:29:13 2023, max compression
```

## Comparing `evidently-0.3.0.tar` & `evidently-0.3.1.tar`

### file list

```diff
@@ -1,205 +1,208 @@
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.321893 evidently-0.3.0/
--rw-r--r--   0 emelidral   (501) staff       (20)      373 2023-04-12 10:10:18.322016 evidently-0.3.0/PKG-INFO
--rw-r--r--   0 emelidral   (501) staff       (20)     1447 2023-04-11 11:50:44.033151 evidently-0.3.0/setup.cfg
--rw-r--r--   0 emelidral   (501) staff       (20)     2068 2023-04-11 11:50:44.033217 evidently-0.3.0/setup.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.0/setupbase.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.289234 evidently-0.3.0/src/
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.292634 evidently-0.3.0/src/evidently/
--rw-r--r--   0 emelidral   (501) staff       (20)      256 2023-04-11 11:50:44.033482 evidently-0.3.0/src/evidently/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2680 2023-04-11 17:10:42.502107 evidently-0.3.0/src/evidently/__main__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.0/src/evidently/_config.py
--rw-r--r--   0 emelidral   (501) staff       (20)      111 2023-04-12 10:07:31.233524 evidently-0.3.0/src/evidently/_version.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6886 2023-04-11 22:08:01.497073 evidently-0.3.0/src/evidently/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.294020 evidently-0.3.0/src/evidently/calculations/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.0/src/evidently/calculations/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.0/src/evidently/calculations/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16012 2023-04-11 11:50:44.034784 evidently-0.3.0/src/evidently/calculations/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.0/src/evidently/calculations/data_integration.py
--rw-r--r--   0 emelidral   (501) staff       (20)    31464 2023-04-11 11:50:44.034969 evidently-0.3.0/src/evidently/calculations/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.0/src/evidently/calculations/regression_performance.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.298034 evidently-0.3.0/src/evidently/calculations/stattests/
--rw-r--r--   0 emelidral   (501) staff       (20)     1184 2023-04-11 11:50:44.035148 evidently-0.3.0/src/evidently/calculations/stattests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-04-11 11:50:44.035216 evidently-0.3.0/src/evidently/calculations/stattests/anderson_darling_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.0/src/evidently/calculations/stattests/chisquare_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5352 2023-04-11 11:50:44.035359 evidently-0.3.0/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.0/src/evidently/calculations/stattests/energy_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.0/src/evidently/calculations/stattests/epps_singleton_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.0/src/evidently/calculations/stattests/fisher_exact_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.0/src/evidently/calculations/stattests/g_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.0/src/evidently/calculations/stattests/hellinger_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.0/src/evidently/calculations/stattests/jensenshannon.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.0/src/evidently/calculations/stattests/kl_div.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.0/src/evidently/calculations/stattests/ks_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1732 2023-04-11 11:50:44.035946 evidently-0.3.0/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.0/src/evidently/calculations/stattests/mmd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.0/src/evidently/calculations/stattests/psi.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4586 2023-04-11 11:50:44.036122 evidently-0.3.0/src/evidently/calculations/stattests/registry.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.0/src/evidently/calculations/stattests/t_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)      743 2023-04-11 11:50:44.036270 evidently-0.3.0/src/evidently/calculations/stattests/text_content_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.0/src/evidently/calculations/stattests/tvd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.0/src/evidently/calculations/stattests/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.0/src/evidently/calculations/stattests/wasserstein_distance_norm.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.0/src/evidently/calculations/stattests/z_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.0/src/evidently/calculations/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7042 2023-04-11 22:08:01.497774 evidently-0.3.0/src/evidently/core.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.298911 evidently-0.3.0/src/evidently/descriptors/
--rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-04-11 11:50:44.040731 evidently-0.3.0/src/evidently/descriptors/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.0/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-04-11 11:50:44.040840 evidently-0.3.0/src/evidently/descriptors/oov_words_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.0/src/evidently/descriptors/text_length_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-04-11 11:50:44.040933 evidently-0.3.0/src/evidently/descriptors/trigger_words_presence_descriptor.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.299951 evidently-0.3.0/src/evidently/features/
--rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-04-11 11:50:44.041013 evidently-0.3.0/src/evidently/features/OOV_words_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.0/src/evidently/features/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1894 2023-04-11 11:50:44.041102 evidently-0.3.0/src/evidently/features/generated_features.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-04-11 11:50:44.041157 evidently-0.3.0/src/evidently/features/non_letter_character_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-04-11 11:50:44.041206 evidently-0.3.0/src/evidently/features/text_length_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-04-11 11:50:44.041271 evidently-0.3.0/src/evidently/features/trigger_words_presence_feature.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.301404 evidently-0.3.0/src/evidently/metric_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.0/src/evidently/metric_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.0/src/evidently/metric_preset/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3973 2023-04-11 11:50:44.041471 evidently-0.3.0/src/evidently/metric_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.0/src/evidently/metric_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.0/src/evidently/metric_preset/metric_preset.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.0/src/evidently/metric_preset/regression_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.0/src/evidently/metric_preset/target_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.0/src/evidently/metric_preset/text_overview.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7679 2023-04-11 22:08:01.498430 evidently-0.3.0/src/evidently/metric_results.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.301934 evidently-0.3.0/src/evidently/metrics/
--rw-r--r--   0 emelidral   (501) staff       (20)     3737 2023-04-11 11:50:44.041950 evidently-0.3.0/src/evidently/metrics/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.0/src/evidently/metrics/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.304405 evidently-0.3.0/src/evidently/metrics/classification_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.0/src/evidently/metrics/classification_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2994 2023-04-11 11:50:44.042167 evidently-0.3.0/src/evidently/metrics/classification_performance/base_classification_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2890 2023-04-11 11:50:44.042230 evidently-0.3.0/src/evidently/metrics/classification_performance/class_balance_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4298 2023-04-11 11:50:44.042357 evidently-0.3.0/src/evidently/metrics/classification_performance/class_separation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11993 2023-04-11 11:50:44.042435 evidently-0.3.0/src/evidently/metrics/classification_performance/classification_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-04-11 11:50:44.042500 evidently-0.3.0/src/evidently/metrics/classification_performance/classification_quality_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3312 2023-04-11 11:50:44.042564 evidently-0.3.0/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1534 2023-04-11 11:50:44.042621 evidently-0.3.0/src/evidently/metrics/classification_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-04-11 11:50:44.042685 evidently-0.3.0/src/evidently/metrics/classification_performance/pr_curve_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-04-11 11:50:44.042749 evidently-0.3.0/src/evidently/metrics/classification_performance/pr_table_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5959 2023-04-11 11:50:44.042828 evidently-0.3.0/src/evidently/metrics/classification_performance/probability_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7318 2023-04-11 11:50:44.042904 evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_class_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16900 2023-04-11 22:08:01.499197 evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_feature_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-04-11 11:50:44.043054 evidently-0.3.0/src/evidently/metrics/classification_performance/roc_curve_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.306211 evidently-0.3.0/src/evidently/metrics/data_drift/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.0/src/evidently/metrics/data_drift/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16581 2023-04-11 11:50:44.043222 evidently-0.3.0/src/evidently/metrics/data_drift/column_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6963 2023-04-11 11:50:44.043309 evidently-0.3.0/src/evidently/metrics/data_drift/column_value_plot.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12269 2023-04-11 11:50:44.043396 evidently-0.3.0/src/evidently/metrics/data_drift/data_drift_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4682 2023-04-11 11:50:44.043500 evidently-0.3.0/src/evidently/metrics/data_drift/dataset_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10630 2023-04-11 11:50:44.043573 evidently-0.3.0/src/evidently/metrics/data_drift/embedding_drift_methods.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4469 2023-04-11 11:50:44.043645 evidently-0.3.0/src/evidently/metrics/data_drift/embeddings_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13290 2023-04-11 11:50:44.043698 evidently-0.3.0/src/evidently/metrics/data_drift/target_by_features_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10000 2023-04-11 11:50:44.043757 evidently-0.3.0/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11173 2023-04-11 11:50:44.043845 evidently-0.3.0/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.307315 evidently-0.3.0/src/evidently/metrics/data_integrity/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.0/src/evidently/metrics/data_integrity/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8345 2023-04-11 11:50:44.043991 evidently-0.3.0/src/evidently/metrics/data_integrity/column_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7142 2023-04-11 11:50:44.044068 evidently-0.3.0/src/evidently/metrics/data_integrity/column_regexp_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    30453 2023-04-11 11:50:44.044199 evidently-0.3.0/src/evidently/metrics/data_integrity/column_summary_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12456 2023-04-11 11:50:44.044306 evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8789 2023-04-11 11:50:44.044393 evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_summary_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.309456 evidently-0.3.0/src/evidently/metrics/data_quality/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.0/src/evidently/metrics/data_quality/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5821 2023-04-11 11:50:44.044563 evidently-0.3.0/src/evidently/metrics/data_quality/column_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3054 2023-04-11 11:50:44.044629 evidently-0.3.0/src/evidently/metrics/data_quality/column_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5936 2023-04-11 11:50:44.044695 evidently-0.3.0/src/evidently/metrics/data_quality/column_quantile_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6872 2023-04-11 11:50:44.044766 evidently-0.3.0/src/evidently/metrics/data_quality/column_value_list_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8991 2023-04-11 11:50:44.044848 evidently-0.3.0/src/evidently/metrics/data_quality/column_value_range_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.0/src/evidently/metrics/data_quality/conflict_prediction_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.0/src/evidently/metrics/data_quality/conflict_target_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13927 2023-04-11 11:50:44.045061 evidently-0.3.0/src/evidently/metrics/data_quality/dataset_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-04-11 11:50:44.045118 evidently-0.3.0/src/evidently/metrics/data_quality/stability_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7248 2023-04-11 11:50:44.045194 evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-04-11 11:50:44.045257 evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_distribution.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.312060 evidently-0.3.0/src/evidently/metrics/regression_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.0/src/evidently/metrics/regression_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4488 2023-04-11 11:50:44.045377 evidently-0.3.0/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)    28709 2023-04-11 11:50:44.045473 evidently-0.3.0/src/evidently/metrics/regression_performance/error_bias_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-04-11 11:50:44.045565 evidently-0.3.0/src/evidently/metrics/regression_performance/error_distribution.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4145 2023-04-11 11:50:44.045610 evidently-0.3.0/src/evidently/metrics/regression_performance/error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6061 2023-04-11 11:50:44.045672 evidently-0.3.0/src/evidently/metrics/regression_performance/error_normality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1675 2023-04-11 11:50:44.045735 evidently-0.3.0/src/evidently/metrics/regression_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4214 2023-04-11 11:50:44.045783 evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3896 2023-04-11 11:50:44.045845 evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_vs_actual.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-04-11 11:50:44.045914 evidently-0.3.0/src/evidently/metrics/regression_performance/regression_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12823 2023-04-11 11:50:44.045990 evidently-0.3.0/src/evidently/metrics/regression_performance/regression_performance_metrics.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-04-11 11:50:44.046056 evidently-0.3.0/src/evidently/metrics/regression_performance/regression_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9131 2023-04-11 11:50:44.046126 evidently-0.3.0/src/evidently/metrics/regression_performance/top_error.py
--rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-04-11 11:50:44.046174 evidently-0.3.0/src/evidently/metrics/regression_performance/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4630 2023-04-11 11:50:44.046235 evidently-0.3.0/src/evidently/metrics/regression_performance/visualization.py
--rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.0/src/evidently/metrics/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.312534 evidently-0.3.0/src/evidently/model/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.0/src/evidently/model/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.0/src/evidently/model/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.0/src/evidently/model/widget.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.312706 evidently-0.3.0/src/evidently/nbextension/
--rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.0/src/evidently/nbextension/__init__.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.313401 evidently-0.3.0/src/evidently/nbextension/static/
--rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.0/src/evidently/nbextension/static/extension.js
--rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.0/src/evidently/nbextension/static/index.js
--rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.0/src/evidently/nbextension/static/index.js.LICENSE.txt
--rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.0/src/evidently/nbextension/static/material-ui-icons.woff2
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.314070 evidently-0.3.0/src/evidently/options/
--rw-r--r--   0 emelidral   (501) staff       (20)      783 2023-04-11 11:50:44.056118 evidently-0.3.0/src/evidently/options/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3349 2023-04-11 11:50:44.056178 evidently-0.3.0/src/evidently/options/color_scheme.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-04-11 11:50:44.056254 evidently-0.3.0/src/evidently/options/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.0/src/evidently/options/quality_metrics.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.314409 evidently-0.3.0/src/evidently/pipeline/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.0/src/evidently/pipeline/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1165 2023-04-11 11:50:44.056415 evidently-0.3.0/src/evidently/pipeline/column_mapping.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.315235 evidently-0.3.0/src/evidently/renderers/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.0/src/evidently/renderers/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.0/src/evidently/renderers/base_renderer.py
--rw-r--r--   0 emelidral   (501) staff       (20)    27722 2023-04-11 11:50:44.056806 evidently-0.3.0/src/evidently/renderers/html_widgets.py
--rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.0/src/evidently/renderers/notebook_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.0/src/evidently/renderers/render_utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.315561 evidently-0.3.0/src/evidently/report/
--rw-r--r--   0 emelidral   (501) staff       (20)       27 2023-04-11 11:50:44.057001 evidently-0.3.0/src/evidently/report/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7338 2023-04-11 11:50:44.057070 evidently-0.3.0/src/evidently/report/report.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.316049 evidently-0.3.0/src/evidently/runner/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.0/src/evidently/runner/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.0/src/evidently/runner/loader.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.0/src/evidently/runner/runner.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.316550 evidently-0.3.0/src/evidently/suite/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.0/src/evidently/suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13761 2023-04-11 11:50:44.057526 evidently-0.3.0/src/evidently/suite/base_suite.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.0/src/evidently/suite/execution_graph.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.316876 evidently-0.3.0/src/evidently/telemetry/
--rw-r--r--   0 emelidral   (501) staff       (20)       36 2023-04-11 11:50:44.057752 evidently-0.3.0/src/evidently/telemetry/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.0/src/evidently/telemetry/sender.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.318562 evidently-0.3.0/src/evidently/test_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.0/src/evidently/test_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.0/src/evidently/test_preset/classification_binary.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.0/src/evidently/test_preset/classification_binary_topk.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.0/src/evidently/test_preset/classification_multiclass.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6024 2023-04-11 11:50:44.058298 evidently-0.3.0/src/evidently/test_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.0/src/evidently/test_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.0/src/evidently/test_preset/data_stability.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5483 2023-04-11 11:50:44.058454 evidently-0.3.0/src/evidently/test_preset/no_target_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.0/src/evidently/test_preset/regression.py
--rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.0/src/evidently/test_preset/test_preset.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.318904 evidently-0.3.0/src/evidently/test_suite/
--rw-r--r--   0 emelidral   (501) staff       (20)       34 2023-04-11 11:50:44.058625 evidently-0.3.0/src/evidently/test_suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7454 2023-04-11 11:50:44.058693 evidently-0.3.0/src/evidently/test_suite/test_suite.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.320259 evidently-0.3.0/src/evidently/tests/
--rw-r--r--   0 emelidral   (501) staff       (20)     4410 2023-04-11 11:50:44.058785 evidently-0.3.0/src/evidently/tests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11758 2023-04-11 11:50:44.058862 evidently-0.3.0/src/evidently/tests/base_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22752 2023-04-11 11:50:44.059177 evidently-0.3.0/src/evidently/tests/classification_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    19989 2023-04-11 11:50:44.059285 evidently-0.3.0/src/evidently/tests/data_drift_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    41950 2023-04-11 11:50:44.059392 evidently-0.3.0/src/evidently/tests/data_integrity_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    53163 2023-04-11 11:50:44.059500 evidently-0.3.0/src/evidently/tests/data_quality_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10930 2023-04-11 11:50:44.059579 evidently-0.3.0/src/evidently/tests/regression_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-04-11 11:50:44.059661 evidently-0.3.0/src/evidently/tests/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-12 10:10:18.321850 evidently-0.3.0/src/evidently/utils/
--rw-r--r--   0 emelidral   (501) staff       (20)       40 2023-04-11 11:50:44.059731 evidently-0.3.0/src/evidently/utils/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.0/src/evidently/utils/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8342 2023-04-11 11:50:44.059864 evidently-0.3.0/src/evidently/utils/data_drift_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.0/src/evidently/utils/data_operations.py
--rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.0/src/evidently/utils/data_preprocessing.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.0/src/evidently/utils/generators.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1392 2023-04-11 22:08:01.499801 evidently-0.3.0/src/evidently/utils/numpy_encoder.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.060206 evidently-0.3.0/src/evidently/utils/types.py
--rw-r--r--   0 emelidral   (501) staff       (20)    25482 2023-04-11 11:50:44.060302 evidently-0.3.0/src/evidently/utils/visualizations.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.213387 evidently-0.3.1/
+-rw-r--r--   0 emelidral   (501) staff       (20)      373 2023-04-27 10:29:13.213518 evidently-0.3.1/PKG-INFO
+-rw-r--r--   0 emelidral   (501) staff       (20)     1447 2023-04-11 11:50:44.033151 evidently-0.3.1/setup.cfg
+-rw-r--r--   0 emelidral   (501) staff       (20)     2068 2023-04-11 11:50:44.033217 evidently-0.3.1/setup.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.1/setupbase.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.171365 evidently-0.3.1/src/
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.176027 evidently-0.3.1/src/evidently/
+-rw-r--r--   0 emelidral   (501) staff       (20)      256 2023-04-11 11:50:44.033482 evidently-0.3.1/src/evidently/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1892 2023-04-27 10:27:02.402053 evidently-0.3.1/src/evidently/__main__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.1/src/evidently/_config.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      111 2023-04-27 10:27:48.159586 evidently-0.3.1/src/evidently/_version.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7505 2023-04-27 10:27:02.402425 evidently-0.3.1/src/evidently/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.177724 evidently-0.3.1/src/evidently/calculations/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.1/src/evidently/calculations/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.1/src/evidently/calculations/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16012 2023-04-11 11:50:44.034784 evidently-0.3.1/src/evidently/calculations/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.1/src/evidently/calculations/data_integration.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    32536 2023-04-27 10:27:02.402855 evidently-0.3.1/src/evidently/calculations/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.1/src/evidently/calculations/regression_performance.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.182859 evidently-0.3.1/src/evidently/calculations/stattests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1258 2023-04-27 10:27:02.403157 evidently-0.3.1/src/evidently/calculations/stattests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-04-11 11:50:44.035216 evidently-0.3.1/src/evidently/calculations/stattests/anderson_darling_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.1/src/evidently/calculations/stattests/chisquare_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7331 2023-04-27 10:27:02.403563 evidently-0.3.1/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.1/src/evidently/calculations/stattests/energy_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.1/src/evidently/calculations/stattests/epps_singleton_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.1/src/evidently/calculations/stattests/fisher_exact_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.1/src/evidently/calculations/stattests/g_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.1/src/evidently/calculations/stattests/hellinger_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.1/src/evidently/calculations/stattests/jensenshannon.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.1/src/evidently/calculations/stattests/kl_div.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.1/src/evidently/calculations/stattests/ks_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1732 2023-04-11 11:50:44.035946 evidently-0.3.1/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.1/src/evidently/calculations/stattests/mmd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.1/src/evidently/calculations/stattests/psi.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4696 2023-04-27 10:27:02.403868 evidently-0.3.1/src/evidently/calculations/stattests/registry.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.1/src/evidently/calculations/stattests/t_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      799 2023-04-27 10:27:02.404121 evidently-0.3.1/src/evidently/calculations/stattests/text_content_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      791 2023-04-27 10:27:02.404318 evidently-0.3.1/src/evidently/calculations/stattests/text_content_drift_abs.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.1/src/evidently/calculations/stattests/tvd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.1/src/evidently/calculations/stattests/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.1/src/evidently/calculations/stattests/wasserstein_distance_norm.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.1/src/evidently/calculations/stattests/z_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.1/src/evidently/calculations/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7042 2023-04-24 17:06:50.387018 evidently-0.3.1/src/evidently/core.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.183967 evidently-0.3.1/src/evidently/descriptors/
+-rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-04-11 11:50:44.040731 evidently-0.3.1/src/evidently/descriptors/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.1/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-04-11 11:50:44.040840 evidently-0.3.1/src/evidently/descriptors/oov_words_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.1/src/evidently/descriptors/text_length_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-04-11 11:50:44.040933 evidently-0.3.1/src/evidently/descriptors/trigger_words_presence_descriptor.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.185226 evidently-0.3.1/src/evidently/features/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-04-11 11:50:44.041013 evidently-0.3.1/src/evidently/features/OOV_words_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.1/src/evidently/features/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1894 2023-04-11 11:50:44.041102 evidently-0.3.1/src/evidently/features/generated_features.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-04-11 11:50:44.041157 evidently-0.3.1/src/evidently/features/non_letter_character_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-04-11 11:50:44.041206 evidently-0.3.1/src/evidently/features/text_length_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-04-11 11:50:44.041271 evidently-0.3.1/src/evidently/features/trigger_words_presence_feature.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.186934 evidently-0.3.1/src/evidently/metric_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.1/src/evidently/metric_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.1/src/evidently/metric_preset/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4787 2023-04-27 10:27:02.404624 evidently-0.3.1/src/evidently/metric_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.1/src/evidently/metric_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.1/src/evidently/metric_preset/metric_preset.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.1/src/evidently/metric_preset/regression_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.1/src/evidently/metric_preset/target_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.1/src/evidently/metric_preset/text_overview.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8795 2023-04-27 10:27:02.404905 evidently-0.3.1/src/evidently/metric_results.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.187546 evidently-0.3.1/src/evidently/metrics/
+-rw-r--r--   0 emelidral   (501) staff       (20)     3737 2023-04-11 11:50:44.041950 evidently-0.3.1/src/evidently/metrics/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.1/src/evidently/metrics/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.190618 evidently-0.3.1/src/evidently/metrics/classification_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.1/src/evidently/metrics/classification_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2994 2023-04-11 11:50:44.042167 evidently-0.3.1/src/evidently/metrics/classification_performance/base_classification_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3132 2023-04-27 10:27:02.405129 evidently-0.3.1/src/evidently/metrics/classification_performance/class_balance_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4298 2023-04-11 11:50:44.042357 evidently-0.3.1/src/evidently/metrics/classification_performance/class_separation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12015 2023-04-27 10:27:02.405315 evidently-0.3.1/src/evidently/metrics/classification_performance/classification_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-04-11 11:50:44.042500 evidently-0.3.1/src/evidently/metrics/classification_performance/classification_quality_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3569 2023-04-27 10:27:02.405480 evidently-0.3.1/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1534 2023-04-11 11:50:44.042621 evidently-0.3.1/src/evidently/metrics/classification_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-04-11 11:50:44.042685 evidently-0.3.1/src/evidently/metrics/classification_performance/pr_curve_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-04-11 11:50:44.042749 evidently-0.3.1/src/evidently/metrics/classification_performance/pr_table_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5959 2023-04-11 11:50:44.042828 evidently-0.3.1/src/evidently/metrics/classification_performance/probability_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7318 2023-04-11 11:50:44.042904 evidently-0.3.1/src/evidently/metrics/classification_performance/quality_by_class_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16640 2023-04-27 10:27:02.405864 evidently-0.3.1/src/evidently/metrics/classification_performance/quality_by_feature_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-04-11 11:50:44.043054 evidently-0.3.1/src/evidently/metrics/classification_performance/roc_curve_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.192754 evidently-0.3.1/src/evidently/metrics/data_drift/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.1/src/evidently/metrics/data_drift/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16581 2023-04-11 11:50:44.043222 evidently-0.3.1/src/evidently/metrics/data_drift/column_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6963 2023-04-11 11:50:44.043309 evidently-0.3.1/src/evidently/metrics/data_drift/column_value_plot.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12293 2023-04-27 10:27:02.406117 evidently-0.3.1/src/evidently/metrics/data_drift/data_drift_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4706 2023-04-27 10:27:02.406287 evidently-0.3.1/src/evidently/metrics/data_drift/dataset_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10729 2023-04-27 10:27:02.406479 evidently-0.3.1/src/evidently/metrics/data_drift/embedding_drift_methods.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4516 2023-04-27 10:27:02.406718 evidently-0.3.1/src/evidently/metrics/data_drift/embeddings_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13290 2023-04-11 11:50:44.043698 evidently-0.3.1/src/evidently/metrics/data_drift/target_by_features_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10024 2023-04-27 10:27:02.406909 evidently-0.3.1/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11173 2023-04-11 11:50:44.043845 evidently-0.3.1/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.194030 evidently-0.3.1/src/evidently/metrics/data_integrity/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.1/src/evidently/metrics/data_integrity/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8345 2023-04-11 11:50:44.043991 evidently-0.3.1/src/evidently/metrics/data_integrity/column_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7142 2023-04-11 11:50:44.044068 evidently-0.3.1/src/evidently/metrics/data_integrity/column_regexp_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    27020 2023-04-27 10:27:02.407423 evidently-0.3.1/src/evidently/metrics/data_integrity/column_summary_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12456 2023-04-11 11:50:44.044306 evidently-0.3.1/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8789 2023-04-11 11:50:44.044393 evidently-0.3.1/src/evidently/metrics/data_integrity/dataset_summary_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.196548 evidently-0.3.1/src/evidently/metrics/data_quality/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.1/src/evidently/metrics/data_quality/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5821 2023-04-11 11:50:44.044563 evidently-0.3.1/src/evidently/metrics/data_quality/column_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3054 2023-04-11 11:50:44.044629 evidently-0.3.1/src/evidently/metrics/data_quality/column_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5896 2023-04-27 10:27:02.407846 evidently-0.3.1/src/evidently/metrics/data_quality/column_quantile_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6872 2023-04-11 11:50:44.044766 evidently-0.3.1/src/evidently/metrics/data_quality/column_value_list_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8991 2023-04-11 11:50:44.044848 evidently-0.3.1/src/evidently/metrics/data_quality/column_value_range_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.1/src/evidently/metrics/data_quality/conflict_prediction_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.1/src/evidently/metrics/data_quality/conflict_target_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13927 2023-04-11 11:50:44.045061 evidently-0.3.1/src/evidently/metrics/data_quality/dataset_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-04-11 11:50:44.045118 evidently-0.3.1/src/evidently/metrics/data_quality/stability_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7248 2023-04-11 11:50:44.045194 evidently-0.3.1/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-04-11 11:50:44.045257 evidently-0.3.1/src/evidently/metrics/data_quality/text_descriptors_distribution.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.199630 evidently-0.3.1/src/evidently/metrics/regression_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.1/src/evidently/metrics/regression_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4488 2023-04-11 11:50:44.045377 evidently-0.3.1/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    28336 2023-04-27 10:27:02.408320 evidently-0.3.1/src/evidently/metrics/regression_performance/error_bias_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-04-11 11:50:44.045565 evidently-0.3.1/src/evidently/metrics/regression_performance/error_distribution.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4145 2023-04-11 11:50:44.045610 evidently-0.3.1/src/evidently/metrics/regression_performance/error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6061 2023-04-11 11:50:44.045672 evidently-0.3.1/src/evidently/metrics/regression_performance/error_normality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1675 2023-04-11 11:50:44.045735 evidently-0.3.1/src/evidently/metrics/regression_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4214 2023-04-11 11:50:44.045783 evidently-0.3.1/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3896 2023-04-11 11:50:44.045845 evidently-0.3.1/src/evidently/metrics/regression_performance/predicted_vs_actual.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-04-11 11:50:44.045914 evidently-0.3.1/src/evidently/metrics/regression_performance/regression_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12823 2023-04-11 11:50:44.045990 evidently-0.3.1/src/evidently/metrics/regression_performance/regression_performance_metrics.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-04-11 11:50:44.046056 evidently-0.3.1/src/evidently/metrics/regression_performance/regression_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9131 2023-04-11 11:50:44.046126 evidently-0.3.1/src/evidently/metrics/regression_performance/top_error.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-04-11 11:50:44.046174 evidently-0.3.1/src/evidently/metrics/regression_performance/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4630 2023-04-11 11:50:44.046235 evidently-0.3.1/src/evidently/metrics/regression_performance/visualization.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.1/src/evidently/metrics/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.200502 evidently-0.3.1/src/evidently/model/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.1/src/evidently/model/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.1/src/evidently/model/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.1/src/evidently/model/widget.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.200726 evidently-0.3.1/src/evidently/nbextension/
+-rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.1/src/evidently/nbextension/__init__.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.201617 evidently-0.3.1/src/evidently/nbextension/static/
+-rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.1/src/evidently/nbextension/static/extension.js
+-rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.1/src/evidently/nbextension/static/index.js
+-rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.1/src/evidently/nbextension/static/index.js.LICENSE.txt
+-rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.1/src/evidently/nbextension/static/material-ui-icons.woff2
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.203572 evidently-0.3.1/src/evidently/options/
+-rw-r--r--   0 emelidral   (501) staff       (20)      471 2023-04-27 10:27:02.408578 evidently-0.3.1/src/evidently/options/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2637 2023-04-27 10:27:02.408728 evidently-0.3.1/src/evidently/options/base.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3391 2023-04-27 10:27:02.408907 evidently-0.3.1/src/evidently/options/color_scheme.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-04-11 11:50:44.056254 evidently-0.3.1/src/evidently/options/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)       67 2023-04-27 10:27:02.409017 evidently-0.3.1/src/evidently/options/option.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.1/src/evidently/options/quality_metrics.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.204016 evidently-0.3.1/src/evidently/pipeline/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.1/src/evidently/pipeline/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1162 2023-04-27 10:27:02.409249 evidently-0.3.1/src/evidently/pipeline/column_mapping.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.205174 evidently-0.3.1/src/evidently/renderers/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.1/src/evidently/renderers/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.1/src/evidently/renderers/base_renderer.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    27722 2023-04-11 11:50:44.056806 evidently-0.3.1/src/evidently/renderers/html_widgets.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.1/src/evidently/renderers/notebook_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.1/src/evidently/renderers/render_utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.205625 evidently-0.3.1/src/evidently/report/
+-rw-r--r--   0 emelidral   (501) staff       (20)       27 2023-04-11 11:50:44.057001 evidently-0.3.1/src/evidently/report/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7495 2023-04-27 10:27:02.409529 evidently-0.3.1/src/evidently/report/report.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.206230 evidently-0.3.1/src/evidently/runner/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.1/src/evidently/runner/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.1/src/evidently/runner/loader.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.1/src/evidently/runner/runner.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.206836 evidently-0.3.1/src/evidently/suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.1/src/evidently/suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13890 2023-04-27 10:27:02.409871 evidently-0.3.1/src/evidently/suite/base_suite.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.1/src/evidently/suite/execution_graph.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.207260 evidently-0.3.1/src/evidently/telemetry/
+-rw-r--r--   0 emelidral   (501) staff       (20)       36 2023-04-11 11:50:44.057752 evidently-0.3.1/src/evidently/telemetry/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.1/src/evidently/telemetry/sender.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.209381 evidently-0.3.1/src/evidently/test_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.1/src/evidently/test_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.1/src/evidently/test_preset/classification_binary.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.1/src/evidently/test_preset/classification_binary_topk.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.1/src/evidently/test_preset/classification_multiclass.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7352 2023-04-27 10:27:02.410133 evidently-0.3.1/src/evidently/test_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.1/src/evidently/test_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.1/src/evidently/test_preset/data_stability.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6811 2023-04-27 10:27:02.410385 evidently-0.3.1/src/evidently/test_preset/no_target_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.1/src/evidently/test_preset/regression.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.1/src/evidently/test_preset/test_preset.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.209801 evidently-0.3.1/src/evidently/test_suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)       34 2023-04-11 11:50:44.058625 evidently-0.3.1/src/evidently/test_suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8419 2023-04-27 10:27:02.410660 evidently-0.3.1/src/evidently/test_suite/test_suite.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.211547 evidently-0.3.1/src/evidently/tests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     4460 2023-04-27 10:27:02.410897 evidently-0.3.1/src/evidently/tests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11758 2023-04-11 11:50:44.058862 evidently-0.3.1/src/evidently/tests/base_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22752 2023-04-11 11:50:44.059177 evidently-0.3.1/src/evidently/tests/classification_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    21917 2023-04-27 10:27:02.411138 evidently-0.3.1/src/evidently/tests/data_drift_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    42332 2023-04-27 10:27:02.411682 evidently-0.3.1/src/evidently/tests/data_integrity_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    53681 2023-04-27 10:27:02.412175 evidently-0.3.1/src/evidently/tests/data_quality_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10930 2023-04-11 11:50:44.059579 evidently-0.3.1/src/evidently/tests/regression_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-04-11 11:50:44.059661 evidently-0.3.1/src/evidently/tests/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-04-27 10:29:13.213353 evidently-0.3.1/src/evidently/utils/
+-rw-r--r--   0 emelidral   (501) staff       (20)       40 2023-04-11 11:50:44.059731 evidently-0.3.1/src/evidently/utils/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.1/src/evidently/utils/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9086 2023-04-27 10:27:02.412473 evidently-0.3.1/src/evidently/utils/data_drift_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.1/src/evidently/utils/data_operations.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.1/src/evidently/utils/data_preprocessing.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.1/src/evidently/utils/generators.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1392 2023-04-24 17:06:50.391821 evidently-0.3.1/src/evidently/utils/numpy_encoder.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.060206 evidently-0.3.1/src/evidently/utils/types.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    26111 2023-04-27 10:27:02.412839 evidently-0.3.1/src/evidently/utils/visualizations.py
```

### Comparing `evidently-0.3.0/setup.cfg` & `evidently-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/setup.py` & `evidently-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/setupbase.py` & `evidently-0.3.1/setupbase.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/__main__.py` & `evidently-0.3.1/src/evidently/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 import argparse
-import json
 import logging
-import os
 import sys
 from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 
-import yaml
-
-from evidently._config import TELEMETRY_ADDRESS
-from evidently._config import TELEMETRY_ENABLED
-from evidently.pipeline.column_mapping import ColumnMapping
 from evidently.runner.loader import SamplingOptions
-from evidently.runner.runner import DataOptions
-from evidently.runner.runner import parse_options
-from evidently.telemetry import TelemetrySender
 
 
 @dataclass
 class DataFormatOptions:
     header: bool
     separator: str
     date_column: str
@@ -49,25 +39,14 @@
     pretty_print: bool = False
 
 
 def __get_not_none(src: Dict, key, default):
     return default if src.get(key, None) is None else src.get(key)
 
 
-def __load_config_file(config_file: str):
-    with open(config_file, encoding="utf-8") as f_config:
-        if config_file.endswith(".yaml") or config_file.endswith(".yml"):
-            opts_data = yaml.load(f_config, Loader=yaml.SafeLoader)
-        elif config_file.endswith(".json"):
-            opts_data = json.load(f_config)
-        else:
-            raise Exception(f"config .{config_file.split('.')[-1]} not supported")
-    return opts_data
-
-
 def help_handler(**_kv):
     parser.print_help()
     sys.exit(1)
 
 
 def _add_default_parameters(configurable_parser, default_output_name: str):
     configurable_parser.add_argument("--reference", dest="reference", required=True, help="Path to reference data")
@@ -84,11 +63,10 @@
 parser = argparse.ArgumentParser()
 
 parsers = parser.add_subparsers()
 parser.set_defaults(handler=help_handler)
 calculate_parser = parsers.add_parser("calculate")
 calc_subparsers = calculate_parser.add_subparsers()
 
-
 parsed = parser.parse_args(sys.argv[1:])
 
 parsed.handler(**parsed.__dict__)
```

### Comparing `evidently-0.3.0/src/evidently/base_metric.py` & `evidently-0.3.1/src/evidently/base_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from typing import Union
 
 import pandas as pd
 
 from evidently.core import BaseResult
 from evidently.core import ColumnType
 from evidently.features.generated_features import GeneratedFeature
+from evidently.options.base import AnyOptions
+from evidently.options.base import Options
 from evidently.pipeline.column_mapping import ColumnMapping
 from evidently.utils.data_preprocessing import DataDefinition
 
 if TYPE_CHECKING:
     from evidently.suite.base_suite import Context
 
 
@@ -136,14 +138,22 @@
 
 TResult = TypeVar("TResult", bound=MetricResult)
 
 
 class Metric(Generic[TResult]):
     context: Optional["Context"] = None
 
+    # TODO: if we want metric-specific options
+    options: Options
+    # resulting options will be determined via
+    # options = global_option.override(display_options).override(metric_options)
+
+    def __init__(self, options: AnyOptions = None):
+        self.options = Options.from_any_options(options)
+
     def get_id(self) -> str:
         return self.__class__.__name__
 
     @abc.abstractmethod
     def calculate(self, data: InputData) -> TResult:
         raise NotImplementedError()
 
@@ -182,14 +192,20 @@
         for field, value in sorted(self.__dict__.items(), key=lambda x: x[0]):
             if field in ["context"]:
                 continue
             if issubclass(type(value), ColumnName) and value.feature_class is not None:
                 required_features.append(value.feature_class)
         return required_features
 
+    def get_options(self):
+        options = self.options if hasattr(self, "options") else Options()
+        if self.context is not None:
+            options = self.context.options.override(options)
+        return options
+
 
 class ColumnMetricResult(MetricResult):
     column_name: str
     # todo: use enum
     column_type: str
 
     def get_pandas(self) -> pd.DataFrame:
```

### Comparing `evidently-0.3.0/src/evidently/calculations/classification_performance.py` & `evidently-0.3.1/src/evidently/calculations/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/data_drift.py` & `evidently-0.3.1/src/evidently/calculations/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/data_integration.py` & `evidently-0.3.1/src/evidently/calculations/data_integration.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/data_quality.py` & `evidently-0.3.1/src/evidently/calculations/data_quality.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Methods for overall dataset quality calculations - rows count, a specific values count, etc."""
 
 import dataclasses
 from typing import Callable
+from typing import Collection
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import chi2_contingency
 
+from evidently.core import ColumnType
 from evidently.metric_results import ColumnCorrelations
 from evidently.metric_results import DatasetColumns
 from evidently.metric_results import Distribution
 from evidently.metric_results import Histogram
 from evidently.metric_results import HistogramData
 from evidently.utils.data_preprocessing import DataDefinition
 from evidently.utils.types import ColumnDistribution
@@ -156,19 +158,19 @@
         ):
             if features is not None and item in features:
                 return features[item]
 
         raise KeyError(item)
 
 
-def get_features_stats(feature: pd.Series, feature_type: str) -> FeatureQualityStats:
+def get_features_stats(feature: pd.Series, feature_type: ColumnType) -> FeatureQualityStats:
     def get_percentage_from_all_values(value: Union[int, float]) -> float:
         return np.round(100 * value / all_values_count, 2)
 
-    result = FeatureQualityStats(feature_type=feature_type)
+    result = FeatureQualityStats(feature_type=feature_type.value)
     all_values_count = feature.shape[0]
 
     if not all_values_count > 0:
         # we have no data, return default stats for en empty dataset
         return result
     result.number_of_rows = all_values_count
     result.missing_count = int(feature.isnull().sum())
@@ -182,15 +184,15 @@
     result.most_common_value = value_counts.index[0]
     result.most_common_value_percentage = get_percentage_from_all_values(value_counts.iloc[0])
 
     if result.count > 0 and pd.isnull(result.most_common_value):
         result.most_common_not_null_value = value_counts.index[1]
         result.most_common_not_null_value_percentage = get_percentage_from_all_values(value_counts.iloc[1])
 
-    if feature_type == "num":
+    if feature_type == ColumnType.Numerical:
         # round most common feature value for numeric features to 1e-5
         if not np.issubdtype(feature, np.number):
             feature = feature.astype(float)
         if isinstance(result.most_common_value, float):
             result.most_common_value = np.round(result.most_common_value, 5)
         result.infinite_count = int(np.sum(np.isinf(feature)))
         result.infinite_percentage = get_percentage_from_all_values(result.infinite_count)
@@ -200,15 +202,15 @@
         std = common_stats["std"]
         result.std = np.round(std, 2)
         result.mean = np.round(common_stats["mean"], 2)
         result.percentile_25 = np.round(common_stats["25%"], 2)
         result.percentile_50 = np.round(common_stats["50%"], 2)
         result.percentile_75 = np.round(common_stats["75%"], 2)
 
-    if feature_type == "datetime":
+    if feature_type == ColumnType.Datetime:
         # cast datetime value to str for datetime features
         result.most_common_value = str(result.most_common_value)
         # cast datetime value to str for datetime features
         result.max = str(feature.max())
         result.min = str(feature.min())
 
     return result
@@ -216,383 +218,423 @@
 
 def calculate_data_quality_stats(
     dataset: pd.DataFrame, columns: DatasetColumns, task: Optional[str]
 ) -> DataQualityStats:
     result = DataQualityStats(rows_count=get_rows_count(dataset))
 
     result.num_features_stats = {
-        feature_name: get_features_stats(dataset[feature_name], feature_type="num")
+        feature_name: get_features_stats(dataset[feature_name], feature_type=ColumnType.Numerical)
         for feature_name in columns.num_feature_names
     }
 
     result.cat_features_stats = {
-        feature_name: get_features_stats(dataset[feature_name], feature_type="cat")
+        feature_name: get_features_stats(dataset[feature_name], feature_type=ColumnType.Categorical)
         for feature_name in columns.cat_feature_names
     }
 
     if columns.utility_columns.date:
         date_list = columns.datetime_feature_names + [columns.utility_columns.date]
 
     else:
         date_list = columns.datetime_feature_names
 
     result.datetime_features_stats = {
-        feature_name: get_features_stats(dataset[feature_name], feature_type="datetime") for feature_name in date_list
+        feature_name: get_features_stats(dataset[feature_name], feature_type=ColumnType.Datetime)
+        for feature_name in date_list
     }
 
     target_name = columns.utility_columns.target
 
     if target_name is not None and target_name in dataset:
         result.target_stats = {}
 
         if task == "classification":
-            result.target_stats[target_name] = get_features_stats(dataset[target_name], feature_type="cat")
+            result.target_stats[target_name] = get_features_stats(
+                dataset[target_name],
+                feature_type=ColumnType.Categorical,
+            )
 
         else:
-            result.target_stats[target_name] = get_features_stats(dataset[target_name], feature_type="num")
+            result.target_stats[target_name] = get_features_stats(
+                dataset[target_name],
+                feature_type=ColumnType.Numerical,
+            )
 
     prediction_name = columns.utility_columns.prediction
 
     if isinstance(prediction_name, str) and prediction_name in dataset:
         result.prediction_stats = {}
 
         if task == "classification":
-            result.prediction_stats[prediction_name] = get_features_stats(dataset[prediction_name], feature_type="cat")
+            result.prediction_stats[prediction_name] = get_features_stats(
+                dataset[prediction_name],
+                feature_type=ColumnType.Categorical,
+            )
 
         else:
-            result.prediction_stats[prediction_name] = get_features_stats(dataset[prediction_name], feature_type="num")
+            result.prediction_stats[prediction_name] = get_features_stats(
+                dataset[prediction_name],
+                feature_type=ColumnType.Numerical,
+            )
 
     return result
 
 
-class DataQualityGetPlotData:
-    def __init__(self) -> None:
-        self.period_prefix: Optional[str] = None
-        self.curr: Optional[pd.DataFrame] = None
-        self.ref: Optional[pd.DataFrame] = None
-
-    def calculate_main_plot(
-        self,
-        curr: pd.DataFrame,
-        ref: Optional[pd.DataFrame],
-        feature_name: str,
-        feature_type: str,
-        merge_small_cat: Optional[int] = MAX_CATEGORIES,
-    ) -> Optional[Histogram]:
-        if feature_type == "cat" and merge_small_cat is not None:
-            if ref is not None:
-                ref = ref.copy()
-            if merge_small_cat is not None:
-                curr, ref = self._transform_cat_data(curr.copy(), ref, feature_name, merge_small_cat)
-        curr_data = curr[feature_name].dropna()
-        ref_data = None
-        if ref is not None:
-            ref_data = ref[feature_name].dropna()
-
-        if feature_type == "num":
-            bins_for_hist: Histogram = make_hist_for_num_plot(curr_data, ref_data)
-            log_ref_data = None
-            if ref_data is not None:
-                log_ref_data = np.log10(ref_data[ref_data > 0])
-            bins_for_hist_log = make_hist_for_num_plot(
-                np.log10(curr_data[curr_data > 0]),
-                log_ref_data,
+def _relabel_data(
+    current_data: pd.Series,
+    reference_data: Optional[pd.Series],
+    max_categories: Optional[int] = MAX_CATEGORIES,
+) -> Tuple[pd.Series, Optional[pd.Series]]:
+    if max_categories is None:
+        return current_data.copy(), reference_data.copy() if reference_data is not None else None
+
+    current_data_str = current_data.astype(str)
+    reference_data_str = None
+    if reference_data is not None:
+        reference_data_str = reference_data.astype(str)
+        unique_values = len(
+            np.union1d(
+                current_data_str.unique(),
+                reference_data_str.unique(),
             )
-            bins_for_hist.current_log = bins_for_hist_log.current
-            bins_for_hist.reference_log = bins_for_hist_log.reference
+        )
+    else:
+        unique_values = current_data_str.nunique()
+
+    if unique_values > max_categories:
+        curr_cats = current_data_str.value_counts(normalize=True)
+
+        if reference_data_str is not None:
+            ref_cats = reference_data_str.value_counts(normalize=True)
+            categories = pd.concat([curr_cats, ref_cats])
+
+        else:
+            categories = curr_cats
+
+        cats = categories.sort_values(ascending=False).index.drop_duplicates(keep="first")[:max_categories].values
+
+        result_current = current_data.apply(lambda x: x if str(x) in cats else "other")
+        result_reference = None
+        if reference_data is not None:
+            result_reference = reference_data.apply(lambda x: x if str(x) in cats else "other")
+        return result_current, result_reference
+    else:
+        return current_data.copy(), reference_data.copy() if reference_data is not None else None
+
 
-            return bins_for_hist
-        if feature_type == "cat":
-            return make_hist_for_cat_plot(curr_data, ref_data, dropna=True)
-        if feature_type == "datetime":
-            freq = self._choose_agg_period(feature_name, ref, curr)
-            curr_data = curr[feature_name].dt.to_period(freq=freq)
-            curr_data = curr_data.value_counts().reset_index()
-            curr_data.columns = [feature_name, "number_of_items"]
-            curr_data[feature_name] = curr_data[feature_name].dt.to_timestamp()
-            reference = None
-            if ref is not None:
-                ref_data = ref[feature_name].dt.to_period(freq=freq)
-                ref_data = ref_data.value_counts().reset_index()
-                ref_data.columns = [feature_name, "number_of_items"]
-                ref_data[feature_name] = ref_data[feature_name].dt.to_timestamp()
-                max_ref_date = ref_data[feature_name].max()
-                min_curr_date = curr_data[feature_name].min()
-                if max_ref_date == min_curr_date:
-                    curr_data, ref_data = self._split_periods(curr_data, ref_data, feature_name)
-                reference = ref_data
-                reference.columns = ["x", "count"]
-            curr_data.columns = ["x", "count"]
-            return Histogram(current=HistogramData.from_df(curr_data), reference=HistogramData.from_df(reference))
-        if feature_type == "text":
-            return None
-
-        raise ValueError(f"Unknown feature type {feature_type}")
-
-    def calculate_data_in_time(
-        self,
-        curr: pd.DataFrame,
-        ref: Optional[pd.DataFrame],
-        feature_name: str,
-        feature_type: str,
-        datetime_name: str,
-        merge_small_cat: Optional[int] = MAX_CATEGORIES,
+def _split_periods(curr_data: pd.DataFrame, ref_data: pd.DataFrame, feature_name: str):
+    max_ref_date = ref_data[feature_name].max()
+    min_curr_date = curr_data[feature_name].min()
+
+    if (
+        curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"].iloc[0]
+        > ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"].iloc[0]
     ):
-        result = None
-        if feature_type == "cat" and merge_small_cat is not None:
-            if ref is not None:
-                ref = ref.copy()
-            curr, ref = self._transform_cat_data(curr.copy(), ref, feature_name, merge_small_cat)
-
-        freq = self._choose_agg_period(datetime_name, ref, curr)
-        df_for_time_plot_curr = (
-            curr.assign(period=lambda x: x[datetime_name].dt.to_period(freq=freq))
-            .loc[:, ["period", feature_name]]
-            .copy()
+        curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"] = (
+            curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"]
+            + ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"]
+        )
+        ref_data = ref_data[ref_data[feature_name] != max_ref_date]
+    else:
+        ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"] = (
+            ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"]
+            + curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"]
         )
+        curr_data = curr_data[curr_data[feature_name] != min_curr_date]
+    return curr_data, ref_data
+
+
+def _choose_agg_period(
+    current_date_column: pd.Series,
+    reference_date_column: Optional[pd.Series],
+) -> Tuple[str, str]:
+    optimal_points = 150
+    prefix_dict = {
+        "A": "year",
+        "Q": "quarter",
+        "M": "month",
+        "W": "week",
+        "D": "day",
+        "H": "hour",
+    }
+    datetime_feature = current_date_column
+    if reference_date_column is not None:
+        datetime_feature = datetime_feature.append(reference_date_column)
+    days = (datetime_feature.max() - datetime_feature.min()).days
+    time_points = pd.Series(
+        index=["A", "Q", "M", "W", "D", "H"],
+        data=[
+            abs(optimal_points - days / 365),
+            abs(optimal_points - days / 90),
+            abs(optimal_points - days / 30),
+            abs(optimal_points - days / 7),
+            abs(optimal_points - days),
+            abs(optimal_points - days * 24),
+        ],
+    )
+    period_prefix = prefix_dict[time_points.idxmin()]
+    return period_prefix, str(time_points.idxmin())
+
+
+def prepare_data_for_plots(
+    current_data: pd.Series,
+    reference_data: Optional[pd.Series],
+    column_type: ColumnType,
+    max_categories: Optional[int] = MAX_CATEGORIES,
+) -> Tuple[pd.Series, Optional[pd.Series]]:
+    if column_type == ColumnType.Categorical:
+        current_data, reference_data = _relabel_data(current_data, reference_data, max_categories)
+    else:
+        current_data = current_data.copy()
+        if reference_data is not None:
+            reference_data = reference_data.copy()
+    return current_data, reference_data
+
+
+def _transform_df_to_time_mean_view(
+    period_data: pd.Series,
+    datetime_column_name: str,
+    datetime_data: pd.Series,
+    data_column_name: str,
+    column_data: pd.Series,
+):
+    df = pd.DataFrame({"period": period_data, data_column_name: column_data, datetime_column_name: datetime_data})
+    df = df.groupby("period")[datetime_column_name].mean().reset_index()
+    df[datetime_data] = df["period"].dt.to_timestamp()
+    return df
+
+
+def _transform_df_to_time_count_view(
+    period_data: pd.Series,
+    datetime_column_name: str,
+    datetime_data: pd.Series,
+    data_column_name: str,
+    column_data: pd.Series,
+):
+    df = pd.DataFrame({"period": period_data, datetime_column_name: datetime_data, data_column_name: column_data})
+    df = df.groupby(["period", data_column_name]).size()
+    df.name = "num"
+    df = df.reset_index()
+    df[datetime_column_name] = df["period"].dt.to_timestamp()
+    return df[df["num"] > 0]
+
+
+Data = Tuple[str, ColumnType, pd.Series, Optional[pd.Series]]
+
+
+def _prepare_box_data(
+    curr: pd.DataFrame,
+    ref: Optional[pd.DataFrame],
+    cat_feature_name: str,
+    num_feature_name: str,
+) -> Dict[str, Dict[str, list]]:
+    dfs = [curr]
+    names = ["current"]
+    if ref is not None:
+        dfs.append(ref)
+        names.append("reference")
+    res = {}
+    for df, name in zip(dfs, names):
+        df_for_plot = df.groupby(cat_feature_name)[num_feature_name].quantile([0, 0.25, 0.5, 0.75, 1]).reset_index()
+        df_for_plot.columns = [cat_feature_name, "q", num_feature_name]
+        res_df = {}
+        values = df_for_plot[cat_feature_name].unique()
+
+        def _quantiles(qdf, value):
+            return qdf[df_for_plot.q == value].set_index(cat_feature_name).loc[values, num_feature_name].tolist()
+
+        res_df["mins"] = _quantiles(df_for_plot, 0)
+        res_df["lowers"] = _quantiles(df_for_plot, 0.25)
+        res_df["means"] = _quantiles(df_for_plot, 0.5)
+        res_df["uppers"] = _quantiles(df_for_plot, 0.75)
+        res_df["maxs"] = _quantiles(df_for_plot, 1)
+        res_df["values"] = values
+        res[name] = res_df
+    return res
+
+
+def _get_count_values(column_data: pd.Series, target_data: pd.Series, target_name: str, column_name: str):
+    df = pd.DataFrame({target_name: target_data, column_name: column_data})
+    df = df.groupby([target_name, column_name]).size()
+    df.name = "count_objects"
+    df = df.reset_index()
+    return df[df["count_objects"] > 0]
+
+
+def plot_data(
+    data: Data,
+    datetime_data: Optional[Data],
+    target_data: Optional[Data],
+    merge_small_categories: Optional[int] = MAX_CATEGORIES,
+) -> Tuple[Optional[Histogram], Optional[Dict[str, Collection[str]]], Optional[Dict[str, Collection[str]]]]:
+    """
+    Args:
+        data: Column data includes column name current and reference data (if present)
+        datetime_data: Datetime data if present
+        target_data: Target data if present
+        merge_small_categories: Maximum of labels in categorical data what should be shown
+    Returns:
+        Histogram data or None
+        TODO: add reason why should be returned None
+    """
+    column_name, column_type, current_data, reference_data = data
+    if column_type == ColumnType.Categorical:
+        current_data, reference_data = _relabel_data(current_data, reference_data, merge_small_categories)
+    else:
+        current_data = current_data.copy()
+        if reference_data is not None:
+            reference_data = reference_data.copy()
+    current_data.dropna(inplace=True)
+    if reference_data is not None:
+        reference_data.dropna(inplace=True)
+
+    data_hist = None
+    if column_type == ColumnType.Numerical:
+        data_hist = make_hist_for_num_plot(current_data, reference_data, calculate_log=True)
+    elif column_type == ColumnType.Categorical:
+        data_hist = make_hist_for_cat_plot(current_data, reference_data, dropna=True)
+    elif column_type == ColumnType.Datetime:
+        prefix, freq = _choose_agg_period(current_data, reference_data)
+        curr_data = current_data.dt.to_period(freq=freq).value_counts().reset_index()
+        curr_data.columns = ["x", "number_of_items"]
+        curr_data["x"] = curr_data["x"].dt.to_timestamp()
+        reference = None
+        if reference_data is not None:
+            ref_data = reference_data.dt.to_period(freq=freq).value_counts().reset_index()
+            ref_data.columns = ["x", "number_of_items"]
+            ref_data["x"] = ref_data["x"].dt.to_timestamp()
+            max_ref_date = ref_data["x"].max()
+            min_curr_date = curr_data["x"].min()
+            if max_ref_date == min_curr_date:
+                curr_data, ref_data = _split_periods(curr_data, ref_data, "x")
+            reference = ref_data
+            reference.columns = ["x", "count"]
+        curr_data.columns = ["x", "count"]
+        data_hist = Histogram(current=HistogramData.from_df(curr_data), reference=HistogramData.from_df(reference))
+    elif column_type == ColumnType.Text:
+        data_hist = None
+    else:
+        raise ValueError(f"Unsupported column type {column_type}")
+
+    data_in_time = None
+    if datetime_data is not None:
+        datetime_name, _, datetime_current, datetime_reference = datetime_data
+        prefix, freq = _choose_agg_period(datetime_current, datetime_reference)
+        current_period_data = datetime_current.dt.to_period(freq=freq)
         df_for_time_plot_ref = None
-        if ref is not None:
-            df_for_time_plot_ref = (
-                ref.assign(period=lambda x: x[datetime_name].dt.to_period(freq=freq))
-                .loc[:, ["period", feature_name]]
-                .copy()
-            )
-        if feature_type == "num":
-            df_for_time_plot_curr = self._transform_df_to_time_mean_view(
-                df_for_time_plot_curr,
+        reference_period_data = None
+        if reference_data is not None and datetime_reference is not None:
+            reference_period_data = datetime_reference.dt.to_period(freq=freq)
+        if column_type == ColumnType.Numerical:
+            df_for_time_plot_curr = _transform_df_to_time_mean_view(
+                current_period_data,
                 datetime_name,
-                feature_name,
+                datetime_current,
+                column_name,
+                current_data,
             )
-            if df_for_time_plot_ref is not None:
-                df_for_time_plot_ref = self._transform_df_to_time_mean_view(
-                    df_for_time_plot_ref,
+            if reference_period_data is not None:
+                df_for_time_plot_ref = _transform_df_to_time_mean_view(
+                    reference_period_data,
                     datetime_name,
-                    feature_name,
+                    datetime_reference,
+                    column_name,
+                    reference_data,
                 )
-            result = {
-                "current": df_for_time_plot_curr,
-                "reference": df_for_time_plot_ref,
-                "freq": self.period_prefix,
+            data_in_time = {
+                "data_for_plots": {
+                    "current": df_for_time_plot_curr,
+                    "reference": df_for_time_plot_ref,
+                },
+                "freq": prefix,
                 "datetime_name": datetime_name,
             }
 
-        if feature_type == "cat":
-            df_for_time_plot_curr = self._transform_df_to_time_count_view(
-                df_for_time_plot_curr,
+        if column_type == ColumnType.Categorical:
+            df_for_time_plot_curr = _transform_df_to_time_count_view(
+                current_period_data,
                 datetime_name,
-                feature_name,
+                datetime_current,
+                column_name,
+                current_data,
             )
-            if df_for_time_plot_ref is not None:
-                df_for_time_plot_ref = self._transform_df_to_time_count_view(
-                    df_for_time_plot_ref,
+            if reference_period_data is not None:
+                df_for_time_plot_ref = _transform_df_to_time_count_view(
+                    reference_period_data,
                     datetime_name,
-                    feature_name,
+                    datetime_reference,
+                    column_name,
+                    reference_data,
                 )
-            result = {
-                "current": df_for_time_plot_curr,
-                "reference": df_for_time_plot_ref,
-                "freq": self.period_prefix,
+            data_in_time = {
+                "data_for_plots": {
+                    "current": df_for_time_plot_curr,
+                    "reference": df_for_time_plot_ref,
+                },
+                "freq": prefix,
                 "datetime_name": datetime_name,
             }
 
-        return result
-
-    def calculate_data_by_target(
-        self,
-        curr: pd.DataFrame,
-        ref: Optional[pd.DataFrame],
-        feature_name: str,
-        feature_type: str,
-        target_name: str,
-        target_type: str,
-        merge_small_cat: Optional[int] = MAX_CATEGORIES,
-    ):
-        if feature_type == "cat" and target_type == "num":
-            if ref is not None:
-                ref = ref.copy()
-            if merge_small_cat is not None:
-                curr, ref = self._transform_cat_data(curr.copy(), ref, feature_name, merge_small_cat)
-            return self._prepare_box_data(curr, ref, feature_name, target_name)
-        if feature_type == "num" and target_type == "cat":
-            if ref is not None:
-                ref = ref.copy()
-            if merge_small_cat is not None:
-                curr, ref = self._transform_cat_data(curr.copy(), ref, target_name, merge_small_cat)
-            return self._prepare_box_data(curr, ref, target_name, feature_name)
-        if feature_type == "num" and target_type == "num":
-            result = {}
-            result["current"] = {
-                feature_name: curr[feature_name].tolist(),
-                target_name: curr[target_name].tolist(),
+    data_by_target = None
+    if target_data is not None:
+        target_name, target_type, target_current, target_reference = target_data
+        curr_df = pd.DataFrame({column_name: current_data, target_name: target_current})
+        ref_df = None
+        if target_reference is not None and reference_data is not None:
+            ref_df = pd.DataFrame({column_name: reference_data, target_name: target_reference})
+        if column_type == ColumnType.Categorical and target_type == ColumnType.Numerical:
+            data_by_target = {
+                "data_for_plots": _prepare_box_data(curr_df, ref_df, column_name, target_name),
+                "target_name": target_name,
+                "target_type": target_type.value,
+            }
+        if column_type == ColumnType.Numerical and target_type == ColumnType.Categorical:
+            data_by_target = {
+                "data_for_plots": _prepare_box_data(curr_df, ref_df, target_name, column_name),
+                "target_name": target_name,
+                "target_type": target_type.value,
+            }
+        if column_type == ColumnType.Numerical and target_type == ColumnType.Numerical:
+            result = {
+                "current": {
+                    column_name: current_data.tolist(),
+                    target_name: target_current.tolist(),
+                }
             }
-            if ref is not None:
+            if reference_data is not None and target_reference is not None:
                 result["reference"] = {
-                    feature_name: ref[feature_name].tolist(),
-                    target_name: ref[target_name].tolist(),
+                    column_name: reference_data.tolist(),
+                    target_name: target_reference.tolist(),
                 }
-            return result
-        if feature_type == "cat" and target_type == "cat":
-            if ref is not None:
-                ref = ref.copy()
-            if merge_small_cat is not None:
-                curr, ref = self._transform_cat_data(curr.copy(), ref, feature_name, merge_small_cat)
-            if ref is not None:
-                ref = ref.copy()
-            if merge_small_cat is not None:
-                curr, ref = self._transform_cat_data(curr.copy(), ref, target_name, merge_small_cat, True)
-            result = {}
-            result["current"] = self._get_count_values(curr, target_name, feature_name)
-            if ref is not None:
-                result["reference"] = self._get_count_values(ref, target_name, feature_name)
-            return result
-        return None
-
-    def _split_periods(self, curr_data, ref_data, feature_name):
-        max_ref_date = ref_data[feature_name].max()
-        min_curr_date = curr_data[feature_name].min()
-
-        if (
-            curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"].iloc[0]
-            > ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"].iloc[0]
-        ):
-            curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"] = (
-                curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"]
-                + ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"]
-            )
-            ref_data = ref_data[ref_data[feature_name] != max_ref_date]
-        else:
-            ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"] = (
-                ref_data.loc[ref_data[feature_name] == max_ref_date, "number_of_items"]
-                + curr_data.loc[curr_data[feature_name] == min_curr_date, "number_of_items"]
-            )
-            curr_data = curr_data[curr_data[feature_name] != min_curr_date]
-        return curr_data, ref_data
-
-    def _get_count_values(self, df: pd.DataFrame, target_column: str, feature_name: Optional[str]):
-        df = df.groupby([target_column, feature_name]).size()
-        df.name = "count_objects"
-        df = df.reset_index()
-        return df[df["count_objects"] > 0]
-
-    def _prepare_box_data(
-        self, curr: pd.DataFrame, ref: Optional[pd.DataFrame], cat_feature_name: str, num_feature_name: str
-    ) -> Dict[str, Dict[str, list]]:
-        dfs = [curr]
-        names = ["current"]
-        if ref is not None:
-            dfs.append(ref)
-            names.append("reference")
-        res = {}
-        for df, name in zip(dfs, names):
-            df_for_plot = df.groupby(cat_feature_name)[num_feature_name].quantile([0, 0.25, 0.5, 0.75, 1]).reset_index()
-            df_for_plot.columns = [cat_feature_name, "q", num_feature_name]
-            res_df = {}
-            values = df_for_plot[cat_feature_name].unique()
-
-            def _quantiles(qdf, value):
-                return qdf[df_for_plot.q == value].set_index(cat_feature_name).loc[values, num_feature_name].tolist()
-
-            res_df["mins"] = _quantiles(df_for_plot, 0)
-            res_df["lowers"] = _quantiles(df_for_plot, 0.25)
-            res_df["means"] = _quantiles(df_for_plot, 0.5)
-            res_df["uppers"] = _quantiles(df_for_plot, 0.75)
-            res_df["maxs"] = _quantiles(df_for_plot, 1)
-            res_df["values"] = values
-            res[name] = res_df
-        return res
-
-    def _transform_cat_data(
-        self,
-        curr: pd.DataFrame,
-        ref: Optional[pd.DataFrame],
-        feature_name: str,
-        merge_small_cat: int,
-        rewrite: bool = False,
-    ) -> Tuple[pd.DataFrame, Optional[pd.DataFrame]]:
-        if self.curr is not None and rewrite is not True:
-            return self.curr, self.ref
-        if ref is not None:
-            unique_values = len(
-                np.union1d(
-                    curr[feature_name].astype(str).unique(),
-                    ref[feature_name].astype(str).unique(),
-                )
-            )
-        else:
-            unique_values = curr[feature_name].astype(str).nunique()
-
-        if unique_values > merge_small_cat:
-            curr_cats = curr[feature_name].astype(str).value_counts(normalize=True)
-
-            if ref is not None:
-                ref_cats = ref[feature_name].astype(str).value_counts(normalize=True)
-                categories = pd.concat([curr_cats, ref_cats])
-
-            else:
-                categories = curr_cats
-
-            cats = categories.sort_values(ascending=False).index.drop_duplicates(keep="first")[:merge_small_cat].values
-
-            curr[feature_name] = curr[feature_name].apply(lambda x: x if str(x) in cats else "other")
-            if ref is not None:
-                ref[feature_name] = ref[feature_name].apply(lambda x: x if str(x) in cats else "other")
-            self.curr = curr
-            self.ref = ref
-        return curr, ref
-
-    def _choose_agg_period(
-        self, date_column: str, reference_data: Optional[pd.DataFrame], current_data: pd.DataFrame
-    ) -> str:
-        optimal_points = 150
-        prefix_dict = {
-            "A": "year",
-            "Q": "quarter",
-            "M": "month",
-            "W": "week",
-            "D": "day",
-            "H": "hour",
-        }
-        datetime_feature = current_data[date_column]
-        if reference_data is not None:
-            datetime_feature = datetime_feature.append(reference_data[date_column])
-        days = (datetime_feature.max() - datetime_feature.min()).days
-        time_points = pd.Series(
-            index=["A", "Q", "M", "W", "D", "H"],
-            data=[
-                abs(optimal_points - days / 365),
-                abs(optimal_points - days / 90),
-                abs(optimal_points - days / 30),
-                abs(optimal_points - days / 7),
-                abs(optimal_points - days),
-                abs(optimal_points - days * 24),
-            ],
-        )
-        self.period_prefix = prefix_dict[time_points.idxmin()]
-        return str(time_points.idxmin())
+            data_by_target = {
+                "data_for_plots": result,
+                "target_name": target_name,
+                "target_type": target_type.value,
+            }
+        if column_type == ColumnType.Categorical and target_type == ColumnType.Categorical:
+            result = {"current": _get_count_values(current_data, target_current, target_name, column_name)}
+            if target_reference is not None and reference_data is not None:
+                result["reference"] = _get_count_values(reference_data, target_reference, target_name, column_name)
+            data_by_target = {
+                "data_for_plots": result,
+                "target_name": target_name,
+                "target_type": target_type.value,
+            }
 
-    def _transform_df_to_time_mean_view(self, df: pd.DataFrame, date_column: str, feature_name: str):
-        df = df.groupby("period")[feature_name].mean().reset_index()
-        df[date_column] = df["period"].dt.to_timestamp()
-        return df
-
-    def _transform_df_to_time_count_view(self, df: pd.DataFrame, date_column: str, feature_name: str):
-        df = df.groupby(["period", feature_name]).size()
-        df.name = "num"
-        df = df.reset_index()
-        df[date_column] = df["period"].dt.to_timestamp()
-        return df[df["num"] > 0]
+    return data_hist, data_in_time, data_by_target
 
 
 def _select_features_for_corr(dataset: pd.DataFrame, data_definition: DataDefinition) -> tuple:
     """Define which features should be used for calculating correlation matrices:
         - for pearson, spearman, and kendall correlation matrices we select numerical features which have > 1
             unique values;
         - for kramer_v correlation matrix, we select categorical features which have > 1 unique values.
     Args:
-        columns: all columns data information.
+        dataset: data for processing
+        data_definition: definition for all columns in data
     Returns:
         num_for_corr: list of feature names for pearson, spearman, and kendall correlation matrices.
         cat_for_corr: list of feature names for kramer_v correlation matrix.
     """
 
     num = data_definition.get_columns("numerical_columns")
     cat = data_definition.get_columns("categorical_columns")
```

### Comparing `evidently-0.3.0/src/evidently/calculations/regression_performance.py` & `evidently-0.3.1/src/evidently/calculations/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/__init__.py` & `evidently-0.3.1/src/evidently/calculations/stattests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 from .psi import psi_stat_test
 from .registry import PossibleStatTestType
 from .registry import StatTest
 from .registry import StatTestFuncType
 from .registry import get_stattest
 from .registry import register_stattest
 from .t_test import t_test
-from .text_content_drift import text_content_drift_stat_test
+from .text_content_drift import perc_text_content_drift_stat_test
+from .text_content_drift_abs import abs_text_content_drift_stat_test
 from .tvd_stattest import tvd_test
 from .wasserstein_distance_norm import wasserstein_stat_test
 from .z_stattest import z_stat_test
```

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/anderson_darling_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/anderson_darling_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/chisquare_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/chisquare_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/energy_distance.py` & `evidently-0.3.1/src/evidently/calculations/stattests/energy_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/epps_singleton_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/epps_singleton_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/fisher_exact_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/fisher_exact_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/g_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/g_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/hellinger_distance.py` & `evidently-0.3.1/src/evidently/calculations/stattests/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/jensenshannon.py` & `evidently-0.3.1/src/evidently/calculations/stattests/jensenshannon.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/kl_div.py` & `evidently-0.3.1/src/evidently/calculations/stattests/kl_div.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/ks_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/ks_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/mmd_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/mmd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/psi.py` & `evidently-0.3.1/src/evidently/calculations/stattests/psi.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/registry.py` & `evidently-0.3.1/src/evidently/calculations/stattests/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,17 @@
     _registered_stat_tests[stat_test.name] = {ft: stat_test for ft in stat_test.allowed_feature_types}
     _registered_stat_test_funcs[stat_test.func] = stat_test.name
 
 
 def _get_default_stattest(reference_data: pd.Series, current_data: pd.Series, feature_type: str) -> StatTest:
     n_values = pd.concat([reference_data, current_data]).nunique()
     if feature_type == "text":
-        return stattests.text_content_drift_stat_test
+        if reference_data.shape[0] > 1000:
+            return stattests.abs_text_content_drift_stat_test
+        return stattests.perc_text_content_drift_stat_test
     elif reference_data.shape[0] <= 1000:
         if feature_type == "num":
             if n_values <= 5:
                 return stattests.chi_stat_test if n_values > 2 else stattests.z_stat_test
             elif n_values > 5:
                 return stattests.ks_stat_test
         elif feature_type == "cat":
```

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/t_test.py` & `evidently-0.3.1/src/evidently/calculations/stattests/t_test.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/text_content_drift.py` & `evidently-0.3.1/src/evidently/calculations/stattests/text_content_drift.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import pandas as pd
 
 from evidently.calculations.stattests.registry import StatTest
 from evidently.calculations.stattests.registry import register_stattest
 from evidently.utils.data_drift_utils import calculate_text_drift_score
 
 
-def _text_content_drift(
+def _perc_text_content_drift(
     reference_data: pd.Series, current_data: pd.Series, feature_type: str, threshold: float
 ) -> Tuple[float, bool]:
-    return calculate_text_drift_score(reference_data, current_data, p_value=threshold)
+    return calculate_text_drift_score(reference_data, current_data, bootstrap=True, p_value=1 - threshold)
 
 
-text_content_drift_stat_test = StatTest(
-    name="text_content_drift",
-    display_name="Text content drift",
-    func=_text_content_drift,
+perc_text_content_drift_stat_test = StatTest(
+    name="perc_text_content_drift",
+    display_name="Percentile text content drift",
+    func=_perc_text_content_drift,
     allowed_feature_types=["text"],
-    default_threshold=0.05,
+    default_threshold=0.95,
 )
 
-register_stattest(text_content_drift_stat_test)
+register_stattest(perc_text_content_drift_stat_test)
```

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/tvd_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/tvd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/utils.py` & `evidently-0.3.1/src/evidently/calculations/stattests/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/wasserstein_distance_norm.py` & `evidently-0.3.1/src/evidently/calculations/stattests/wasserstein_distance_norm.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/stattests/z_stattest.py` & `evidently-0.3.1/src/evidently/calculations/stattests/z_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/calculations/utils.py` & `evidently-0.3.1/src/evidently/calculations/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/core.py` & `evidently-0.3.1/src/evidently/core.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/descriptors/non_letter_character_percentage_descriptor.py` & `evidently-0.3.1/src/evidently/descriptors/non_letter_character_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/descriptors/oov_words_percentage_descriptor.py` & `evidently-0.3.1/src/evidently/descriptors/oov_words_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/descriptors/trigger_words_presence_descriptor.py` & `evidently-0.3.1/src/evidently/descriptors/trigger_words_presence_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/features/OOV_words_percentage_feature.py` & `evidently-0.3.1/src/evidently/features/OOV_words_percentage_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/features/generated_features.py` & `evidently-0.3.1/src/evidently/features/generated_features.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/features/non_letter_character_percentage_feature.py` & `evidently-0.3.1/src/evidently/features/non_letter_character_percentage_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/features/text_length_feature.py` & `evidently-0.3.1/src/evidently/features/text_length_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/features/trigger_words_presence_feature.py` & `evidently-0.3.1/src/evidently/features/trigger_words_presence_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metric_preset/classification_performance.py` & `evidently-0.3.1/src/evidently/metric_preset/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metric_preset/data_quality.py` & `evidently-0.3.1/src/evidently/metric_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metric_preset/regression_performance.py` & `evidently-0.3.1/src/evidently/metric_preset/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metric_preset/target_drift.py` & `evidently-0.3.1/src/evidently/metric_preset/target_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metric_preset/text_overview.py` & `evidently-0.3.1/src/evidently/metric_preset/text_overview.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metric_results.py` & `evidently-0.3.1/src/evidently/metric_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Tuple
+from typing import Type
+from typing import TypeVar
 from typing import Union
+from typing import overload
 
 import numpy as np
 import pandas as pd
+from typing_extensions import Literal
 
 from evidently.base_metric import MetricResult
 from evidently.core import IncludeTags
 from evidently.pipeline.column_mapping import TargetNames
 
 Label = Union[int, str]
 ScatterData = Union[pd.Series, List[float], pd.Index]
@@ -238,17 +243,15 @@
         tags = {IncludeTags.Render}
 
     x: pd.Series
     count: pd.Series
     name: Optional[str] = None
 
     @classmethod
-    def from_df(cls, value: Optional[pd.DataFrame]):
-        if value is None:
-            return None
+    def from_df(cls, value: pd.DataFrame):
         return cls(x=value["x"], count=value["count"])
 
     @classmethod
     def from_distribution(cls, dist: Optional[Distribution], name: str = None):
         if dist is None:
             return None
         return cls(x=pd.Series(dist.x), count=pd.Series(dist.y), name=name)
@@ -290,7 +293,43 @@
     log_loss: Optional[float] = None
     tpr: Optional[float] = None
     tnr: Optional[float] = None
     fpr: Optional[float] = None
     fnr: Optional[float] = None
     rate_plots_data: Optional[RatesPlotData] = None
     plot_data: Optional[Boxes] = None
+
+
+TR = TypeVar("TR")
+TA = TypeVar("TA")
+
+
+@overload
+def raw_agg_properties(field_name, raw_type: Type[TR], agg_type: Type[TA], optional: Literal[False]) -> Tuple[TR, TA]:
+    ...
+
+
+@overload
+def raw_agg_properties(
+    field_name, raw_type: Type[TR], agg_type: Type[TA], optional: Literal[True]
+) -> Tuple[Optional[TR], Optional[TA]]:
+    ...
+
+
+def raw_agg_properties(field_name, raw_type: Type[TR], agg_type: Type[TA], optional: bool) -> Tuple[TR, TA]:
+    def property_raw(self):
+        val = getattr(self, field_name)
+        if optional and val is None:
+            return None
+        if not isinstance(val, raw_type):
+            raise ValueError("Raw data not available")
+        return val
+
+    def property_agg(self):
+        val = getattr(self, field_name)
+        if optional and val is None:
+            return None
+        if not isinstance(val, agg_type):
+            raise ValueError("Agg data not available")
+        return val
+
+    return property(property_raw), property(property_agg)  # type: ignore[return-value]
```

### Comparing `evidently-0.3.0/src/evidently/metrics/__init__.py` & `evidently-0.3.1/src/evidently/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/base_metric.py` & `evidently-0.3.1/src/evidently/metrics/base_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/base_classification_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/base_classification_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/class_balance_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/class_balance_metric.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Union
 
-import pandas as pd
-
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.metric_results import Histogram
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
@@ -32,15 +31,19 @@
         prediction_name = dataset_columns.utility_columns.prediction
         if target_name is None or prediction_name is None:
             raise ValueError("The columns 'target' and 'prediction' columns should be present")
         curr_target = data.current_data[target_name]
         ref_target = None
         if data.reference_data is not None:
             ref_target = data.reference_data[target_name]
-        target_names = dataset_columns.target_names
+        target_names: Optional[Dict[Union[int, str], str]]
+        if isinstance(dataset_columns.target_names, list):
+            target_names = {idx: str(val) for idx, val in enumerate(dataset_columns.target_names)}
+        else:
+            target_names = dataset_columns.target_names
         if target_names is not None:
             curr_target = curr_target.map(target_names)
             if ref_target is not None:
                 ref_target = ref_target.map(target_names)
 
         plot_data = make_hist_for_cat_plot(curr_target, ref_target)
```

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/class_separation_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/class_separation_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/classification_dummy_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/classification_dummy_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from sklearn.metrics import classification_report
 from sklearn.metrics import log_loss
 from sklearn.metrics import precision_score
 from sklearn.metrics import recall_score
 
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import calculate_matrix
@@ -117,24 +116,25 @@
 
             else:
                 coeff_recall = min(1.0, 0.5 / (1 - threshold))
 
             coeff_precision = min(1.0, (1 - threshold) / 0.5)
             neg_label_precision = precision_score(target, dummy_preds, pos_label=labels[1]) * coeff_precision
             neg_label_recall = recall_score(target, dummy_preds, pos_label=labels[1]) * coeff_recall
+            f1_label2_value = 2 * neg_label_precision * neg_label_recall / (neg_label_precision + neg_label_recall)
             metrics_matrix = {
                 str(labels[0]): ClassMetric(
                     precision=current_dummy.precision,
                     recall=current_dummy.recall,
-                    f1=current_dummy.f1,
+                    **{"f1-score": current_dummy.f1},
                 ),
                 str(labels[1]): ClassMetric(
                     precision=neg_label_precision,
                     recall=neg_label_recall,
-                    f1=2 * neg_label_precision * neg_label_recall / (neg_label_precision + neg_label_recall),
+                    **{"f1-score": f1_label2_value},
                 ),
             }
         if prediction is not None and prediction.prediction_probas is not None:
             # dummy log_loss and roc_auc
             binaraized_target = (target.astype(str).values.reshape(-1, 1) == list(labels)).astype(int)
             dummy_prediction = np.full(
                 prediction.prediction_probas.shape,
```

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/classification_quality_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/classification_quality_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/confusion_matrix_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/confusion_matrix_metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import dataclasses
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import calculate_matrix
 from evidently.metric_results import ConfusionMatrix
 from evidently.metrics.classification_performance.base_classification_metric import ThresholdClassificationMetric
 from evidently.model.widget import BaseWidgetInfo
+from evidently.pipeline.column_mapping import TargetNames
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.renderers.html_widgets import plotly_figure
 from evidently.utils.visualizations import plot_conf_mtrx
 
 DEFAULT_THRESHOLD = 0.5
 
 
 class ClassificationConfusionMatrixResult(MetricResult):
     current_matrix: ConfusionMatrix
     reference_matrix: Optional[ConfusionMatrix]
-    target_names: Optional[Dict[Union[str, int], str]] = None
+    target_names: Optional[TargetNames] = None
 
 
 class ClassificationConfusionMatrix(ThresholdClassificationMetric[ClassificationConfusionMatrixResult]):
     probas_threshold: Optional[float]
     k: Optional[Union[float, int]]
 
     def __init__(self, probas_threshold: Optional[float] = None, k: Optional[Union[float, int]] = None):
@@ -58,15 +58,19 @@
         )
 
 
 @default_renderer(wrap_type=ClassificationConfusionMatrix)
 class ClassificationConfusionMatrixRenderer(MetricRenderer):
     def render_html(self, obj: ClassificationConfusionMatrix) -> List[BaseWidgetInfo]:
         metric_result = obj.get_result()
-        target_names = metric_result.target_names
+        target_names: Optional[Dict[Union[int, str], str]]
+        if isinstance(metric_result.target_names, list):
+            target_names = {idx: str(item) for idx, item in enumerate(metric_result.target_names)}
+        else:
+            target_names = metric_result.target_names
         curr_matrix = metric_result.current_matrix
         ref_matrix = metric_result.reference_matrix
         if target_names is not None:
             curr_matrix.labels = [target_names[x] for x in curr_matrix.labels]
             if ref_matrix is not None:
                 ref_matrix.labels = [target_names[x] for x in ref_matrix.labels]
```

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/objects.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/objects.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/pr_curve_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/pr_curve_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/pr_table_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/pr_table_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/probability_distribution_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/probability_distribution_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_class_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/quality_by_class_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/quality_by_feature_table.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/quality_by_feature_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import dataclasses
 import json
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Union
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.classification_performance import get_prediction_data
+from evidently.features.generated_features import FeatureDescriptor
+from evidently.features.generated_features import GeneratedFeature
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
-from evidently.metric_results import PredictionData
 from evidently.metric_results import StatsByFeature
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import header_text
 from evidently.utils.data_operations import process_columns
@@ -35,44 +34,45 @@
 
     target_name: str
     columns: List[str]
 
 
 class ClassificationQualityByFeatureTable(Metric[ClassificationQualityByFeatureTableResults]):
     columns: Optional[List[str]]
-    text_features_gen: Optional[
-        Dict[
-            str,
-            Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]],
-        ]
-    ]
+    descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]]
+    text_features_gen: Optional[Dict[str, Dict[str, GeneratedFeature]]]
 
-    def __init__(self, columns: Optional[List[str]] = None):
+    def __init__(
+        self,
+        columns: Optional[List[str]] = None,
+        descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]] = None,
+    ):
         self.columns = columns
         self.text_features_gen = None
+        self.descriptors = descriptors
 
     def required_features(self, data_definition: DataDefinition):
         if len(data_definition.get_columns("text_features")) > 0:
             text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
             text_features_gen = {}
             text_features_gen_result = []
             for col in text_cols:
-                col_dict: Dict[
-                    str,
-                    Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage],
-                ] = {}
-                col_dict[f"{col}: Text Length"] = TextLength(col)
-                col_dict[f"{col}: Non Letter Character %"] = NonLetterCharacterPercentage(col)
-                col_dict[f"{col}: OOV %"] = OOVWordsPercentage(col)
-
-                text_features_gen_result += [
-                    col_dict[f"{col}: Text Length"],
-                    col_dict[f"{col}: Non Letter Character %"],
-                    col_dict[f"{col}: OOV %"],
-                ]
+                if self.columns is not None and col not in self.columns:
+                    continue
+                if self.descriptors is None or col not in self.descriptors:
+                    col_dict = {
+                        f"{col}: Text Length": TextLength(col),
+                        f"{col}: Non Letter Character %": NonLetterCharacterPercentage(col),
+                        f"{col}: OOV %": OOVWordsPercentage(col),
+                    }
+                else:
+                    column_descriptors = self.descriptors[col]
+                    col_dict = {f"{col}: " + name: value.feature(col) for name, value in column_descriptors.items()}
+
+                text_features_gen_result += list(col_dict.values())
                 text_features_gen[col] = col_dict
             self.text_features_gen = text_features_gen
 
             return text_features_gen_result
         else:
             return []
 
@@ -108,50 +108,31 @@
                         + dataset_columns.cat_feature_names
                         + dataset_columns.text_feature_names
                     ),
                 )
             )
 
         # process text columns
-        if (
-            self.text_features_gen is not None
-            and len(np.intersect1d(list(self.text_features_gen.keys()), columns)) >= 1
-        ):
-            for col in np.intersect1d(list(self.text_features_gen.keys()), columns):
-                columns += list(self.text_features_gen[col].keys())
-                columns.remove(col)
-                curr_text_df = pd.concat(
-                    [data.get_current_column(x.feature_name()) for x in list(self.text_features_gen[col].values())],
-                    axis=1,
-                )
-                curr_text_df.columns = list(self.text_features_gen[col].keys())
-                curr_df = pd.concat(
-                    [
-                        curr_df.reset_index(drop=True),
-                        curr_text_df.reset_index(drop=True),
-                    ],
-                    axis=1,
-                )
+
+        if self.text_features_gen is not None:
+            for column, features in self.text_features_gen.items():
+                columns.remove(column)
+                columns += list(features.keys())
+                curr_text_df = pd.concat([data.get_current_column(x.feature_name()) for x in features.values()], axis=1)
+                curr_text_df.columns = list(features.keys())
+                curr_df = pd.concat([curr_df.reset_index(drop=True), curr_text_df.reset_index(drop=True)], axis=1)
 
                 if ref_df is not None:
                     ref_text_df = pd.concat(
-                        [
-                            data.get_reference_column(x.feature_name())
-                            for x in list(self.text_features_gen[col].values())
-                        ],
-                        axis=1,
-                    )
-                    ref_text_df.columns = list(self.text_features_gen[col].keys())
-                    ref_df = pd.concat(
-                        [
-                            ref_df.reset_index(drop=True),
-                            ref_text_df.reset_index(drop=True),
-                        ],
+                        [data.get_reference_column(x.feature_name()) for x in features.values()],
                         axis=1,
                     )
+                    ref_text_df.columns = list(features.keys())
+                    ref_df = pd.concat([ref_df.reset_index(drop=True), ref_text_df.reset_index(drop=True)], axis=1)
+
         table_columns = columns + [target_name]
         if isinstance(prediction_name, str):
             table_columns += [prediction_name]
         if isinstance(prediction_name, list):
             table_columns += prediction_name
         reference = None
         if ref_df is not None:
@@ -178,15 +159,18 @@
         reference_data = result.reference.plot_data if result.reference is not None else None
         target_name = result.target_name
         curr_predictions = result.current.predictions
         # todo: better typing?
         assert curr_predictions is not None
         ref_predictions = result.reference.predictions if result.reference is not None else None
         columns = result.columns
-        labels = curr_predictions.labels
+        if ref_predictions is not None:
+            labels = np.union1d(curr_predictions.labels, ref_predictions.labels).tolist()
+        else:
+            labels = curr_predictions.labels
 
         color_options = self.color_options
 
         current_data["prediction_labels"] = curr_predictions.predictions.values
 
         if reference_data is not None and ref_predictions is not None:
             reference_data["prediction_labels"] = ref_predictions.predictions.values
```

### Comparing `evidently-0.3.0/src/evidently/metrics/classification_performance/roc_curve_metric.py` & `evidently-0.3.1/src/evidently/metrics/classification_performance/roc_curve_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/column_drift_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/column_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/column_value_plot.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/column_value_plot.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/data_drift_table.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/data_drift_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     dataset_drift: bool
     drift_by_columns: Dict[str, ColumnDataDriftMetrics]
     dataset_columns: DatasetColumns
 
 
 class DataDriftTable(Metric[DataDriftTableResults]):
     columns: Optional[List[str]]
-    options: DataDriftOptions
+    drift_options: DataDriftOptions
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         stattest: Optional[PossibleStatTestType] = None,
         cat_stattest: Optional[PossibleStatTestType] = None,
         num_stattest: Optional[PossibleStatTestType] = None,
@@ -53,39 +53,39 @@
         stattest_threshold: Optional[float] = None,
         cat_stattest_threshold: Optional[float] = None,
         num_stattest_threshold: Optional[float] = None,
         text_stattest_threshold: Optional[float] = None,
         per_column_stattest_threshold: Optional[Dict[str, float]] = None,
     ):
         self.columns = columns
-        self.options = DataDriftOptions(
+        self.drift_options = DataDriftOptions(
             all_features_stattest=stattest,
             cat_features_stattest=cat_stattest,
             num_features_stattest=num_stattest,
             text_features_stattest=text_stattest,
             per_feature_stattest=per_column_stattest,
             all_features_threshold=stattest_threshold,
             cat_features_threshold=cat_stattest_threshold,
             num_features_threshold=num_stattest_threshold,
             text_features_threshold=text_stattest_threshold,
             per_feature_threshold=per_column_stattest_threshold,
         )
 
     def get_parameters(self) -> tuple:
-        return None if self.columns is None else tuple(self.columns), self.options
+        return None if self.columns is None else tuple(self.columns), self.drift_options
 
     def calculate(self, data: InputData) -> DataDriftTableResults:
         if data.reference_data is None:
             raise ValueError("Reference dataset should be present")
 
         dataset_columns = process_columns(data.reference_data, data.column_mapping)
         result = get_drift_for_columns(
             current_data=data.current_data,
             reference_data=data.reference_data,
-            data_drift_options=self.options,
+            data_drift_options=self.drift_options,
             dataset_columns=dataset_columns,
             columns=self.columns,
         )
         return DataDriftTableResults(
             number_of_columns=result.number_of_columns,
             number_of_drifted_columns=result.number_of_drifted_columns,
             share_of_drifted_columns=result.share_of_drifted_columns,
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/dataset_drift_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/dataset_drift_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     number_of_drifted_columns: int
     share_of_drifted_columns: float
     dataset_drift: bool
 
 
 class DatasetDriftMetric(Metric[DatasetDriftMetricResults]):
     columns: Optional[List[str]]
-    options: DataDriftOptions
+    drift_options: DataDriftOptions
     drift_share: float
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
         drift_share: float = 0.5,
         stattest: Optional[PossibleStatTestType] = None,
@@ -41,15 +41,15 @@
         stattest_threshold: Optional[float] = None,
         cat_stattest_threshold: Optional[float] = None,
         num_stattest_threshold: Optional[float] = None,
         text_stattest_threshold: Optional[float] = None,
         per_column_stattest_threshold: Optional[Dict[str, float]] = None,
     ):
         self.columns = columns
-        self.options = DataDriftOptions(
+        self.drift_options = DataDriftOptions(
             all_features_stattest=stattest,
             cat_features_stattest=cat_stattest,
             num_features_stattest=num_stattest,
             text_features_stattest=text_stattest,
             per_feature_stattest=per_column_stattest,
             all_features_threshold=stattest_threshold,
             cat_features_threshold=cat_stattest_threshold,
@@ -59,26 +59,26 @@
         )
         self.drift_share = drift_share
 
     def get_parameters(self) -> tuple:
         return (
             self.drift_share,
             None if self.columns is None else tuple(self.columns),
-            self.options,
+            self.drift_options,
         )
 
     def calculate(self, data: InputData) -> DatasetDriftMetricResults:
         if data.reference_data is None:
             raise ValueError("Reference dataset should be present")
 
         dataset_columns = process_columns(data.reference_data, data.column_mapping)
         result = get_drift_for_columns(
             current_data=data.current_data,
             reference_data=data.reference_data,
-            data_drift_options=self.options,
+            data_drift_options=self.drift_options,
             drift_share_threshold=self.drift_share,
             dataset_columns=dataset_columns,
             columns=self.columns,
         )
         return DatasetDriftMetricResults(
             drift_share=self.drift_share,
             number_of_columns=result.number_of_columns,
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/embedding_drift_methods.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/embedding_drift_methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,23 +42,23 @@
     return pd.DataFrame(pca.fit_transform(reference_emb)), pd.DataFrame(pca.transform(current_emb))
 
 
 def distance(
     dist: str = "euclidean",
     threshold: float = 0.2,
     bootstrap: Optional[bool] = None,
-    p_value: float = 0.05,
+    quantile_probability: float = 0.95,
     pca_components: Optional[int] = None,
 ) -> Callable:
     """Returns a function for calculating drift on embeddings using the average distance method with specified parameters
     Args:
         dist: "euclidean", "cosine", "cityblock" or "chebyshev"
         threshold: all values above this threshold means data drift. Applies when bootstrap != True
         bootstrap: boolean parameter to determine whether to apply statistical hypothesis testing
-        p_value: applies when bootstrap == True
+        quantile_probability: applies when bootstrap == True
         pca_components: number of components to keep
     Returns:
         func: a function for calculating drift, which takes in reference and current embeddings data
         and returns a tuple: drift score, whether there is drift, and the name of the drift calculation method.
     """
 
     def func(current_emb: pd.DataFrame, reference_emb: pd.DataFrame) -> Tuple[float, bool, str]:
@@ -76,15 +76,15 @@
                 b_ref_idx = np.random.choice(reference_emb.shape[0], b_ref_size)
                 b_curr_idx = np.random.choice(reference_emb.shape[0], b_curr_size)
                 bstrp_res.append(
                     DISTANCE_DICT[dist](
                         reference_emb.iloc[b_ref_idx, :].mean(axis=0), reference_emb.iloc[b_curr_idx, :].mean(axis=0)
                     )
                 )
-            perc = np.percentile(bstrp_res, 100 * (1 - p_value))
+            perc = np.percentile(bstrp_res, 100 * quantile_probability)
             return res, res > perc, "distance"
         return res, res > threshold, "distance"
 
     return func
 
 
 def calc_roc_auc_random(y_test, i):
@@ -95,22 +95,22 @@
     roc_auc_random = roc_auc_score(y_test, y_random_pred)
     return roc_auc_random
 
 
 def model(
     threshold: float = 0.55,
     bootstrap: Optional[bool] = None,
-    p_value: float = 0.05,
+    quantile_probability: float = 0.95,
     pca_components: Optional[int] = None,
 ) -> Callable:
     """Returns a function for calculating drift on embeddings using the classifier method with specified parameters
     Args:
         threshold: all values above this threshold means data drift. Applies when bootstrap != True
         bootstrap: boolean parameter to determine whether to apply statistical hypothesis testing
-        p_value: applies when bootstrap == True
+        quantile_probability: applies when bootstrap == True
         pca_components: number of components to keep
     Returns:
         func: a function for calculating drift, which takes in reference and current embeddings data
         and returns a tuple: drift score, whether there is drift, and the name of the drift calculation method.
     """
 
     def func(current_emb: pd.DataFrame, reference_emb: pd.DataFrame) -> Tuple[float, bool, str]:
@@ -125,15 +125,15 @@
         )
         clf = SGDClassifier(loss="log", random_state=42)
         clf.fit(X_train, y_train)
         y_pred_proba = clf.predict_proba(X_test)[:, 1]
         roc_auc = roc_auc_score(y_test, y_pred_proba)
         if bootstrap:
             roc_auc_values = [calc_roc_auc_random(y_test, i) for i in range(100)]
-            rand_roc_auc = np.percentile(roc_auc_values, 100 * (1 - p_value))
+            rand_roc_auc = np.percentile(roc_auc_values, 100 * quantile_probability)
             return roc_auc, roc_auc > rand_roc_auc, "model"
         return roc_auc, roc_auc > threshold, "model"
 
     return func
 
 
 def ratio(
@@ -197,22 +197,22 @@
         - 2.0 / (m * n) * Kxy.sum()
     )
 
 
 def mmd(
     threshold: float = 0.015,
     bootstrap: Optional[bool] = None,
-    p_value: float = 0.05,
+    quantile_probability: float = 0.05,
     pca_components: Optional[int] = None,
 ) -> Callable:
     """Returns a function for calculating drift on embeddings using the mmd method with specified parameters
     Args:
         threshold: all values above this threshold means data drift. Applies when bootstrap != True
         bootstrap: boolean parameter to determine whether to apply statistical hypothesis testing
-        p_value: applies when bootstrap == True
+        quantile_probability: applies when bootstrap == True
         pca_components: number of components to keep
     Returns:
         func: a function for calculating drift, which takes in reference and current embeddings data
         and returns a tuple: drift score, whether there is drift, and the name of the drift calculation method.
     """
 
     def func(current_emb: pd.DataFrame, reference_emb: pd.DataFrame) -> Tuple[float, bool, str]:
@@ -241,13 +241,13 @@
             y_size = int(m * n / (m + n))
             bstrp_res = []
             for i in range(N_BOOTSTRAP):
                 np.random.seed(i)
                 x_idxs = np.random.choice(m, x_size)
                 y_idxs = np.random.choice(m, y_size)
                 bstrp_res.append(MMD2u_bstrp(K, x_size, y_size, x_idxs, y_idxs))
-                perc = np.percentile(bstrp_res, 100 * (1 - p_value))
+                perc = np.percentile(bstrp_res, 100 * quantile_probability)
             return max(mmd2u, 0), mmd2u > perc, "mmd"
         else:
             return max(mmd2u, 0), mmd2u > threshold, "mmd"
 
     return func
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/embeddings_drift.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/embeddings_drift.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     drift_detected: bool
     method_name: str
     reference: np.ndarray
     current: np.ndarray
 
 
 class EmbeddingsDriftMetric(Metric[EmbeddingsDriftMetricResults]):
-    embeddings: str
+    embeddings_name: str
     drift_method: Optional[Callable]
 
     def __init__(
         self,
         embeddings_name: str,
         drift_method: Optional[Callable] = None,
     ):
@@ -66,23 +66,21 @@
         if self.embeddings_name not in emb_dict.keys():
             raise ValueError(f"{self.embeddings_name} not in column_mapping.embeddings")
         emb_list = emb_dict[self.embeddings_name]
         drift_score, drift_detected, method_name = self.drift_method(
             data.current_data[emb_list], data.reference_data[emb_list]
         )
         # visualisation
-        ref_sample = data.reference_data[emb_list].sample(
-            min(SAMPLE_CONSTANT, data.reference_data.shape[0]), random_state=24
-        )
-        curr_sample = data.current_data[emb_list].sample(
-            min(SAMPLE_CONSTANT, data.current_data.shape[0]), random_state=24
-        )
+        ref_sample_size = min(SAMPLE_CONSTANT, data.reference_data.shape[0])
+        curr_sample_size = min(SAMPLE_CONSTANT, data.current_data.shape[0])
+        ref_sample = data.reference_data[emb_list].sample(ref_sample_size, random_state=24)
+        curr_sample = data.current_data[emb_list].sample(curr_sample_size, random_state=24)
         data_2d = umap.UMAP().fit_transform(pd.concat([ref_sample, curr_sample]))
-        reference = get_gaussian_kde(data_2d[:SAMPLE_CONSTANT, 0], data_2d[:SAMPLE_CONSTANT, 1])
-        current = get_gaussian_kde(data_2d[SAMPLE_CONSTANT:, 0], data_2d[SAMPLE_CONSTANT:, 1])
+        reference = get_gaussian_kde(data_2d[:ref_sample_size, 0], data_2d[:ref_sample_size, 1])
+        current = get_gaussian_kde(data_2d[ref_sample_size:, 0], data_2d[ref_sample_size:, 1])
 
         return EmbeddingsDriftMetricResults(
             embeddings_name=self.embeddings_name,
             drift_score=drift_score,
             drift_detected=drift_detected,
             method_name=method_name,
             reference=reference,
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/target_by_features_table.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/target_by_features_table.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,26 +43,26 @@
     dataset_drift: bool
     drift_by_columns: Dict[str, ColumnDataDriftMetrics]
     dataset_columns: DatasetColumns
 
 
 class TextDescriptorsDriftMetric(Metric[TextDescriptorsDriftMetricResults]):
     column_name: str
-    options: DataDriftOptions
+    drift_options: DataDriftOptions
     generated_text_features: Dict[str, GeneratedFeature]
 
     def __init__(
         self,
         column_name: str,
         descriptors: Optional[Dict[str, FeatureDescriptor]] = None,
         stattest: Optional[PossibleStatTestType] = None,
         stattest_threshold: Optional[float] = None,
     ):
         self.column_name = column_name
-        self.options = DataDriftOptions(all_features_stattest=stattest, all_features_threshold=stattest_threshold)
+        self.drift_options = DataDriftOptions(all_features_stattest=stattest, all_features_threshold=stattest_threshold)
         if descriptors:
             self.descriptors = descriptors
         else:
             self.descriptors = {
                 "Text Length": TextLength(),
                 "Non Letter Character %": NonLetterCharacterPercentage(),
                 "OOV %": OOV(),
@@ -75,15 +75,15 @@
             self.generated_text_features = {
                 name: desc.feature(self.column_name) for name, desc in self.descriptors.items()
             }
             return list(self.generated_text_features.values())
         return []
 
     def get_parameters(self) -> tuple:
-        return self.column_name, self.options
+        return self.column_name, self.drift_options
 
     def calculate(self, data: InputData) -> TextDescriptorsDriftMetricResults:
         if data.reference_data is None:
             raise ValueError("Reference dataset should be present")
         curr_text_df = pd.concat(
             [data.get_current_column(x.feature_name()) for x in list(self.generated_text_features.values())],
             axis=1,
@@ -100,15 +100,15 @@
 
         drift_by_columns = {}
         for col in curr_text_df.columns:
             drift_by_columns[col] = get_one_column_drift(
                 current_data=curr_text_df,
                 reference_data=ref_text_df,
                 column_name=col,
-                options=self.options,
+                options=self.drift_options,
                 dataset_columns=text_dataset_columns,
             )
         dataset_drift = get_dataset_drift(drift_by_columns, 0)
 
         return TextDescriptorsDriftMetricResults(
             number_of_columns=curr_text_df.shape[1],
             number_of_drifted_columns=dataset_drift.number_of_drifted_columns,
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_integrity/column_missing_values_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_integrity/column_missing_values_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_integrity/column_regexp_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_integrity/column_regexp_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_integrity/column_summary_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_integrity/column_summary_metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from pandas.api.types import is_numeric_dtype
-from pandas.api.types import is_string_dtype
 
 from evidently.base_metric import ColumnMetric
 from evidently.base_metric import ColumnMetricResult
+from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import MetricResult
-from evidently.calculations.data_quality import DataQualityGetPlotData
 from evidently.calculations.data_quality import FeatureQualityStats
 from evidently.calculations.data_quality import get_features_stats
+from evidently.calculations.data_quality import plot_data
 from evidently.core import ColumnType
 from evidently.core import IncludeTags
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
 from evidently.metric_results import Histogram
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
-from evidently.utils.data_operations import process_columns
 from evidently.utils.data_preprocessing import DataDefinition
 from evidently.utils.types import Numeric
 from evidently.utils.visualizations import plot_boxes
 from evidently.utils.visualizations import plot_cat_cat_rel
 from evidently.utils.visualizations import plot_cat_feature_in_time
 from evidently.utils.visualizations import plot_distr
 from evidently.utils.visualizations import plot_distr_with_log_button
@@ -136,19 +134,25 @@
     current_characteristics: ColumnCharacteristics
     plot_data: DataQualityPlot
 
 
 class ColumnSummaryMetric(ColumnMetric[ColumnSummaryResult]):
     generated_text_features: Optional[Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]]]
 
-    def __init__(self, column_name: str):
-        self.column_name = column_name
+    def __init__(self, column_name: Union[str, ColumnName]):
+        if isinstance(column_name, str):
+            self.column = ColumnName.main_dataset(column_name)
+        else:
+            self.column = column_name
+        self.column_name = self.column.name
         self.generated_text_features = None
 
     def required_features(self, data_definition: DataDefinition):
+        if not self.column.is_main_dataset():
+            return ColumnMetric.required_features(self, data_definition)
         column_type = data_definition.get_column(self.column_name).column_type
         if column_type == ColumnType.Text:
             self.generated_text_features = {
                 "text_length": TextLength(self.column_name),
                 "non_letter_char": NonLetterCharacterPercentage(self.column_name),
                 "oov": OOVWordsPercentage(self.column_name),
             }
@@ -159,193 +163,103 @@
         return (self.column_name,)
 
     @staticmethod
     def acceptable_types() -> List[ColumnType]:
         return [ColumnType.Numerical, ColumnType.Categorical, ColumnType.Text]
 
     def calculate(self, data: InputData) -> ColumnSummaryResult:
-        columns = process_columns(data.current_data, data.column_mapping)
-
-        if self.column_name not in data.current_data:
-            raise ValueError(f"Column '{self.column_name}' not found in current dataset.")
 
-        if data.reference_data is not None and self.column_name not in data.reference_data:
-            raise ValueError(f"Column '{self.column_name}' not found in reference dataset.")
+        if not data.has_column(self.column):
+            raise ValueError(f"Column '{self.column.display_name}' not found in dataset.")
 
-        column_type = None
-        target_name = columns.utility_columns.target
-        target_type = None
-        data_by_target = None
-
-        # define target type and prediction type. TODO move it to process_columns func
-        if columns.utility_columns.target is not None:
-            reg_condition = data.column_mapping.task == "regression" or (
-                is_numeric_dtype(data.current_data[target_name])
-                and columns.task != "classification"
-                and data.current_data[target_name].nunique() > 5
-            )
-            if reg_condition:
-                target_type = "num"
-            else:
-                target_type = "cat"
-            if target_name == self.column_name:
-                column_type = target_type
-
-        if columns.utility_columns.prediction is not None:
-            if (
-                isinstance(columns.utility_columns.prediction, str)
-                and columns.utility_columns.prediction == self.column_name
-            ):
-                if (
-                    is_string_dtype(data.current_data[columns.utility_columns.prediction])
-                    or (
-                        is_numeric_dtype(data.current_data[columns.utility_columns.prediction])
-                        and columns.task != "classification"
-                        and data.current_data[columns.utility_columns.prediction].nunique() < 5
-                    )
-                    or (
-                        is_numeric_dtype(data.current_data[columns.utility_columns.prediction])
-                        and columns.task == "classification"
-                        and (
-                            data.current_data[columns.utility_columns.prediction].max() > 1
-                            or data.current_data[columns.utility_columns.prediction].min() < 0
-                        )
-                    )
-                ):
-                    column_type = "cat"
-                else:
-                    column_type = "num"
-
-            if (
-                isinstance(columns.utility_columns.prediction, list)
-                and self.column_name in columns.utility_columns.prediction
-            ):
-                column_type = "num"
-        if self.column_name in columns.num_feature_names:
-            column_type = "num"
-        elif self.column_name in columns.cat_feature_names:
-            column_type = "cat"
-        elif self.column_name in columns.datetime_feature_names or (
-            columns.utility_columns.date is not None and columns.utility_columns.date == self.column_name
-        ):
-            column_type = "datetime"
-        elif self.column_name in columns.text_feature_names:
-            column_type = "text"
-        if column_type is None:
-            raise ValueError(f"column {self.column_name} not in num, cat, text or datetime features lists")
+        column_type, column_current_data, column_reference_data = data.get_data(self.column)
 
         curr_characteristics: ColumnCharacteristics
-        reference_data = None
         ref_characteristics: Optional[ColumnCharacteristics] = None
-        if column_type == "text" and self.generated_text_features is not None:
-            if data.reference_data is not None:
+        if column_type == ColumnType.Text and self.generated_text_features is not None:
+            if column_reference_data is not None:
                 ref_characteristics = self.get_text_stats(
                     "reference",
                     data,
-                    data.reference_data[self.column_name],
+                    column_reference_data,
                     self.generated_text_features,
                 )
             curr_characteristics = self.get_text_stats(
                 "current",
                 data,
-                data.current_data[self.column_name],
+                column_current_data,
                 self.generated_text_features,
             )
         else:
-            if data.reference_data is not None:
-                reference_data = data.reference_data
-                ref_characteristics = self.map_data(
-                    get_features_stats(data.reference_data[self.column_name], column_type)
-                )
-            curr_characteristics = self.map_data(get_features_stats(data.current_data[self.column_name], column_type))
-
-            if data.reference_data is not None and column_type == "cat":
-                current_values_set = set(data.current_data[self.column_name].unique())
-                reference_values_set = set(data.reference_data[self.column_name].unique())
+            if column_reference_data is not None:
+                ref_characteristics = self.map_data(get_features_stats(column_reference_data, column_type))
+            curr_characteristics = self.map_data(get_features_stats(column_current_data, column_type))
+
+            if column_reference_data is not None and column_type == ColumnType.Categorical:
+                current_values_set = set(column_current_data.unique())
+                reference_values_set = set(column_reference_data.unique())
                 unique_in_current = current_values_set - reference_values_set
                 new_in_current_values_count: int = len(unique_in_current)
                 unique_in_reference = reference_values_set - current_values_set
                 unused_in_current_values_count: int = len(unique_in_reference)
                 if any(pd.isnull(list(unique_in_current))) and any(pd.isnull(list(unique_in_reference))):
                     new_in_current_values_count -= 1
                     unused_in_current_values_count -= 1
                 if not isinstance(curr_characteristics, CategoricalCharacteristics):
                     raise ValueError(f"{self.column_name} should be categorical")
                 curr_characteristics.new_in_current_values_count = new_in_current_values_count
                 curr_characteristics.unused_in_current_values_count = unused_in_current_values_count
 
-        # plot data
-        gpd = DataQualityGetPlotData()
-        bins_for_hist = gpd.calculate_main_plot(data.current_data, reference_data, self.column_name, column_type)
-        data_in_time = None
+        datetime_column = data.data_definition.get_datetime_column()
+        datetime_data = None
         if (
-            columns.utility_columns.date is not None
-            and columns.utility_columns.date != self.column_name
-            and column_type != "datetime"
+            datetime_column is not None
+            and datetime_column.column_name != self.column.name
+            and column_type != ColumnType.Datetime
         ):
-            data_in_time = gpd.calculate_data_in_time(
-                data.current_data,
-                reference_data,
-                self.column_name,
-                column_type,
-                columns.utility_columns.date,
-            )
-            data_in_time = DataInTime(
-                data_for_plots={
-                    "current": data_in_time["current"],
-                    "reference": data_in_time["reference"],
-                },
-                freq=data_in_time["freq"],
-                datetime_name=data_in_time["datetime_name"],
-            )
+            datetime_type, datetime_current, datetime_reference = data.get_data(datetime_column.column_name)
+            datetime_data = (datetime_column.column_name, datetime_type, datetime_current, datetime_reference)
 
+        target_column = data.data_definition.get_target_column()
+        target_data = None
         if (
-            target_name is not None
-            and target_type is not None
-            and columns.utility_columns.target != self.column_name
-            and column_type != "datetime"
+            target_column is not None
+            and target_column.column_name != self.column.name
+            and column_type != ColumnType.Datetime
         ):
+            target_type, target_current, target_reference = data.get_data(target_column.column_name)
+            target_data = (target_column.column_name, target_type, target_current, target_reference)
+        bins_for_hist, data_in_time, data_by_target = plot_data(
+            (self.column.display_name, column_type, column_current_data, column_reference_data),
+            datetime_data,
+            target_data,
+        )
 
-            data_for_plots = gpd.calculate_data_by_target(
-                data.current_data,
-                reference_data,
-                self.column_name,
-                column_type,
-                target_name,
-                target_type,
-            )
-            data_by_target = DataByTarget(
-                data_for_plots=data_for_plots,
-                target_name=target_name,
-                target_type=target_type,
-            )
         counts_of_values = None
-        if column_type in ["cat", "num"]:
+        if column_type in [ColumnType.Categorical, ColumnType.Numerical]:
             counts_of_values = {}
-            current_counts = data.current_data[self.column_name].value_counts(dropna=False).reset_index()
+            current_counts = column_current_data.value_counts(dropna=False).reset_index()
             current_counts.columns = ["x", "count"]
             counts_of_values["current"] = current_counts.head(10)
-            if data.reference_data is not None:
-                reference_counts = data.reference_data[self.column_name].value_counts(dropna=False).reset_index()
+            if column_reference_data is not None:
+                reference_counts = column_reference_data.value_counts(dropna=False).reset_index()
                 reference_counts.columns = ["x", "count"]
                 counts_of_values["reference"] = reference_counts.head(10)
 
-        plot_data = DataQualityPlot(
-            bins_for_hist=bins_for_hist,
-            data_in_time=data_in_time,
-            data_by_target=data_by_target,
-            counts_of_values=counts_of_values,
-        )
-
         return ColumnSummaryResult(
             column_name=self.column_name,
-            column_type=column_type,
+            column_type=column_type.value,
             reference_characteristics=ref_characteristics,
             current_characteristics=curr_characteristics,
-            plot_data=plot_data,
+            plot_data=DataQualityPlot(
+                bins_for_hist=bins_for_hist,
+                data_in_time=data_in_time,
+                data_by_target=data_by_target,
+                counts_of_values=counts_of_values,
+            ),
         )
 
     @staticmethod
     def map_data(stats: FeatureQualityStats) -> ColumnCharacteristics:
         if stats.feature_type == "num":
             if isinstance(stats.max, str) or isinstance(stats.min, str) or isinstance(stats.most_common_value, str):
                 raise ValueError("max / min stats should be int or float type, but got str")
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_integrity/dataset_summary_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_integrity/dataset_summary_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/column_correlations_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/column_correlations_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/column_distribution_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/column_distribution_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/column_quantile_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/column_quantile_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List
 from typing import Optional
+from typing import Union
 
 import pandas as pd
 
 from evidently.base_metric import ColumnMetricResult
+from evidently.base_metric import ColumnName
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import ColumnType
 from evidently.metric_results import Distribution
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
@@ -34,43 +36,41 @@
     current: QuantileStats
     reference: Optional[QuantileStats] = None
 
 
 class ColumnQuantileMetric(Metric[ColumnQuantileMetricResult]):
     """Calculates quantile with specified range"""
 
-    column_name: str
+    column: ColumnName
     quantile: float
 
-    def __init__(self, column_name: str, quantile: float) -> None:
+    def __init__(self, column_name: Union[str, ColumnName], quantile: float) -> None:
         self.quantile = quantile
-        self.column_name = column_name
+        if isinstance(column_name, str):
+            self.column = ColumnName.main_dataset(column_name)
+        else:
+            self.column = column_name
 
     def calculate(self, data: InputData) -> ColumnQuantileMetricResult:
         if not 0 < self.quantile <= 1:
             raise ValueError("Quantile should all be in the interval (0, 1].")
 
-        if self.column_name not in data.current_data:
-            raise ValueError(f"Column '{self.column_name}' is not in current data.")
+        if not data.has_column(self.column):
+            raise ValueError(f"Column '{self.column}' is not in data.")
 
-        current_column = data.current_data[self.column_name]
+        column_type, current_column, reference_column = data.get_data(self.column)
 
         if not pd.api.types.is_numeric_dtype(current_column.dtype):
-            raise ValueError(f"Column '{self.column_name}' in current data is not numeric.")
-
-        current_quantile = data.current_data[self.column_name].quantile(self.quantile)
-
-        if data.reference_data is not None:
-            if self.column_name not in data.reference_data:
-                raise ValueError(f"Column '{self.column_name}' is not in reference data.")
+            raise ValueError(f"Column '{self.column}' in current data is not numeric.")
 
-            reference_column = data.reference_data[self.column_name]
+        current_quantile = current_column.quantile(self.quantile)
 
+        if reference_column is not None:
             if not pd.api.types.is_numeric_dtype(reference_column.dtype):
-                raise ValueError(f"Column '{self.column_name}' in reference data is not numeric.")
+                raise ValueError(f"Column '{self.column}' in reference data is not numeric.")
 
             reference_quantile = reference_column.quantile(self.quantile)
 
         else:
             reference_column = None
             reference_quantile = None
 
@@ -80,15 +80,15 @@
         reference = None
         if reference_quantile is not None:
             reference = QuantileStats(
                 value=reference_quantile,
                 distribution=distributions[1],
             )
         return ColumnQuantileMetricResult(
-            column_name=self.column_name,
+            column_name=self.column.display_name,
             column_type=ColumnType.Numerical.value,
             current=QuantileStats(
                 value=current_quantile,
                 distribution=distributions[0],
             ),
             quantile=self.quantile,
             reference=reference,
```

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/column_value_list_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/column_value_list_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/column_value_range_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/column_value_range_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/conflict_prediction_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/conflict_prediction_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/conflict_target_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/conflict_target_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/dataset_correlations_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/dataset_correlations_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/stability_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/stability_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/data_quality/text_descriptors_distribution.py` & `evidently-0.3.1/src/evidently/metrics/data_quality/text_descriptors_distribution.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/error_bias_table.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/error_bias_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import copy
 import json
 from typing import Dict
 from typing import List
 from typing import Optional
-from typing import Type
-from typing import Union
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.calculations.regression_performance import error_bias_table
 from evidently.calculations.regression_performance import error_with_quantiles
+from evidently.features.generated_features import FeatureDescriptor
+from evidently.features.generated_features import GeneratedFeature
 from evidently.features.non_letter_character_percentage_feature import NonLetterCharacterPercentage
 from evidently.features.OOV_words_percentage_feature import OOVWordsPercentage
 from evidently.features.text_length_feature import TextLength
 from evidently.model.widget import AdditionalGraphInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import default_renderer
@@ -48,50 +48,52 @@
 class RegressionErrorBiasTable(Metric[RegressionErrorBiasTableResults]):
     # by default, we get 5% values for the error bias calculations
     TOP_ERROR_DEFAULT = 0.05
     TOP_ERROR_MIN = 0
     TOP_ERROR_MAX = 0.5
     top_error: float
     columns: Optional[List[str]]
-    text_features_gen: Optional[
-        Dict[
-            str,
-            Dict[str, Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage]],
-        ]
-    ]
+    descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]]
+    text_features_gen: Optional[Dict[str, Dict[str, GeneratedFeature]]]
 
-    def __init__(self, columns: Optional[List[str]] = None, top_error: Optional[float] = None):
+    def __init__(
+        self,
+        columns: Optional[List[str]] = None,
+        top_error: Optional[float] = None,
+        descriptors: Optional[Dict[str, Dict[str, FeatureDescriptor]]] = None,
+    ):
         if top_error is None:
             self.top_error = self.TOP_ERROR_DEFAULT
 
         else:
             self.top_error = top_error
 
         self.columns = columns
         self.text_features_gen = None
+        self.descriptors = descriptors
 
     def required_features(self, data_definition: DataDefinition):
         if len(data_definition.get_columns("text_features")) > 0:
             text_cols = [col.column_name for col in data_definition.get_columns("text_features")]
             text_features_gen = {}
             text_features_gen_result = []
             for col in text_cols:
-                col_dict: Dict[
-                    str,
-                    Union[TextLength, NonLetterCharacterPercentage, OOVWordsPercentage],
-                ] = {}
-                col_dict[f"{col}: Text Length"] = TextLength(col)
-                col_dict[f"{col}: Non Letter Character %"] = NonLetterCharacterPercentage(col)
-                col_dict[f"{col}: OOV %"] = OOVWordsPercentage(col)
-
-                text_features_gen_result += [
-                    col_dict[f"{col}: Text Length"],
-                    col_dict[f"{col}: Non Letter Character %"],
-                    col_dict[f"{col}: OOV %"],
-                ]
+                if self.columns is not None and col not in self.columns:
+                    continue
+                if self.descriptors is None or col not in self.descriptors:
+                    col_dict = {
+                        f"{col}: Text Length": TextLength(col),
+                        f"{col}: Non Letter Character %": NonLetterCharacterPercentage(col),
+                        f"{col}: OOV %": OOVWordsPercentage(col),
+                    }
+                else:
+                    column_descriptors = self.descriptors[col]
+                    col_dict = {f"{col}: " + name: value.feature(col) for name, value in column_descriptors.items()}
+
+                text_features_gen_result += list(col_dict.values())
                 text_features_gen[col] = col_dict
             self.text_features_gen = text_features_gen
 
             return text_features_gen_result
         else:
             return []
 
@@ -129,51 +131,31 @@
 
         else:
             columns = self.columns
 
         num_feature_names = list(np.intersect1d(dataset_columns.num_feature_names, columns))
         cat_feature_names = list(np.intersect1d(dataset_columns.cat_feature_names, columns))
         # process text columns
-        if (
-            self.text_features_gen is not None
-            and len(np.intersect1d(list(self.text_features_gen.keys()), columns)) >= 1
-        ):
-            for col in np.intersect1d(list(self.text_features_gen.keys()), columns):
-                num_feature_names += list(self.text_features_gen[col].keys())
-                columns += list(self.text_features_gen[col].keys())
-                columns.remove(col)
-                curr_text_df = pd.concat(
-                    [data.get_current_column(x.feature_name()) for x in list(self.text_features_gen[col].values())],
-                    axis=1,
-                )
-                curr_text_df.columns = list(self.text_features_gen[col].keys())
-                curr_df = pd.concat(
-                    [
-                        curr_df.reset_index(drop=True),
-                        curr_text_df.reset_index(drop=True),
-                    ],
-                    axis=1,
-                )
+        if self.text_features_gen is not None:
+            for column, features in self.text_features_gen.items():
+                columns.remove(column)
+                num_feature_names += list(features.keys())
+                columns += list(features.keys())
+                curr_text_df = pd.concat([data.get_current_column(x.feature_name()) for x in features.values()], axis=1)
+                curr_text_df.columns = list(features.keys())
+                curr_df = pd.concat([curr_df.reset_index(drop=True), curr_text_df.reset_index(drop=True)], axis=1)
 
                 if ref_df is not None:
                     ref_text_df = pd.concat(
-                        [
-                            data.get_reference_column(x.feature_name())
-                            for x in list(self.text_features_gen[col].values())
-                        ],
-                        axis=1,
-                    )
-                    ref_text_df.columns = list(self.text_features_gen[col].keys())
-                    ref_df = pd.concat(
-                        [
-                            ref_df.reset_index(drop=True),
-                            ref_text_df.reset_index(drop=True),
-                        ],
+                        [data.get_reference_column(x.feature_name()) for x in features.values()],
                         axis=1,
                     )
+                    ref_text_df.columns = list(features.keys())
+                    ref_df = pd.concat([ref_df.reset_index(drop=True), ref_text_df.reset_index(drop=True)], axis=1)
+
         columns_ext = np.union1d(columns, [target_name, prediction_name])
         curr_df = self._make_df_for_plot(curr_df[columns_ext], target_name, prediction_name, None)
 
         if ref_df is not None:
             ref_df = self._make_df_for_plot(ref_df[columns_ext], target_name, prediction_name, None)
 
         err_quantiles = error_with_quantiles(curr_df, prediction_name, target_name, quantile=self.top_error)
```

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/error_distribution.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/error_distribution.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/error_in_time.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/error_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/error_normality.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/error_normality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/objects.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/objects.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/predicted_vs_actual.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/predicted_vs_actual.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/regression_dummy_metric.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/regression_dummy_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/regression_performance_metrics.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/regression_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/regression_quality.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/regression_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/top_error.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/top_error.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/utils.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/regression_performance/visualization.py` & `evidently-0.3.1/src/evidently/metrics/regression_performance/visualization.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/metrics/utils.py` & `evidently-0.3.1/src/evidently/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/model/widget.py` & `evidently-0.3.1/src/evidently/model/widget.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/nbextension/static/index.js` & `evidently-0.3.1/src/evidently/nbextension/static/index.js`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/nbextension/static/index.js.LICENSE.txt` & `evidently-0.3.1/src/evidently/nbextension/static/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/nbextension/static/material-ui-icons.woff2` & `evidently-0.3.1/src/evidently/nbextension/static/material-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/options/color_scheme.py` & `evidently-0.3.1/src/evidently/options/color_scheme.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from dataclasses import dataclass
 from typing import Optional
 from typing import Sequence
 
+from evidently.options.option import Option
+
 RED = "#ed0400"
 GREY = "#4d4d4d"
 COLOR_DISCRETE_SEQUENCE = (
     "#ed0400",
     "#0a5f38",
     "#6c3461",
     "#71aa34",
     "#d8dcd6",
     "#6b8ba4",
 )
 
 
-@dataclass
-class ColorOptions:
+class ColorOptions(Option):
     """Collection of colors for data visualization
 
     - primary_color - basic color for data visualization.
         Uses by default for all bars and lines for widgets with one dataset and as a default for current data.
     - secondary_color - basic color for second data visualization if we have two data sets, for example, reference data.
     - current_data_color - color for all current data, by default primary color is used
     - reference_data_color - color for reference data, by default secondary color is used
```

### Comparing `evidently-0.3.0/src/evidently/options/data_drift.py` & `evidently-0.3.1/src/evidently/options/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/options/quality_metrics.py` & `evidently-0.3.1/src/evidently/options/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/pipeline/column_mapping.py` & `evidently-0.3.1/src/evidently/pipeline/column_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class TaskType:
     REGRESSION_TASK: str = "regression"
     CLASSIFICATION_TASK: str = "classification"
 
 
-TargetNames = Union[List[int], List[str], Dict[int, str], Dict[str, str]]
+TargetNames = Union[List[Union[int, str]], Dict[Union[int, str], str]]
 Embeddings = Dict[str, List[str]]
 
 
 @dataclass
 class ColumnMapping:
     target: Optional[str] = "target"
     prediction: Optional[Union[str, int, Union[Sequence[str], Sequence[int]]]] = "prediction"
```

### Comparing `evidently-0.3.0/src/evidently/renderers/base_renderer.py` & `evidently-0.3.1/src/evidently/renderers/base_renderer.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/renderers/html_widgets.py` & `evidently-0.3.1/src/evidently/renderers/html_widgets.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/renderers/notebook_utils.py` & `evidently-0.3.1/src/evidently/renderers/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/renderers/render_utils.py` & `evidently-0.3.1/src/evidently/renderers/render_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/report/report.py` & `evidently-0.3.1/src/evidently/report/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.core import IncludeOptions
 from evidently.metric_preset.metric_preset import MetricPreset
 from evidently.metric_results import DatasetColumns
 from evidently.model.dashboard import DashboardInfo
 from evidently.model.widget import AdditionalGraphInfo
-from evidently.options import ColorOptions
+from evidently.options.base import AnyOptions
 from evidently.renderers.base_renderer import DetailsInfo
 from evidently.suite.base_suite import Display
 from evidently.suite.base_suite import Suite
 from evidently.suite.base_suite import find_metric_renderer
 from evidently.utils.data_operations import process_columns
 from evidently.utils.data_preprocessing import create_data_definition
 from evidently.utils.generators import BaseGenerator
@@ -28,27 +28,28 @@
 
 class Report(Display):
     _inner_suite: Suite
     _columns_info: DatasetColumns
     _first_level_metrics: List[Union[Metric]]
     metrics: List[Union[Metric, MetricPreset, BaseGenerator]]
 
-    def __init__(self, metrics: List[Union[Metric, MetricPreset, BaseGenerator]], options: Optional[List] = None):
+    def __init__(self, metrics: List[Union[Metric, MetricPreset, BaseGenerator]], options: AnyOptions = None):
         super().__init__(options)
         # just save all metrics and metric presets
         self.metrics = metrics
-        self._inner_suite = Suite()
+        self._inner_suite = Suite(self.options)
         self._first_level_metrics = []
 
     def run(
         self,
         *,
         reference_data: Optional[pd.DataFrame],
         current_data: pd.DataFrame,
         column_mapping: Optional[ColumnMapping] = None,
+        agg_data: bool = False,
     ) -> None:
         if column_mapping is None:
             column_mapping = ColumnMapping()
 
         if current_data is None:
             raise ValueError("Current dataset should be present")
 
@@ -100,21 +101,24 @@
             reference_data,
             current_data,
             ref_add,
             curr_add,
             column_mapping,
             data_definition,
         )
+        if agg_data:
+            self._inner_suite.context.options.agg_data = True
         self._inner_suite.run_calculate(data)
 
-    def as_dict(
+    def as_dict(  # type: ignore[override]
         self,
         include_render: bool = False,
         include: Dict[str, IncludeOptions] = None,
         exclude: Dict[str, IncludeOptions] = None,
+        **kwargs,
     ) -> dict:
         metrics = []
         include = include or {}
         exclude = exclude or {}
         for metric in self._first_level_metrics:
             renderer = find_metric_renderer(type(metric), self._inner_suite.context.renderers)
             metric_id = metric.get_id()
@@ -153,15 +157,15 @@
             raise ValueError(f"Metric group {group} not found in this report")
         return result[group]
 
     def _build_dashboard_info(self):
         metrics_results = []
         additional_graphs = []
 
-        color_options = self.options_provider.get(ColorOptions)
+        color_options = self.options.color_options
 
         for test in self._first_level_metrics:
             renderer = find_metric_renderer(type(test), self._inner_suite.context.renderers)
             # set the color scheme from the report for each render
             renderer.color_options = color_options
             html_info = renderer.render_html(test)
```

### Comparing `evidently-0.3.0/src/evidently/runner/loader.py` & `evidently-0.3.1/src/evidently/runner/loader.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/runner/runner.py` & `evidently-0.3.1/src/evidently/runner/runner.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/suite/base_suite.py` & `evidently-0.3.1/src/evidently/suite/base_suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 import copy
 import dataclasses
 import json
 import logging
 from datetime import datetime
 from typing import Dict
 from typing import Iterator
+from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import pandas as pd
 
 import evidently
 from evidently.base_metric import ErrorResult
 from evidently.base_metric import InputData
 from evidently.base_metric import Metric
 from evidently.base_metric import MetricResult
 from evidently.core import IncludeOptions
-from evidently.options import OptionsProvider
+from evidently.options.base import AnyOptions
+from evidently.options.base import Options
+from evidently.options.option import Option
 from evidently.renderers.base_renderer import DEFAULT_RENDERERS
 from evidently.renderers.base_renderer import MetricRenderer
 from evidently.renderers.base_renderer import RenderersDefinitions
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.notebook_utils import determine_template
 from evidently.suite.execution_graph import ExecutionGraph
 from evidently.suite.execution_graph import SimpleExecutionGraph
@@ -84,32 +87,27 @@
     execution_graph: Optional[ExecutionGraph]
     metrics: list
     tests: list
     metric_results: Dict[Metric, MetricResult]
     test_results: Dict[Test, TestResult]
     state: State
     renderers: RenderersDefinitions
+    options: Options = Options()
 
 
 class ExecutionError(Exception):
     pass
 
 
 class Display:
     # collection of all possible common options
-    options_provider: OptionsProvider
+    options: Options
 
-    def __init__(self, options: Optional[list] = None):
-        if options is None:
-            options = []
-
-        self.options_provider = OptionsProvider()
-
-        for option in options:
-            self.options_provider.add(option)
+    def __init__(self, options: AnyOptions = None):
+        self.options = Options.from_any_options(options)
 
     @abc.abstractmethod
     def _build_dashboard_info(self):
         raise NotImplementedError()
 
     def _repr_html_(self):
         dashboard_id, dashboard_info, graphs = self._build_dashboard_info()
@@ -168,39 +166,42 @@
 
     @abc.abstractmethod
     def as_dict(
         self,
         include_render: bool = False,
         include: Dict[str, IncludeOptions] = None,
         exclude: Dict[str, IncludeOptions] = None,
+        **kwargs,
     ) -> dict:
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def _get_json_content(
         self,
         include_render: bool = False,
         include: Dict[str, IncludeOptions] = None,
         exclude: Dict[str, IncludeOptions] = None,
+        **kwargs,
     ) -> dict:
         """Return all data for json representation"""
         result = {
             "version": evidently.__version__,
             "timestamp": str(datetime.now()),
         }
-        result.update(self.as_dict(include_render=include_render, include=include, exclude=exclude))
+        result.update(self.as_dict(include_render=include_render, include=include, exclude=exclude, **kwargs))
         return result
 
     def json(
         self,
         include_render: bool = False,
         include: Dict[str, IncludeOptions] = None,
         exclude: Dict[str, IncludeOptions] = None,
+        **kwargs,
     ) -> str:
         return json.dumps(
-            self._get_json_content(include_render=include_render, include=include, exclude=exclude),
+            self._get_json_content(include_render=include_render, include=include, exclude=exclude, **kwargs),
             cls=NumpyEncoder,
         )
 
     def save_json(
         self,
         filename,
         include_render: bool = False,
@@ -217,23 +218,24 @@
     def _render(self, temple_func, template_params: TemplateParams):
         return temple_func(params=template_params)
 
 
 class Suite:
     context: Context
 
-    def __init__(self):
+    def __init__(self, options: Options):
         self.context = Context(
             execution_graph=None,
             metrics=[],
             tests=[],
             metric_results={},
             test_results={},
             state=States.Init,
             renderers=DEFAULT_RENDERERS,
+            options=options,
         )
 
     def add_test(self, test: Test):
         test.set_context(self.context)
         for field_name, dependency in _discover_dependencies(test):
             if isinstance(dependency, Metric):
                 self.add_metric(dependency)
@@ -271,15 +273,15 @@
         features = {}
         if self.context.execution_graph is not None:
             execution_graph: ExecutionGraph = self.context.execution_graph
             for metric, calculation in execution_graph.get_metric_execution_iterator():
                 try:
                     required_features = metric.required_features(data_definition)
                 except Exception as e:
-                    logging.error(f"failed to get features for {type(metric)}: {e}")
+                    logging.error(f"failed to get features for {type(metric)}: {e}", exc_info=e)
                     continue
                 for feature in required_features:
                     params = feature.get_parameters()
                     if params is not None:
                         _id = (type(feature), params)
                         if _id in features:
                             continue
```

### Comparing `evidently-0.3.0/src/evidently/suite/execution_graph.py` & `evidently-0.3.1/src/evidently/suite/execution_graph.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/telemetry/sender.py` & `evidently-0.3.1/src/evidently/telemetry/sender.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/__init__.py` & `evidently-0.3.1/src/evidently/test_preset/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/classification_binary.py` & `evidently-0.3.1/src/evidently/test_preset/classification_binary.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/classification_binary_topk.py` & `evidently-0.3.1/src/evidently/test_preset/classification_binary_topk.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/classification_multiclass.py` & `evidently-0.3.1/src/evidently/test_preset/classification_multiclass.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/data_drift.py` & `evidently-0.3.1/src/evidently/test_preset/data_drift.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,41 @@
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
+import numpy as np
+
 from evidently import TaskType
 from evidently.base_metric import InputData
 from evidently.calculations.stattests import PossibleStatTestType
 from evidently.metric_results import DatasetColumns
 from evidently.test_preset.test_preset import TestPreset
 from evidently.tests import TestAllFeaturesValueDrift
 from evidently.tests import TestColumnDrift
+from evidently.tests import TestEmbeddingsDrift
 from evidently.tests import TestShareOfDriftedColumns
+from evidently.utils.data_drift_utils import add_emb_drift_to_reports
 from evidently.utils.data_drift_utils import resolve_stattest_threshold
 
 
 class DataDriftTestPreset(TestPreset):
     """
     Data Drift tests.
 
     Contains tests:
     - `TestShareOfDriftedColumns`
     - `TestColumnValueDrift`
     - `TestAllFeaturesValueDrift`
+    - 'TestEmbeddingsDrift'
     """
 
     columns: Optional[List[str]]
+    embeddings: Optional[List[str]]
+    embeddings_drift_method: Optional[Dict[str, Callable]]
     drift_share: Optional[float]
     stattest: Optional[PossibleStatTestType]
     cat_stattest: Optional[PossibleStatTestType]
     num_stattest: Optional[PossibleStatTestType]
     text_stattest: Optional[PossibleStatTestType]
     per_column_stattest: Optional[Dict[str, PossibleStatTestType]]
     stattest_threshold: Optional[float]
@@ -35,41 +43,57 @@
     num_stattest_threshold: Optional[float]
     text_stattest_threshold: Optional[float]
     per_column_stattest_threshold: Optional[Dict[str, float]]
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
+        embeddings: Optional[List[str]] = None,
+        embeddings_drift_method: Optional[Dict[str, Callable]] = None,
         drift_share: Optional[float] = None,
         stattest: Optional[PossibleStatTestType] = None,
         cat_stattest: Optional[PossibleStatTestType] = None,
         num_stattest: Optional[PossibleStatTestType] = None,
         text_stattest: Optional[PossibleStatTestType] = None,
         per_column_stattest: Optional[Dict[str, PossibleStatTestType]] = None,
         stattest_threshold: Optional[float] = None,
         cat_stattest_threshold: Optional[float] = None,
         num_stattest_threshold: Optional[float] = None,
         text_stattest_threshold: Optional[float] = None,
         per_column_stattest_threshold: Optional[Dict[str, float]] = None,
     ):
         super().__init__()
         self.columns = columns
+        self.embeddings = embeddings
+        self.embeddings_drift_method = embeddings_drift_method
         self.drift_share = drift_share
         self.stattest = stattest
         self.cat_stattest = cat_stattest
         self.num_stattest = num_stattest
         self.text_stattest = text_stattest
         self.per_column_stattest = per_column_stattest
         self.stattest_threshold = stattest_threshold
         self.cat_stattest_threshold = cat_stattest_threshold
         self.num_stattest_threshold = num_stattest_threshold
         self.text_stattest_threshold = text_stattest_threshold
         self.per_column_stattest_threshold = per_column_stattest_threshold
 
     def generate_tests(self, data: InputData, columns: DatasetColumns):
+        embeddings_data = data.column_mapping.embeddings
+        if embeddings_data is not None:
+            embs = list(set(v for values in embeddings_data.values() for v in values))
+            if self.columns is None:
+                self.columns = list(
+                    np.setdiff1d(
+                        columns.num_feature_names + columns.cat_feature_names + columns.text_feature_names, embs
+                    )
+                )
+            else:
+                self.columns = list(np.setdiff1d(self.columns, embs))
+
         preset_tests: list = [
             TestShareOfDriftedColumns(
                 columns=self.columns,
                 lt=0.3 if self.drift_share is None else self.drift_share,
                 stattest=self.stattest,
                 cat_stattest=self.cat_stattest,
                 num_stattest=self.num_stattest,
@@ -141,8 +165,17 @@
                 self.cat_stattest_threshold,
                 self.num_stattest_threshold,
                 self.text_stattest_threshold,
                 self.per_column_stattest_threshold,
             )
         )
 
+        if embeddings_data is None:
+            return preset_tests
+        preset_tests = add_emb_drift_to_reports(
+            preset_tests,
+            embeddings_data,
+            self.embeddings,
+            self.embeddings_drift_method,
+            TestEmbeddingsDrift,
+        )
         return preset_tests
```

### Comparing `evidently-0.3.0/src/evidently/test_preset/data_quality.py` & `evidently-0.3.1/src/evidently/test_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/data_stability.py` & `evidently-0.3.1/src/evidently/test_preset/data_stability.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_preset/no_target_performance.py` & `evidently-0.3.1/src/evidently/metric_preset/data_drift.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,111 @@
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 
-from evidently import TaskType
+import numpy as np
+
 from evidently.base_metric import InputData
 from evidently.calculations.stattests import PossibleStatTestType
+from evidently.metric_preset.metric_preset import MetricPreset
 from evidently.metric_results import DatasetColumns
-from evidently.test_preset.test_preset import TestPreset
-from evidently.tests import TestAllColumnsShareOfMissingValues
-from evidently.tests import TestCatColumnsOutOfListValues
-from evidently.tests import TestColumnDrift
-from evidently.tests import TestColumnsType
-from evidently.tests import TestNumColumnsMeanInNSigmas
-from evidently.tests import TestNumColumnsOutOfRangeValues
-from evidently.tests import TestShareOfDriftedColumns
-from evidently.utils.data_drift_utils import resolve_stattest_threshold
-
-
-class NoTargetPerformanceTestPreset(TestPreset):
-    """
-    No Target Performance tests.
+from evidently.metrics import DataDriftTable
+from evidently.metrics import DatasetDriftMetric
+from evidently.metrics import EmbeddingsDriftMetric
+from evidently.utils.data_drift_utils import add_emb_drift_to_reports
 
-    Args:
-        columns: list of columns include to tests
 
-    Contains tests:
-    - `TestColumnValueDrift`
-    - `TestShareOfDriftedColumns`
-    - `TestColumnsType`
-    - `TestAllColumnsShareOfMissingValues`
-    - `TestNumColumnsOutOfRangeValues`
-    - `TestCatColumnsOutOfListValues`
-    - `TestNumColumnsMeanInNSigmas`
-    - `TestCustomFeaturesValueDrift`
+class DataDriftPreset(MetricPreset):
+    """Metric Preset for Data Drift analysis.
+
+    Contains metrics:
+    - DatasetDriftMetric
+    - DataDriftTable
+    - EmbeddingsDriftMetric
     """
 
     columns: Optional[List[str]]
-    drift_share: Optional[float]
-    stattest: Optional[PossibleStatTestType] = None
-    cat_stattest: Optional[PossibleStatTestType] = None
-    num_stattest: Optional[PossibleStatTestType] = None
-    text_stattest: Optional[PossibleStatTestType] = None
-    per_column_stattest: Optional[Dict[str, PossibleStatTestType]] = None
-    stattest_threshold: Optional[float] = None
-    cat_stattest_threshold: Optional[float] = None
-    num_stattest_threshold: Optional[float] = None
-    text_stattest_threshold: Optional[float] = None
-    per_column_stattest_threshold: Optional[Dict[str, float]] = None
+    embeddings: Optional[List[str]]
+    embeddings_drift_method: Optional[Dict[str, Callable]]
+    drift_share: float
+    stattest: Optional[PossibleStatTestType]
+    cat_stattest: Optional[PossibleStatTestType]
+    num_stattest: Optional[PossibleStatTestType]
+    text_stattest: Optional[PossibleStatTestType]
+    per_column_stattest: Optional[Dict[str, PossibleStatTestType]]
+    stattest_threshold: Optional[float]
+    cat_stattest_threshold: Optional[float]
+    num_stattest_threshold: Optional[float]
+    text_stattest_threshold: Optional[float]
+    per_column_stattest_threshold: Optional[Dict[str, float]]
 
     def __init__(
         self,
         columns: Optional[List[str]] = None,
-        drift_share: Optional[float] = None,
+        embeddings: Optional[List[str]] = None,
+        embeddings_drift_method: Optional[Dict[str, Callable]] = None,
+        drift_share: float = 0.5,
         stattest: Optional[PossibleStatTestType] = None,
         cat_stattest: Optional[PossibleStatTestType] = None,
         num_stattest: Optional[PossibleStatTestType] = None,
         text_stattest: Optional[PossibleStatTestType] = None,
         per_column_stattest: Optional[Dict[str, PossibleStatTestType]] = None,
         stattest_threshold: Optional[float] = None,
         cat_stattest_threshold: Optional[float] = None,
         num_stattest_threshold: Optional[float] = None,
         text_stattest_threshold: Optional[float] = None,
         per_column_stattest_threshold: Optional[Dict[str, float]] = None,
     ):
         super().__init__()
         self.columns = columns
+        self.embeddings = embeddings
+        self.embeddings_drift_method = embeddings_drift_method
         self.drift_share = drift_share
         self.stattest = stattest
         self.cat_stattest = cat_stattest
         self.num_stattest = num_stattest
         self.text_stattest = text_stattest
         self.per_column_stattest = per_column_stattest
         self.stattest_threshold = stattest_threshold
         self.cat_stattest_threshold = cat_stattest_threshold
         self.num_stattest_threshold = num_stattest_threshold
         self.text_stattest_threshold = text_stattest_threshold
-        self.per_feature_threshold = per_column_stattest_threshold
+        self.per_column_stattest_threshold = per_column_stattest_threshold
 
-    def generate_tests(self, data: InputData, columns: DatasetColumns):
-        preset_tests: List = []
-
-        if columns.utility_columns.prediction is not None and isinstance(columns.utility_columns.prediction, str):
-            stattest, threshold = resolve_stattest_threshold(
-                columns.utility_columns.prediction,
-                "cat" if columns.task == TaskType.CLASSIFICATION_TASK else "num",
-                self.stattest,
-                self.cat_stattest,
-                self.num_stattest,
-                self.text_stattest,
-                self.per_column_stattest,
-                self.stattest_threshold,
-                self.cat_stattest_threshold,
-                self.num_stattest_threshold,
-                self.text_stattest_threshold,
-                self.per_column_stattest_threshold,
-            )
-            preset_tests.append(
-                TestColumnDrift(
-                    column_name=columns.utility_columns.prediction,
-                    stattest=stattest,
-                    stattest_threshold=threshold,
-                )
-            )
-        preset_tests.append(
-            TestShareOfDriftedColumns(
-                lt=0.3 if self.drift_share is None else self.drift_share,
+    def generate_metrics(self, data: InputData, columns: DatasetColumns):
+        result = [
+            DatasetDriftMetric(
+                columns=self.columns,
+                drift_share=self.drift_share,
                 stattest=self.stattest,
                 cat_stattest=self.cat_stattest,
                 num_stattest=self.num_stattest,
                 text_stattest=self.text_stattest,
                 per_column_stattest=self.per_column_stattest,
                 stattest_threshold=self.stattest_threshold,
                 cat_stattest_threshold=self.cat_stattest_threshold,
                 num_stattest_threshold=self.num_stattest_threshold,
                 text_stattest_threshold=self.text_stattest_threshold,
-                per_column_stattest_threshold=self.per_feature_threshold,
-            )
+                per_column_stattest_threshold=self.per_column_stattest_threshold,
+            ),
+            DataDriftTable(
+                columns=self.columns,
+                stattest=self.stattest,
+                cat_stattest=self.cat_stattest,
+                num_stattest=self.num_stattest,
+                text_stattest=self.text_stattest,
+                per_column_stattest=self.per_column_stattest,
+                stattest_threshold=self.stattest_threshold,
+                cat_stattest_threshold=self.cat_stattest_threshold,
+                num_stattest_threshold=self.num_stattest_threshold,
+                text_stattest_threshold=self.text_stattest_threshold,
+                per_column_stattest_threshold=self.per_column_stattest_threshold,
+            ),
+        ]
+        embeddings_data = data.column_mapping.embeddings
+        if embeddings_data is None:
+            return result
+        result = add_emb_drift_to_reports(
+            result, embeddings_data, self.embeddings, self.embeddings_drift_method, EmbeddingsDriftMetric
         )
-        preset_tests.append(TestColumnsType())
-        preset_tests.append(TestAllColumnsShareOfMissingValues(columns=self.columns))
-        preset_tests.append(TestNumColumnsOutOfRangeValues(columns=self.columns))
-        preset_tests.append(TestCatColumnsOutOfListValues(columns=self.columns))
-        preset_tests.append(TestNumColumnsMeanInNSigmas(columns=self.columns))
-
-        return preset_tests
+        return result
```

### Comparing `evidently-0.3.0/src/evidently/test_preset/regression.py` & `evidently-0.3.1/src/evidently/test_preset/regression.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/test_suite/test_suite.py` & `evidently-0.3.1/src/evidently/test_suite/test_suite.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from evidently.base_metric import InputData
 from evidently.core import IncludeOptions
 from evidently.metric_results import DatasetColumns
 from evidently.model.dashboard import DashboardInfo
 from evidently.model.widget import BaseWidgetInfo
 from evidently.options import ColorOptions
+from evidently.options.base import AnyOptions
+from evidently.options.base import Options
 from evidently.pipeline.column_mapping import ColumnMapping
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.suite.base_suite import Display
 from evidently.suite.base_suite import Suite
 from evidently.suite.base_suite import find_test_renderer
 from evidently.test_preset.test_preset import TestPreset
 from evidently.tests.base_test import DEFAULT_GROUP
@@ -34,18 +36,18 @@
     _columns_info: DatasetColumns
     _test_presets: List[TestPreset]
     _test_generators: List[BaseGenerator]
 
     def __init__(
         self,
         tests: Optional[List[Union[Test, TestPreset, BaseGenerator]]],
-        options: Optional[list] = None,
+        options: AnyOptions = None,
     ):
         super().__init__(options)
-        self._inner_suite = Suite()
+        self._inner_suite = Suite(self.options)
         self._test_presets = []
         self._test_generators = []
 
         for original_test in tests or []:
             if isinstance(original_test, TestPreset):
                 self._test_presets.append(original_test)
 
@@ -94,19 +96,31 @@
         self._inner_suite.verify()
         curr_add, ref_add = self._inner_suite.create_additional_features(current_data, reference_data, data_definition)
         data = InputData(reference_data, current_data, ref_add, curr_add, column_mapping, data_definition)
 
         self._inner_suite.run_calculate(data)
         self._inner_suite.run_checks()
 
-    def as_dict(
+    def json(  # type: ignore[override]
         self,
+        include_metrics: bool = False,
         include_render: bool = False,
         include: Dict[str, IncludeOptions] = None,
         exclude: Dict[str, IncludeOptions] = None,
+        **kwargs,
+    ) -> str:
+        return super().json(include_render, include, exclude, include_metrics=include_metrics)
+
+    def as_dict(  # type: ignore[override]
+        self,
+        include_metrics: bool = False,
+        include_render: bool = False,
+        include: Dict[str, IncludeOptions] = None,
+        exclude: Dict[str, IncludeOptions] = None,
+        **kwargs,
     ) -> dict:
         test_results = []
         include = include or {}
         exclude = exclude or {}
         counter = Counter(test_result.status for test_result in self._inner_suite.context.test_results.values())
 
         for test in self._inner_suite.context.test_results:
@@ -121,30 +135,40 @@
                 test_data = TestRenderer.render_json(renderer, test)
                 test_data["status"] = TestStatus.ERROR
                 test_data["description"] = f"Test failed with exception: {e}"
                 test_results.append(test_data)
 
         total_tests = len(self._inner_suite.context.test_results)
 
-        return {
+        result = {
             "tests": test_results,
             "summary": {
                 "all_passed": bool(self),
                 "total_tests": total_tests,
                 "success_tests": counter[TestStatus.SUCCESS] + counter[TestStatus.WARNING],
                 "failed_tests": counter[TestStatus.FAIL],
                 "by_status": {k.value: v for k, v in counter.items()},
             },
         }
+        if include_metrics:
+            from evidently.report import Report
+
+            report = Report([])
+            report._first_level_metrics = self._inner_suite.context.metrics
+            report._inner_suite.context = self._inner_suite.context
+            result["metric_results"] = report.as_dict(include_render=include_render, include=include, exclude=exclude)[
+                "metrics"
+            ]
+        return result
 
     def _build_dashboard_info(self):
         test_results = []
         total_tests = len(self._inner_suite.context.test_results)
         by_status = {}
-        color_options = self.options_provider.get(ColorOptions)
+        color_options = self.options.color_options
 
         for test, test_result in self._inner_suite.context.test_results.items():
             renderer = find_test_renderer(type(test), self._inner_suite.context.renderers)
             renderer.color_options = color_options
             by_status[test_result.status] = by_status.get(test_result.status, 0) + 1
             test_results.append(renderer.render_html(test))
```

### Comparing `evidently-0.3.0/src/evidently/tests/__init__.py` & `evidently-0.3.1/src/evidently/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .classification_performance_tests import TestRecallScore
 from .classification_performance_tests import TestRocAuc
 from .classification_performance_tests import TestTNR
 from .classification_performance_tests import TestTPR
 from .data_drift_tests import TestAllFeaturesValueDrift
 from .data_drift_tests import TestColumnDrift
 from .data_drift_tests import TestCustomFeaturesValueDrift
+from .data_drift_tests import TestEmbeddingsDrift
 from .data_drift_tests import TestNumberOfDriftedColumns
 from .data_drift_tests import TestShareOfDriftedColumns
 from .data_integrity_tests import TestAllColumnsShareOfMissingValues
 from .data_integrity_tests import TestColumnAllConstantValues
 from .data_integrity_tests import TestColumnAllUniqueValues
 from .data_integrity_tests import TestColumnNumberOfDifferentMissingValues
 from .data_integrity_tests import TestColumnNumberOfMissingValues
```

### Comparing `evidently-0.3.0/src/evidently/tests/base_test.py` & `evidently-0.3.1/src/evidently/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/tests/classification_performance_tests.py` & `evidently-0.3.1/src/evidently/tests/classification_performance_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/tests/data_drift_tests.py` & `evidently-0.3.1/src/evidently/tests/data_drift_tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from abc import ABC
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 
 from evidently.base_metric import ColumnName
 from evidently.calculations.data_drift import ColumnDataDriftMetrics
 from evidently.calculations.stattests import PossibleStatTestType
 from evidently.metric_results import DatasetColumns
 from evidently.metrics import ColumnDriftMetric
 from evidently.metrics import DataDriftTable
+from evidently.metrics import EmbeddingsDriftMetric
 from evidently.metrics.data_drift.data_drift_table import DataDriftTableResults
 from evidently.model.widget import BaseWidgetInfo
 from evidently.renderers.base_renderer import DetailsInfo
 from evidently.renderers.base_renderer import TestHtmlInfo
 from evidently.renderers.base_renderer import TestRenderer
 from evidently.renderers.base_renderer import default_renderer
 from evidently.renderers.html_widgets import plotly_figure
@@ -31,14 +33,15 @@
 from evidently.tests.base_test import TestParameters
 from evidently.tests.base_test import TestResult
 from evidently.tests.base_test import TestStatus
 from evidently.tests.base_test import TestValueCondition
 from evidently.utils.data_drift_utils import resolve_stattest_threshold
 from evidently.utils.generators import BaseGenerator
 from evidently.utils.types import Numeric
+from evidently.utils.visualizations import plot_contour
 
 DATA_DRIFT_GROUP = GroupData("data_drift", "Data Drift", "")
 GroupingTypes.TestGroup.add_value(DATA_DRIFT_GROUP)
 
 
 class ColumnDriftParameter(ExcludeNoneMixin, TestParameters):
     stattest: str
@@ -416,30 +419,36 @@
         return result
 
 
 @default_renderer(wrap_type=TestNumberOfDriftedColumns)
 class TestNumberOfDriftedColumnsRenderer(TestRenderer):
     def render_html(self, obj: TestNumberOfDriftedColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
-        parameters = obj.get_result().parameters
+        result = obj.get_result()
+        if result.status == TestStatus.ERROR:
+            return info
+        parameters = result.parameters
         assert isinstance(parameters, ColumnsDriftParameters)
         df = parameters.to_dataframe()
         df = df.sort_values("Data Drift")
         info.with_details(
             title="Drift Table",
             info=table_data(column_names=df.columns.to_list(), data=df.values),
         )
         return info
 
 
 @default_renderer(wrap_type=TestShareOfDriftedColumns)
 class TestShareOfDriftedColumnsRenderer(TestRenderer):
     def render_html(self, obj: TestShareOfDriftedColumns) -> TestHtmlInfo:
         info = super().render_html(obj)
-        parameters = obj.get_result().parameters
+        result = obj.get_result()
+        if result.status == TestStatus.ERROR:
+            return info
+        parameters = result.parameters
         assert isinstance(parameters, ColumnsDriftParameters)
         df = parameters.to_dataframe()
         df = df.sort_values("Data Drift")
         info.details = [
             DetailsInfo(
                 id="drift_table",
                 title="",
@@ -498,7 +507,52 @@
             fig = get_distribution_plot_figure(
                 current_distribution=result.current.distribution,
                 reference_distribution=result.reference.distribution,
                 color_options=self.color_options,
             )
             info.with_details(f"{column_name}", plotly_figure(title="", figure=fig))
         return info
+
+
+class TestEmbeddingsDrift(Test):
+    name = "Drift for embeddings"
+    group = DATA_DRIFT_GROUP.id
+    metric: EmbeddingsDriftMetric
+
+    def __init__(self, embeddings_name: str, drift_method: Optional[Callable] = None):
+        self.metric = EmbeddingsDriftMetric(embeddings_name=embeddings_name, drift_method=drift_method)
+
+    def check(self):
+        drift_info = self.metric.get_result()
+        drift_score = drift_info.drift_score
+        if drift_info.drift_detected:
+            drift = "detected"
+
+        else:
+            drift = "not detected"
+
+        description = (
+            f"Data drift {drift}. "
+            f"The drift score for the embedding set **{drift_info.embeddings_name}** is {drift_score:.3g}. "
+            f"The drift detection method is **{drift_info.method_name}**. "
+        )
+        if not drift_info.drift_detected:
+            result_status = TestStatus.SUCCESS
+
+        else:
+            result_status = TestStatus.FAIL
+        return TestResult(
+            name=self.name,
+            description=description,
+            status=result_status,
+            group=self.group,
+        )
+
+
+@default_renderer(wrap_type=TestEmbeddingsDrift)
+class TestEmbeddingsDriftRenderer(TestRenderer):
+    def render_html(self, obj: TestEmbeddingsDrift) -> TestHtmlInfo:
+        info = super().render_html(obj)
+        result = obj.metric.get_result()
+        fig = plot_contour(result.current, result.reference, "component 1", "component 2")
+        info.with_details(f"Drift in embeddings '{result.embeddings_name}'", plotly_figure(title="", figure=fig))
+        return info
```

### Comparing `evidently-0.3.0/src/evidently/tests/data_integrity_tests.py` & `evidently-0.3.1/src/evidently/tests/data_integrity_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from pandas.core.dtypes.common import infer_dtype_from_object
 
+from evidently.base_metric import ColumnName
 from evidently.metric_results import DatasetColumns
 from evidently.metrics import ColumnRegExpMetric
 from evidently.metrics import ColumnSummaryMetric
 from evidently.metrics import DatasetMissingValuesMetric
 from evidently.metrics import DatasetSummaryMetric
 from evidently.metrics.data_integrity.dataset_missing_values_metric import DatasetMissingValues
 from evidently.metrics.data_integrity.dataset_missing_values_metric import DatasetMissingValuesMetricResult
@@ -731,19 +732,19 @@
     def get_description(self, value: Numeric) -> str:
         return f"The number of duplicate columns is {value}. The test threshold is {self.get_condition()}."
 
 
 class BaseIntegrityByColumnsConditionTest(BaseCheckValueTest, ABC):
     group = DATA_INTEGRITY_GROUP.id
     data_integrity_metric: ColumnSummaryMetric
-    column_name: str
+    column_name: ColumnName
 
     def __init__(
         self,
-        column_name: str,
+        column_name: Union[str, ColumnName],
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
@@ -755,34 +756,40 @@
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
-        self.column_name = column_name
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
         self.data_integrity_metric = ColumnSummaryMetric(column_name=column_name)
 
     def groups(self) -> Dict[str, str]:
         if self.column_name is not None:
-            return {GroupingTypes.ByFeature.id: self.column_name}
+            return {GroupingTypes.ByFeature.id: self.column_name.display_name}
         return {}
 
 
 class BaseIntegrityOneColumnTest(Test, ABC):
     group = DATA_INTEGRITY_GROUP.id
     metric: ColumnSummaryMetric
-    column_name: str
+    column_name: ColumnName
 
-    def __init__(self, column_name: str):
-        self.column_name = column_name
-        self.metric = ColumnSummaryMetric(column_name)
+    def __init__(self, column_name: Union[str, ColumnName]):
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
+        self.metric = ColumnSummaryMetric(self.column_name)
 
     def groups(self) -> Dict[str, str]:
-        return {GroupingTypes.ByFeature.id: self.column_name}
+        return {GroupingTypes.ByFeature.id: self.column_name.display_name}
 
 
 class TestColumnAllConstantValues(BaseIntegrityOneColumnTest):
     """Test that there is only one unique value in a column"""
 
     name = "All Constant Values in a Column"
     metric: ColumnSummaryMetric
```

### Comparing `evidently-0.3.0/src/evidently/tests/data_quality_tests.py` & `evidently-0.3.1/src/evidently/tests/data_quality_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class BaseDataQualityMetricsValueTest(ConditionFromReferenceMixin[ColumnCharacteristics], ABC):
     reference_field: ClassVar = "reference_characteristics"
     group = DATA_QUALITY_GROUP.id
     metric: ColumnSummaryMetric
 
     def __init__(
         self,
-        column_name: str,
+        column_name: Union[str, ColumnName],
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
@@ -379,44 +379,47 @@
 
         fig = plot_correlations(current_correlations, reference_correlations)
         info.with_details("Target-Features Correlations", plotly_figure(title="", figure=fig))
         return info
 
 
 class BaseFeatureDataQualityMetricsTest(BaseDataQualityMetricsValueTest, ABC):
-    column_name: str
+    column_name: ColumnName
 
     def __init__(
         self,
-        column_name: str,
+        column_name: Union[str, ColumnName],
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
-        self.column_name = column_name
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
         super().__init__(
             column_name=column_name,
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
 
     def groups(self) -> Dict[str, str]:
         return {
-            GroupingTypes.ByFeature.id: self.column_name,
+            GroupingTypes.ByFeature.id: self.column_name.display_name,
         }
 
     def check(self):
         result = super().check()
 
         if self.value is None:
             result.mark_as_error(f"No value for the feature '{self.column_name}'")
@@ -723,15 +726,15 @@
             f"The most common value in the column **{self.column_name}** is {most_common_value}. "
             f"Its share is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
     def get_parameters(self) -> ColumnCheckValueParameters:
         return ColumnCheckValueParameters(
-            column_name=self.column_name, condition=self.get_condition(), value=self.value
+            column_name=self.column_name.display_name, condition=self.get_condition(), value=self.value
         )
 
 
 @default_renderer(wrap_type=TestMostCommonValueShare)
 class TestMostCommonValueShareRenderer(TestRenderer):
     def render_html(self, obj: TestMostCommonValueShare) -> TestHtmlInfo:
         info = super().render_html(obj)
@@ -778,19 +781,22 @@
 
 
 class TestMeanInNSigmas(Test):
 
     group = DATA_QUALITY_GROUP.id
     name = "Mean Value Stability"
     metric: ColumnSummaryMetric
-    column_name: str
+    column_name: ColumnName
     n_sigmas: int
 
-    def __init__(self, column_name: str, n_sigmas: int = 2):
-        self.column_name = column_name
+    def __init__(self, column_name: Union[str, ColumnName], n_sigmas: int = 2):
+        if isinstance(column_name, str):
+            self.column_name = ColumnName.main_dataset(column_name)
+        else:
+            self.column_name = column_name
         self.n_sigmas = n_sigmas
         self.metric = ColumnSummaryMetric(column_name)
 
     def check(self):
         reference_feature_stats = self.metric.get_result().reference_characteristics
         features_stats = self.metric.get_result().current_characteristics
 
@@ -824,26 +830,26 @@
                 description = (
                     f"The mean value of the column **{self.column_name}** is {current_mean:.3g}."
                     f" The expected range is from {left_condition:.3g} to {right_condition:.3g}"
                 )
                 test_result = TestStatus.FAIL
 
             parameters = MeanInNSigmasParameter(
-                column_name=self.column_name,
+                column_name=self.column_name.display_name,
                 n_sigmas=self.n_sigmas,
                 current_mean=current_mean,
                 reference_mean=reference_mean,
                 reference_std=reference_std,
             )
 
         return TestResult(
             name=self.name,
             description=description,
             status=test_result,
-            groups={GroupingTypes.ByFeature.id: self.column_name},
+            groups={GroupingTypes.ByFeature.id: self.column_name.display_name},
             parameters=parameters,
             group=self.group,
         )
 
 
 @default_renderer(wrap_type=TestMeanInNSigmas)
 class TestMeanInNSigmasRenderer(TestRenderer):
@@ -1230,46 +1236,49 @@
         return [TestShareOfOutListValues(column_name=name) for name in columns]
 
 
 class TestColumnQuantile(BaseCheckValueTest):
     group = DATA_QUALITY_GROUP.id
     name = "Quantile Value"
     metric: ColumnQuantileMetric
-    column_name: str
+    column: ColumnName
     quantile: float
 
     def __init__(
         self,
-        column_name: str,
+        column_name: Union[str, ColumnName],
         quantile: float,
         eq: Optional[Numeric] = None,
         gt: Optional[Numeric] = None,
         gte: Optional[Numeric] = None,
         is_in: Optional[List[Union[Numeric, str, bool]]] = None,
         lt: Optional[Numeric] = None,
         lte: Optional[Numeric] = None,
         not_eq: Optional[Numeric] = None,
         not_in: Optional[List[Union[Numeric, str, bool]]] = None,
     ):
-        self.column_name = column_name
+        if isinstance(column_name, str):
+            self.column = ColumnName.main_dataset(column_name)
+        else:
+            self.column = column_name
         self.quantile = quantile
         super().__init__(
             eq=eq,
             gt=gt,
             gte=gte,
             is_in=is_in,
             lt=lt,
             lte=lte,
             not_eq=not_eq,
             not_in=not_in,
         )
         self.metric = ColumnQuantileMetric(column_name=column_name, quantile=quantile)
 
     def groups(self) -> Dict[str, str]:
-        return {GroupingTypes.ByFeature.id: self.column_name}
+        return {GroupingTypes.ByFeature.id: self.column.display_name}
 
     def get_condition(self) -> TestValueCondition:
         if self.condition.has_condition():
             return self.condition
 
         reference = self.metric.get_result().reference
 
@@ -1279,15 +1288,15 @@
         raise ValueError("Neither required test parameters nor reference data has been provided.")
 
     def calculate_value_for_test(self) -> Numeric:
         return self.metric.get_result().current.value
 
     def get_description(self, value: Numeric) -> str:
         return (
-            f"The {self.quantile} quantile value of the column **{self.column_name}** is {value:.3g}. "
+            f"The {self.quantile} quantile value of the column **{self.column}** is {value:.3g}. "
             f"The test threshold is {self.get_condition()}."
         )
 
 
 @default_renderer(wrap_type=TestColumnQuantile)
 class TestColumnQuantileRenderer(TestRenderer):
     def render_html(self, obj: TestColumnQuantile) -> TestHtmlInfo:
```

### Comparing `evidently-0.3.0/src/evidently/tests/regression_performance_tests.py` & `evidently-0.3.1/src/evidently/tests/regression_performance_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/tests/utils.py` & `evidently-0.3.1/src/evidently/tests/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/dashboard.py` & `evidently-0.3.1/src/evidently/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/data_drift_utils.py` & `evidently-0.3.1/src/evidently/utils/data_drift_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
@@ -126,15 +127,21 @@
 
     np.random.seed(seed)
     seeds = np.random.randint(0, iter_num * 10, size=iter_num)
     roc_auc_values = [calc_roc_auc_random(y_test, seed=seed) for seed in seeds]
     return np.percentile(roc_auc_values, 100 * (1 - p_value))
 
 
-def calculate_text_drift_score(reference_data: pd.Series, current_data: pd.Series, p_value=0.05) -> Tuple[float, bool]:
+def calculate_text_drift_score(
+    reference_data: pd.Series,
+    current_data: pd.Series,
+    bootstrap: bool,
+    p_value=0.05,
+    threshold=0.55,
+) -> Tuple[float, bool]:
     domain_data = pd.concat(
         [
             pd.DataFrame({"text": reference_data, "target": 0}),
             pd.DataFrame({"text": current_data, "target": 1}),
         ]
     )
 
@@ -148,17 +155,18 @@
 
     domain_classifier_roc_auc, _, _ = roc_auc_domain_classifier(
         X_train,
         X_test,
         y_train,
         y_test,
     )
-
-    random_classifier_95_percentile = roc_auc_random_classifier_percentile(y_test, p_value=p_value)
-    return domain_classifier_roc_auc, domain_classifier_roc_auc > random_classifier_95_percentile
+    if not bootstrap:
+        return domain_classifier_roc_auc, domain_classifier_roc_auc > threshold
+    random_classifier_percentile = roc_auc_random_classifier_percentile(y_test, p_value=p_value)
+    return domain_classifier_roc_auc, domain_classifier_roc_auc > random_classifier_percentile
 
 
 def get_typical_examples(X_test, y_test, y_pred_proba, examples_num=10) -> Tuple[List[str], List[str]]:
     typical_examples = pd.DataFrame({"text": X_test, "label": y_test, "predict_proba": y_pred_proba})
 
     typical_current = typical_examples[typical_examples["label"] == 1]
     typical_current.sort_values("predict_proba", ascending=False, inplace=True)
@@ -216,7 +224,29 @@
     # get examples more characteristic of current or reference dataset
     typical_examples_cur, typical_examples_ref = get_typical_examples(X_test, y_test, y_pred_proba)
 
     # get words more characteristic of current or reference dataset
     typical_words_cur, typical_words_ref = get_typical_words(classifier_pipeline)
 
     return typical_examples_cur, typical_examples_ref, typical_words_cur, typical_words_ref
+
+
+def add_emb_drift_to_reports(
+    result,
+    embeddings_data,
+    embeddings,
+    embeddings_drift_method,
+    entity,
+):
+    sets = list(embeddings_data.keys())
+    if embeddings is not None:
+        sets = np.intersect1d(sets, embeddings)
+    if len(sets) == 0:
+        return result
+    f: Optional[Callable]
+    for emb_set in sets:
+        if embeddings_drift_method is not None:
+            f = embeddings_drift_method.get(emb_set)
+        else:
+            f = None
+        result.append(entity(embeddings_name=emb_set, drift_method=f))
+    return result
```

### Comparing `evidently-0.3.0/src/evidently/utils/data_operations.py` & `evidently-0.3.1/src/evidently/utils/data_operations.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/data_preprocessing.py` & `evidently-0.3.1/src/evidently/utils/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/generators.py` & `evidently-0.3.1/src/evidently/utils/generators.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/numpy_encoder.py` & `evidently-0.3.1/src/evidently/utils/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/types.py` & `evidently-0.3.1/src/evidently/utils/types.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.0/src/evidently/utils/visualizations.py` & `evidently-0.3.1/src/evidently/utils/visualizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,25 +317,46 @@
         fig.add_trace(trace)
         fig.update_layout(boxmode="group")
     fig.update_layout(yaxis_title=yaxis_title, xaxis_title=xaxis_title, boxmode="group")
     fig = json.loads(fig.to_json())
     return fig
 
 
-def make_hist_for_num_plot(curr: pd.Series, ref: pd.Series = None) -> Histogram:
+def histogram_for_data(
+    curr: pd.Series,
+    ref: Optional[pd.Series] = None,
+) -> Tuple[HistogramData, Optional[HistogramData]]:
     if ref is not None:
         ref = ref.dropna()
     bins = np.histogram_bin_edges(pd.concat([curr.dropna(), ref]), bins="doane")
     curr_hist = np.histogram(curr, bins=bins)
     current = make_hist_df(curr_hist)
     reference = None
     if ref is not None:
         ref_hist = np.histogram(ref, bins=bins)
         reference = make_hist_df(ref_hist)
-    return Histogram(current=HistogramData.from_df(current), reference=HistogramData.from_df(reference))
+
+    return HistogramData.from_df(current), HistogramData.from_df(reference) if reference is not None else None
+
+
+def make_hist_for_num_plot(curr: pd.Series, ref: Optional[pd.Series] = None, calculate_log: bool = False) -> Histogram:
+    current, reference = histogram_for_data(curr, ref)
+    current_log = None
+    reference_log = None
+    if calculate_log:
+        current_log, reference_log = histogram_for_data(
+            np.log10(curr[curr > 0]),
+            np.log10(ref[ref > 0]) if ref is not None else None,
+        )
+    return Histogram(
+        current=current,
+        reference=reference,
+        current_log=current_log,
+        reference_log=reference_log,
+    )
 
 
 def plot_cat_cat_rel(
     curr: pd.DataFrame, ref: pd.DataFrame, target_name: str, feature_name: str, color_options: ColorOptions
 ):
     """
     Accepts current and reference data as pandas dataframes with two columns: feature_name and "count_objects".
@@ -745,15 +766,15 @@
         fig.add_trace(trace, 1, 2)
     fig.update_layout(coloraxis={"colorscale": "RdBu_r"})
     return fig
 
 
 def get_gaussian_kde(m1, m2):
     def border(x):
-        return int(max(2, abs(x) * 0.2))
+        return int(max(2, abs(x) * 0.7))
 
     xmin = m1.min()
     xmax = m1.max()
     ymin = m2.min()
     ymax = m2.max()
     X, Y = np.mgrid[xmin - border(xmin) : xmax + border(xmax) : 30j, ymin - border(ymin) : ymax + border(ymax) : 30j]
     positions = np.vstack([X.ravel(), Y.ravel()])
```

