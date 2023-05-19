# Comparing `tmp/boonamber-2.0.2.tar.gz` & `tmp/boonamber-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boonamber-2.0.2.tar", last modified: Tue May  9 13:59:06 2023, max compression
+gzip compressed data, was "boonamber-2.0.3.tar", last modified: Fri May 19 13:52:08 2023, max compression
```

## Comparing `boonamber-2.0.2.tar` & `boonamber-2.0.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.941321 boonamber-2.0.2/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     1072 2023-05-05 14:50:26.000000 boonamber-2.0.2/LICENSE
--rw-r--r--   0 jimturnquist   (502) staff       (20)      997 2023-05-09 13:59:06.941188 boonamber-2.0.2/PKG-INFO
--rw-r--r--   0 jimturnquist   (502) staff       (20)      543 2023-05-09 13:57:59.000000 boonamber-2.0.2/README.md
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.926852 boonamber-2.0.2/boonamber/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2124 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/__init__.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.927699 boonamber-2.0.2/boonamber/util/
--rw-r--r--   0 jimturnquist   (502) staff       (20)      402 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/util/ambererror.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.927896 boonamber-2.0.2/boonamber/v1/
--rw-r--r--   0 jimturnquist   (502) staff       (20)    48321 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v1/__init__.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.929257 boonamber-2.0.2/boonamber/v2/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4450 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    23030 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/amber_client.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.929842 boonamber-2.0.2/boonamber/v2/api/
--rw-r--r--   0 jimturnquist   (502) staff       (20)      139 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/api/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    92075 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/api/default_api.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    24975 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/api_client.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8168 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/configuration.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.941018 boonamber-2.0.2/boonamber/v2/models/
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4250 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/__init__.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2477 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/amber_state.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    11774 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/analytic_results.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3659 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/autotuning.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6030 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/config_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2663 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/delete_model_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3480 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/error.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8715 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/feature_config.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3880 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/feature_config_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3986 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/feature_root_cause.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3681 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/fusion_feature.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3046 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_models_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2712 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_nano_status_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2736 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_pretrain_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3220 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_root_cause_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2704 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_status_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    31255 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_summary_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8967 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/get_version_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9710 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_amber_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9591 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_autotune.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6488 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_buffer_stats.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6625 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_nano.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     7210 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_nano_backend.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     7188 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_nano_config.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3108 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_pattern_memory.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_recent_ams.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3852 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_recent_analytics.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3816 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_recent_floats.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_recent_ids.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3846 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_recent_samples.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3804 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_recent_times.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9886 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_streaming_parameters.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6575 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/m_training.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2326 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/magic_number.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     7172 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/map.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6827 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/mncp.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4792 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/model.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     9003 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/model_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    10035 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/nano_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2346 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/percent_variation.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     6232 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_config_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2732 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_config_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4149 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_data_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3646 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_data_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3032 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_learning_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3671 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_learning_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3147 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_model_copy_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3131 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_model_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2655 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_model_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4048 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_oauth2_access_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     5888 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_oauth2_access_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3326 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_oauth2_refresh_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     5908 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_oauth2_refresh_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4959 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_pretrain_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4189 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/post_pretrain_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4077 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/pretrain_status.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4525 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/put_data_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     4330 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/put_data_response.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     3045 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/put_model_request.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2342 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/streaming_window.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     8682 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/training_config.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2334 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/models/version_number.py
--rw-r--r--   0 jimturnquist   (502) staff       (20)    12835 2023-05-05 15:08:33.000000 boonamber-2.0.2/boonamber/v2/rest.py
-drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-09 13:59:06.927583 boonamber-2.0.2/boonamber.egg-info/
--rw-r--r--   0 jimturnquist   (502) staff       (20)      997 2023-05-09 13:59:06.000000 boonamber-2.0.2/boonamber.egg-info/PKG-INFO
--rw-r--r--   0 jimturnquist   (502) staff       (20)     2962 2023-05-09 13:59:06.000000 boonamber-2.0.2/boonamber.egg-info/SOURCES.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)        1 2023-05-09 13:59:06.000000 boonamber-2.0.2/boonamber.egg-info/dependency_links.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)       15 2023-05-09 13:59:06.000000 boonamber-2.0.2/boonamber.egg-info/requires.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)       10 2023-05-09 13:59:06.000000 boonamber-2.0.2/boonamber.egg-info/top_level.txt
--rw-r--r--   0 jimturnquist   (502) staff       (20)      835 2023-05-09 13:58:16.000000 boonamber-2.0.2/pyproject.toml
--rw-r--r--   0 jimturnquist   (502) staff       (20)       38 2023-05-09 13:59:06.941362 boonamber-2.0.2/setup.cfg
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.926925 boonamber-2.0.3/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     1072 2023-05-19 12:17:41.000000 boonamber-2.0.3/LICENSE
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      845 2023-05-19 13:52:08.926793 boonamber-2.0.3/PKG-INFO
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      391 2023-05-19 12:58:46.000000 boonamber-2.0.3/README.md
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.913848 boonamber-2.0.3/boonamber/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2124 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/__init__.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.914812 boonamber-2.0.3/boonamber/util/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      402 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/util/ambererror.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.914970 boonamber-2.0.3/boonamber/v1/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    48321 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v1/__init__.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.916669 boonamber-2.0.3/boonamber/v2/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4450 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    23478 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/amber_client.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.917135 boonamber-2.0.3/boonamber/v2/api/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      139 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/api/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    92075 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/api/default_api.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    24975 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/api_client.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8168 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/configuration.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.926576 boonamber-2.0.3/boonamber/v2/models/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4250 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/__init__.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2477 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/amber_state.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    11774 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/analytic_results.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3659 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/autotuning.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6030 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2663 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/delete_model_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3480 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/error.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8715 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/feature_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3880 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/feature_config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3986 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/feature_root_cause.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3681 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/fusion_feature.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3046 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_models_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2712 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_nano_status_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2736 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_pretrain_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3220 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_root_cause_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2704 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_status_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    31255 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_summary_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8967 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/get_version_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9710 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_amber_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9591 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_autotune.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6488 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_buffer_stats.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6625 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_nano.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7210 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_nano_backend.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7188 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_nano_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3108 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_pattern_memory.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_ams.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3852 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_analytics.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3816 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_floats.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3780 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_ids.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3846 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_samples.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3804 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_recent_times.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9886 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_streaming_parameters.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6575 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/m_training.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2326 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/magic_number.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     7172 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/map.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6827 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/mncp.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4792 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/model.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     9003 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/model_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    10035 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/nano_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2346 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/percent_variation.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     6232 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_config_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2732 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_config_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4149 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_data_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3646 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_data_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3032 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_learning_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3671 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_learning_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3147 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_model_copy_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3131 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_model_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2655 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_model_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4048 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     5888 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3326 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     5908 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4959 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_pretrain_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4189 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/post_pretrain_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4077 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/pretrain_status.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4525 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/put_data_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     4330 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/put_data_response.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     3045 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/put_model_request.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2342 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/streaming_window.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     8682 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/training_config.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2334 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/models/version_number.py
+-rw-r--r--   0 jimturnquist   (502) staff       (20)    12835 2023-05-19 12:17:41.000000 boonamber-2.0.3/boonamber/v2/rest.py
+drwxr-xr-x   0 jimturnquist   (502) staff       (20)        0 2023-05-19 13:52:08.914689 boonamber-2.0.3/boonamber.egg-info/
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      845 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/PKG-INFO
+-rw-r--r--   0 jimturnquist   (502) staff       (20)     2962 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/SOURCES.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)        1 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/dependency_links.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       15 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/requires.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       10 2023-05-19 13:52:08.000000 boonamber-2.0.3/boonamber.egg-info/top_level.txt
+-rw-r--r--   0 jimturnquist   (502) staff       (20)      835 2023-05-19 13:50:56.000000 boonamber-2.0.3/pyproject.toml
+-rw-r--r--   0 jimturnquist   (502) staff       (20)       38 2023-05-19 13:52:08.926961 boonamber-2.0.3/setup.cfg
```

### Comparing `boonamber-2.0.2/LICENSE` & `boonamber-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/__init__.py` & `boonamber-2.0.3/boonamber/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v1/__init__.py` & `boonamber-2.0.3/boonamber/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/__init__.py` & `boonamber-2.0.3/boonamber/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/amber_client.py` & `boonamber-2.0.3/boonamber/v2/amber_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,25 @@
             license_id: (type: str) license identifier label found within .Amber.license file
             license_file: (type: str) path to .Amber.license file
             verify: (type: boolean) Boolean, controls whether we verify the server’s TLS certificate
             timeout: (type: int) number of seconds to allow API call to wait
 
         Environment:
 
-            `AMBER_LICENSE_FILE`: sets license_file path
+            `AMBER_V2_LICENSE_FILE`: sets license_file path
 
-            `AMBER_LICENSE_ID`: sets license_id
+            `AMBER_V2_LICENSE_ID`: sets license_id
 
-            `AMBER_SERVER`: overrides the server as found in .Amber.license file
+            `AMBER_V2_SERVER`: overrides the server as found in .Amber.license file
 
-            `AMBER_OAUTH_SERVER`: overrides the oauth server as found in .Amber.license file
+            `AMBER_V2_OAUTH_SERVER`: overrides the oauth server as found in .Amber.license file
+
+            `AMBER_V2_LICENSE_KEY`: overrides the license key as found in .Amber.license file
+
+            `AMBER_V2_SECRET_KEY`: overrides the secret key as found in .Amber.license file
 
         Raises:
             ApiException: if error supplying authentication credentials
         """
         self.access_token = ""
         self.refresh_token = ""
         self.reauth_time = 0
@@ -83,20 +87,26 @@
         if "oauth-server" in file_data[self.profile_id].keys():
             self.oauth_server = file_data[self.profile_id]["oauth-server"]
         self.oauth_server = os.environ.get("AMBER_V2_OAUTH_SERVER", self.oauth_server)
         if self.oauth_server == "":
             self.oauth_server = self.server
 
         try:
-            key = "license"
             self.license = file_data[self.profile_id]["license"]
-            key = "secret"
             self.secret = file_data[self.profile_id]["secret"]
         except KeyError as e:
-            raise ApiException('profile "{user}" missing "{key}" key'.format(user=self.profile_id, key=key))
+            # do nothing here
+            self.license = ""
+            self.secret = ""
+
+        self.license = os.environ.get("AMBER_V2_LICENSE_KEY", self.license)
+        self.secret = os.environ.get("AMBER_V2_SECRET_KEY", self.secret)
+
+        if self.license == "" or self.secret == "":
+            raise ApiException("need license and secret keys set in either the environment or the .Amber.license file")
 
         self.api = DefaultApi(ApiClient(self.configuration))
 
     def __authenticate(f):
         @wraps(f)
         def inner(self, *args, **kwargs):
             if time.time() <= self.reauth_time:
```

### Comparing `boonamber-2.0.2/boonamber/v2/api/default_api.py` & `boonamber-2.0.3/boonamber/v2/api/default_api.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/api_client.py` & `boonamber-2.0.3/boonamber/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/configuration.py` & `boonamber-2.0.3/boonamber/v2/configuration.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/__init__.py` & `boonamber-2.0.3/boonamber/v2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/amber_state.py` & `boonamber-2.0.3/boonamber/v2/models/amber_state.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/analytic_results.py` & `boonamber-2.0.3/boonamber/v2/models/analytic_results.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/autotuning.py` & `boonamber-2.0.3/boonamber/v2/models/autotuning.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/config_response.py` & `boonamber-2.0.3/boonamber/v2/models/config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/delete_model_response.py` & `boonamber-2.0.3/boonamber/v2/models/delete_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/error.py` & `boonamber-2.0.3/boonamber/v2/models/error.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/feature_config.py` & `boonamber-2.0.3/boonamber/v2/models/feature_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/feature_config_response.py` & `boonamber-2.0.3/boonamber/v2/models/feature_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/feature_root_cause.py` & `boonamber-2.0.3/boonamber/v2/models/feature_root_cause.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/fusion_feature.py` & `boonamber-2.0.3/boonamber/v2/models/fusion_feature.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_models_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_models_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_nano_status_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_nano_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_pretrain_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_root_cause_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_root_cause_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_status_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_summary_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_summary_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/get_version_response.py` & `boonamber-2.0.3/boonamber/v2/models/get_version_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_amber_status.py` & `boonamber-2.0.3/boonamber/v2/models/m_amber_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_autotune.py` & `boonamber-2.0.3/boonamber/v2/models/m_autotune.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_buffer_stats.py` & `boonamber-2.0.3/boonamber/v2/models/m_buffer_stats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_nano.py` & `boonamber-2.0.3/boonamber/v2/models/m_nano.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_nano_backend.py` & `boonamber-2.0.3/boonamber/v2/models/m_nano_backend.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_nano_config.py` & `boonamber-2.0.3/boonamber/v2/models/m_nano_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_pattern_memory.py` & `boonamber-2.0.3/boonamber/v2/models/m_pattern_memory.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_recent_ams.py` & `boonamber-2.0.3/boonamber/v2/models/m_recent_ams.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_recent_analytics.py` & `boonamber-2.0.3/boonamber/v2/models/m_recent_analytics.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_recent_floats.py` & `boonamber-2.0.3/boonamber/v2/models/m_recent_floats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_recent_ids.py` & `boonamber-2.0.3/boonamber/v2/models/m_recent_ids.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_recent_samples.py` & `boonamber-2.0.3/boonamber/v2/models/m_recent_samples.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_recent_times.py` & `boonamber-2.0.3/boonamber/v2/models/m_recent_times.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_streaming_parameters.py` & `boonamber-2.0.3/boonamber/v2/models/m_streaming_parameters.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/m_training.py` & `boonamber-2.0.3/boonamber/v2/models/m_training.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/magic_number.py` & `boonamber-2.0.3/boonamber/v2/models/magic_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/map.py` & `boonamber-2.0.3/boonamber/v2/models/map.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/mncp.py` & `boonamber-2.0.3/boonamber/v2/models/mncp.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/model.py` & `boonamber-2.0.3/boonamber/v2/models/model.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/model_status.py` & `boonamber-2.0.3/boonamber/v2/models/model_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/nano_status.py` & `boonamber-2.0.3/boonamber/v2/models/nano_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/percent_variation.py` & `boonamber-2.0.3/boonamber/v2/models/percent_variation.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_config_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_config_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_config_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_data_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_data_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_learning_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_learning_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_learning_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_learning_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_model_copy_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_model_copy_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_model_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_model_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_oauth2_access_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_oauth2_access_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_oauth2_access_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_oauth2_refresh_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_oauth2_refresh_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_oauth2_refresh_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_pretrain_request.py` & `boonamber-2.0.3/boonamber/v2/models/post_pretrain_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/post_pretrain_response.py` & `boonamber-2.0.3/boonamber/v2/models/post_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/pretrain_status.py` & `boonamber-2.0.3/boonamber/v2/models/pretrain_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/put_data_request.py` & `boonamber-2.0.3/boonamber/v2/models/put_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/put_data_response.py` & `boonamber-2.0.3/boonamber/v2/models/put_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/put_model_request.py` & `boonamber-2.0.3/boonamber/v2/models/put_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/streaming_window.py` & `boonamber-2.0.3/boonamber/v2/models/streaming_window.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/training_config.py` & `boonamber-2.0.3/boonamber/v2/models/training_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/models/version_number.py` & `boonamber-2.0.3/boonamber/v2/models/version_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber/v2/rest.py` & `boonamber-2.0.3/boonamber/v2/rest.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/boonamber.egg-info/SOURCES.txt` & `boonamber-2.0.3/boonamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.2/pyproject.toml` & `boonamber-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "boonamber"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
     {name = "BoonLogic"},
     {email = "amber-support@boonlogic.com"}
 ]
 urls = {repository = "https://github.com/boonlogic/amber-python-sdk"}
 license = {text = "MIT"}
 description = "An SDK for Boon Amber sensor analytics"
```

