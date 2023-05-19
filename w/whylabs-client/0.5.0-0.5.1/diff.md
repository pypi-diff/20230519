# Comparing `tmp/whylabs-client-0.5.0.tar.gz` & `tmp/whylabs-client-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs-client-0.5.0.tar", last modified: Tue May  2 15:18:36 2023, max compression
+gzip compressed data, was "whylabs-client-0.5.1.tar", last modified: Fri May 19 20:33:58 2023, max compression
```

## Comparing `whylabs-client-0.5.0.tar` & `whylabs-client-0.5.1.tar`

### file list

```diff
@@ -1,156 +1,158 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     3358 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    23347 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-02 15:18:36.518487 whylabs-client-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1269 2023-05-02 15:18:35.000000 whylabs-client-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.469483 whylabs-client-0.5.0/whylabs_client/
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.475484 whylabs-client-0.5.0/whylabs_client/api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15394 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/dataset_metadata_api.py
--rw-rw-rw-   0 root         (0) root         (0)    28878 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/dataset_profile_api.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/feature_weights_api.py
--rw-rw-rw-   0 root         (0) root         (0)    11520 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/log_api.py
--rw-rw-rw-   0 root         (0) root         (0)    20727 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/membership_api.py
--rw-rw-rw-   0 root         (0) root         (0)    67177 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/models_api.py
--rw-rw-rw-   0 root         (0) root         (0)    52337 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/monitor_api.py
--rw-rw-rw-   0 root         (0) root         (0)    48204 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/notification_settings_api.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/schema_api.py
--rw-rw-rw-   0 root         (0) root         (0)    29965 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api/sessions_api.py
--rw-rw-rw-   0 root         (0) root         (0)    37575 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.476484 whylabs-client-0.5.0/whylabs_client/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1038 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17084 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     5075 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/whylabs_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11664 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/action_type.py
--rw-rw-rw-   0 root         (0) root         (0)    12110 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/add_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12005 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/async_log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    13478 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/aws_marketplace_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11342 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/batch_log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11655 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/batch_log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12443 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/column_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11118 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/create_session_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11207 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/create_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11136 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/create_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13099 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/databricks_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    11884 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dataset_request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11114 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/datatype_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/delete_analyzer_results_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/delete_dataset_profiles_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11368 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/distribution_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_auto_scale_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    13257 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_attributes_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11739 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_availability_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11804 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11745 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_ebs_volume_type_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_cron_schedule_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11934 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_data_security_mode_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11969 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    12404 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    16133 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_settings_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_new_cluster_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11603 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_notebook_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11707 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_python_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11293 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
--rw-rw-rw-   0 root         (0) root         (0)    11106 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/email_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12313 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12718 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_search_result.py
--rw-rw-rw-   0 root         (0) root         (0)    11862 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_weight_record.py
--rw-rw-rw-   0 root         (0) root         (0)    11507 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/entity_weight_record_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/feature_flags.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11411 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11222 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_dataset_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11283 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_default_membership_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11431 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_marketplace_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11485 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11379 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_monitor_config_v2_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11417 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_notification_settings_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11334 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/get_session_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11559 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_jobs_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11289 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_jobs_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11496 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_models_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_organization_memberships_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11382 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/list_user_api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    11502 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_async_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11354 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_reference_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11858 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11441 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12111 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/log_session_reference_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/marketplace_dimensions.py
--rw-rw-rw-   0 root         (0) root         (0)    12029 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/membership.py
--rw-rw-rw-   0 root         (0) root         (0)    11756 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/membership_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    12260 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/metric_schema.py
--rw-rw-rw-   0 root         (0) root         (0)    11120 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/missing_recent_data_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11132 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/missing_recent_profiles_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11938 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/missing_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    12569 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/model_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12219 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/model_type.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_config_version.py
--rw-rw-rw-   0 root         (0) root         (0)    12120 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11982 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_settings_day.py
--rw-rw-rw-   0 root         (0) root         (0)    11751 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/notification_sqs_message_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)    14425 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/organization_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    13737 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/organization_summary.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/pager_duty_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12319 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provided_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11680 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11657 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11882 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_aws_marketplace_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_marketplace_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12422 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_user_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11574 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/provision_new_user_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12387 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/reference_profile_item_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11188 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/refresh_access_token_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11444 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/refresh_connection_by_org_id_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11586 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/refresh_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13668 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11112 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11317 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/remove_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    13372 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/request_feature_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15325 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/request_monitor_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11070 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/response.py
--rw-rw-rw-   0 root         (0) root         (0)    11580 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/role.py
--rw-rw-rw-   0 root         (0) root         (0)    11922 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/run_job_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11089 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/run_job_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11471 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/schema_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11447 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/search_index_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11787 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/search_index_type.py
--rw-rw-rw-   0 root         (0) root         (0)    11530 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/search_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11833 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/seasonal_arima_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11197 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/segment.py
--rw-rw-rw-   0 root         (0) root         (0)    11192 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/segment_tag.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/segment_weight.py
--rw-rw-rw-   0 root         (0) root         (0)    11948 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/session_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11350 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/set_default_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11193 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/slack_notification_action.py
--rw-rw-rw-   0 root         (0) root         (0)    11652 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/subscription_tier.py
--rw-rw-rw-   0 root         (0) root         (0)    11610 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/time_period.py
--rw-rw-rw-   0 root         (0) root         (0)    12934 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/uber_notification_schedule.py
--rw-rw-rw-   0 root         (0) root         (0)    11917 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/unique_values_monitor_request_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/update_connection_changes.py
--rw-rw-rw-   0 root         (0) root         (0)    11816 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/update_connection_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11650 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/update_membership_request.py
--rw-rw-rw-   0 root         (0) root         (0)    11747 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/user.py
--rw-rw-rw-   0 root         (0) root         (0)    13667 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/user_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)    11220 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/user_api_key_response.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model/why_logs_metric.py
--rw-rw-rw-   0 root         (0) root         (0)    81897 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.517487 whylabs-client-0.5.0/whylabs_client/models/
--rw-rw-rw-   0 root         (0) root         (0)    10053 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14199 2023-05-02 15:18:25.000000 whylabs-client-0.5.0/whylabs_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 15:18:36.471484 whylabs-client-0.5.0/whylabs_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3358 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6781 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-02 15:18:36.000000 whylabs-client-0.5.0/whylabs_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.720948 whylabs-client-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-05-19 20:33:58.720948 whylabs-client-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    24186 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-19 20:33:58.721948 whylabs-client-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-05-19 20:33:58.000000 whylabs-client-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.685948 whylabs-client-0.5.1/whylabs_client/
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.690948 whylabs-client-0.5.1/whylabs_client/api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15394 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/dataset_metadata_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    34745 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/dataset_profile_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    10632 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/feature_weights_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    11520 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/log_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20727 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/membership_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    67177 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/models_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    52337 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/monitor_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    48204 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/notification_settings_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/schema_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    29965 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api/sessions_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    37579 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.690948 whylabs-client-0.5.1/whylabs_client/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17084 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     5075 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.720948 whylabs-client-0.5.1/whylabs_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11664 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/action_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    12110 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/add_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12005 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/async_log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    13478 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/aws_marketplace_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/batch_log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11655 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/batch_log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12443 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/column_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12228 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/create_reference_profile_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12113 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/create_reference_profile_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11118 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/create_session_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11207 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/create_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/create_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13099 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/databricks_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    11884 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dataset_request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11114 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/datatype_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/delete_analyzer_results_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/delete_dataset_profiles_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11368 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/distribution_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_clusters_auto_scale_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    13257 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_clusters_aws_attributes_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11739 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_clusters_aws_availability_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11804 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_clusters_s3_storage_info_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11745 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_ebs_volume_type_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_cron_schedule_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11934 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_data_security_mode_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11969 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_job_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_job_email_notifications_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16133 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_job_settings_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    16932 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_new_cluster_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11603 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_notebook_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11707 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_spark_jar_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_spark_python_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11293 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/dto_jobs_spark_submit_task_dto.py
+-rw-rw-rw-   0 root         (0) root         (0)    11106 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/email_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12313 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/entity_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12718 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/entity_search_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    11862 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/entity_weight_record.py
+-rw-rw-rw-   0 root         (0) root         (0)    11507 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/entity_weight_record_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/feature_flags.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11411 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11222 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_dataset_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11283 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_default_membership_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11431 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_marketplace_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11485 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11379 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_monitor_config_v2_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11417 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_notification_settings_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11334 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/get_session_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11559 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/list_jobs_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11289 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/list_jobs_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11496 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/list_models_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/list_organization_memberships_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11382 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/list_user_api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    11502 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/log_async_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11354 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/log_reference_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11858 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/log_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11441 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/log_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12111 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/log_session_reference_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/marketplace_dimensions.py
+-rw-rw-rw-   0 root         (0) root         (0)    12029 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/membership.py
+-rw-rw-rw-   0 root         (0) root         (0)    11756 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/membership_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    12260 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/metric_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    11120 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/missing_recent_data_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11132 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/missing_recent_profiles_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11938 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/missing_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    12569 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/model_metadata_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12219 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/monitor_config_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12120 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/monitor_request_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/monitor_request_reference_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11783 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11982 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/notification_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/notification_settings_day.py
+-rw-rw-rw-   0 root         (0) root         (0)    11751 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/notification_sqs_message_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)    14425 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/organization_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    13737 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/organization_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/pager_duty_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12319 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provided_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11680 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provision_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11657 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provision_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11882 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provision_new_aws_marketplace_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12226 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provision_new_marketplace_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    12422 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provision_new_user_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/provision_new_user_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12624 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/reference_profile_item_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11188 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/refresh_access_token_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11444 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/refresh_connection_by_org_id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/refresh_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13668 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/register_databricks_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11112 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/register_databricks_connection_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11317 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/remove_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    13372 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/request_feature_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15325 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/request_monitor_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11070 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11580 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/role.py
+-rw-rw-rw-   0 root         (0) root         (0)    11922 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/run_job_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/run_job_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11471 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/schema_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11447 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/search_index_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11787 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/search_index_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    11530 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/search_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11833 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/seasonal_arima_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/segment.py
+-rw-rw-rw-   0 root         (0) root         (0)    11192 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/segment_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/segment_weight.py
+-rw-rw-rw-   0 root         (0) root         (0)    11948 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/session_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11350 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/set_default_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11193 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/slack_notification_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    11652 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/subscription_tier.py
+-rw-rw-rw-   0 root         (0) root         (0)    11610 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/time_period.py
+-rw-rw-rw-   0 root         (0) root         (0)    12934 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/uber_notification_schedule.py
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/unique_values_monitor_request_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/update_connection_changes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11816 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/update_connection_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11650 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/update_membership_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    11747 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/user.py
+-rw-rw-rw-   0 root         (0) root         (0)    13667 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/user_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/user_api_key_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model/why_logs_metric.py
+-rw-rw-rw-   0 root         (0) root         (0)    81897 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.720948 whylabs-client-0.5.1/whylabs_client/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10247 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14199 2023-05-19 20:33:49.000000 whylabs-client-0.5.1/whylabs_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 20:33:58.687948 whylabs-client-0.5.1/whylabs_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-05-19 20:33:58.000000 whylabs-client-0.5.1/whylabs_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6896 2023-05-19 20:33:58.000000 whylabs-client-0.5.1/whylabs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 20:33:58.000000 whylabs-client-0.5.1/whylabs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-19 20:33:58.000000 whylabs-client-0.5.1/whylabs_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-19 20:33:58.000000 whylabs-client-0.5.1/whylabs_client.egg-info/top_level.txt
```

### Comparing `whylabs-client-0.5.0/PKG-INFO` & `whylabs-client-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
@@ -75,14 +75,15 @@
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
 # Configure API key authorization: ApiKeyAuth
 configuration.api_key['ApiKeyAuth'] = 'YOUR_API_KEY'
+configuration.discard_unknown_keys = True
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
 with whylabs_client.ApiClient(configuration) as api_client:
```

### Comparing `whylabs-client-0.5.0/README.md` & `whylabs-client-0.5.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whylabs-client
 WhyLabs API that enables end-to-end AI observability
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1
-- Package version: 0.5.0
+- Package version: 0.5.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://whylabs.ai](https://whylabs.ai)
 
 ## Requirements.
 
 Python >= 3.6
 
@@ -47,14 +47,16 @@
 
 ```python
 
 import time
 import whylabs_client
 from pprint import pprint
 from whylabs_client.api import dataset_profile_api
+from whylabs_client.model.create_reference_profile_request import CreateReferenceProfileRequest
+from whylabs_client.model.create_reference_profile_response import CreateReferenceProfileResponse
 from whylabs_client.model.delete_analyzer_results_response import DeleteAnalyzerResultsResponse
 from whylabs_client.model.delete_dataset_profiles_response import DeleteDatasetProfilesResponse
 from whylabs_client.model.reference_profile_item_response import ReferenceProfileItemResponse
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = whylabs_client.Configuration(
     host = "http://localhost"
@@ -73,32 +75,49 @@
 
 
 # Enter a context with an instance of the API client
 with whylabs_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = dataset_profile_api.DatasetProfileApi(api_client)
     org_id = "org-123" # str | Your company's unique organization ID
-dataset_id = "model-123" # str | The unique dataset ID in your company.
-start_timestamp = 1577836800000 # int, none_type | Optional, scope deleting analyzer results more recent than the timestamp (optional)
-end_timestamp = 1893456000000 # int, none_type | Optional, scope deleting analyzer results older than the timestamp (optional)
+dataset_id = "model-123" # str | The unique model ID in your company.
+create_reference_profile_request = CreateReferenceProfileRequest(
+        alias="alias_example",
+        version="version_example",
+        dataset_timestamp=1,
+        segments=[
+            Segment(
+                tags=[
+                    SegmentTag(
+                        key="key_example",
+                        value="value_example",
+                    ),
+                ],
+            ),
+        ],
+        tags=[
+            "tags_example",
+        ],
+    ) # CreateReferenceProfileRequest | 
 
     try:
-        # Deletes a set of analyzer results
-        api_response = api_instance.delete_analyzer_results(org_id, dataset_id, start_timestamp=start_timestamp, end_timestamp=end_timestamp)
+        # Returns data needed to uploading the reference profile
+        api_response = api_instance.create_reference_profile(org_id, dataset_id, create_reference_profile_request)
         pprint(api_response)
     except whylabs_client.ApiException as e:
-        print("Exception when calling DatasetProfileApi->delete_analyzer_results: %s\n" % e)
+        print("Exception when calling DatasetProfileApi->create_reference_profile: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
+*DatasetProfileApi* | [**create_reference_profile**](docs/DatasetProfileApi.md#create_reference_profile) | **POST** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/reference-profile | Returns data needed to uploading the reference profile
 *DatasetProfileApi* | [**delete_analyzer_results**](docs/DatasetProfileApi.md#delete_analyzer_results) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/analyzer-results | Deletes a set of analyzer results
 *DatasetProfileApi* | [**delete_dataset_profiles**](docs/DatasetProfileApi.md#delete_dataset_profiles) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{dataset_id} | Deletes a set of dataset profiles
 *DatasetProfileApi* | [**delete_reference_profile**](docs/DatasetProfileApi.md#delete_reference_profile) | **DELETE** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Delete a single reference profile
 *DatasetProfileApi* | [**get_reference_profile**](docs/DatasetProfileApi.md#get_reference_profile) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles/{reference_id} | Returns a single reference profile
 *DatasetProfileApi* | [**list_reference_profiles**](docs/DatasetProfileApi.md#list_reference_profiles) | **GET** /v0/organizations/{org_id}/dataset-profiles/models/{model_id}/reference-profiles | Returns a list for reference profiles
 *DatasetMetadataApi* | [**delete_dataset_metadata**](docs/DatasetMetadataApi.md#delete_dataset_metadata) | **DELETE** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Delete dataset metadata for the specified dataset
 *DatasetMetadataApi* | [**get_dataset_metadata**](docs/DatasetMetadataApi.md#get_dataset_metadata) | **GET** /v0/organizations/{org_id}/dataset/{dataset_id}/metadata | Get dataset metadata for the specified dataset
@@ -158,14 +177,16 @@
  - [AWSMarketplaceMetadata](docs/AWSMarketplaceMetadata.md)
  - [ActionType](docs/ActionType.md)
  - [AddMembershipRequest](docs/AddMembershipRequest.md)
  - [AsyncLogResponse](docs/AsyncLogResponse.md)
  - [BatchLogReferenceRequest](docs/BatchLogReferenceRequest.md)
  - [BatchLogSessionReferenceResponse](docs/BatchLogSessionReferenceResponse.md)
  - [ColumnSchema](docs/ColumnSchema.md)
+ - [CreateReferenceProfileRequest](docs/CreateReferenceProfileRequest.md)
+ - [CreateReferenceProfileResponse](docs/CreateReferenceProfileResponse.md)
  - [CreateSessionRequest](docs/CreateSessionRequest.md)
  - [CreateSessionResponse](docs/CreateSessionResponse.md)
  - [CreateUserRequest](docs/CreateUserRequest.md)
  - [DTOClustersAutoScaleDTO](docs/DTOClustersAutoScaleDTO.md)
  - [DTOClustersAwsAttributesDTO](docs/DTOClustersAwsAttributesDTO.md)
  - [DTOClustersAwsAvailabilityDTO](docs/DTOClustersAwsAvailabilityDTO.md)
  - [DTOClustersClusterLogConfDTO](docs/DTOClustersClusterLogConfDTO.md)
```

### Comparing `whylabs-client-0.5.0/setup.py` & `whylabs-client-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from setuptools import setup, find_packages  # noqa: H301
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "RELEASE.md").read_text()
 
 NAME = "whylabs-client"
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `whylabs-client-0.5.0/whylabs_client/__init__.py` & `whylabs-client-0.5.1/whylabs_client/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 0.1
     Contact: support@whylabs.ai
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 # import ApiClient
 from whylabs_client.api_client import ApiClient
 
 # import Configuration
 from whylabs_client.configuration import Configuration
```

### Comparing `whylabs-client-0.5.0/whylabs_client/api/dataset_metadata_api.py` & `whylabs-client-0.5.1/whylabs_client/api/dataset_metadata_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/dataset_profile_api.py` & `whylabs-client-0.5.1/whylabs_client/api/dataset_profile_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     check_validations,
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
+from whylabs_client.model.create_reference_profile_request import CreateReferenceProfileRequest
+from whylabs_client.model.create_reference_profile_response import CreateReferenceProfileResponse
 from whylabs_client.model.delete_analyzer_results_response import DeleteAnalyzerResultsResponse
 from whylabs_client.model.delete_dataset_profiles_response import DeleteDatasetProfilesResponse
 from whylabs_client.model.reference_profile_item_response import ReferenceProfileItemResponse
 
 
 class DatasetProfileApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -34,14 +36,78 @@
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
+        self.create_reference_profile_endpoint = _Endpoint(
+            settings={
+                'response_type': (CreateReferenceProfileResponse,),
+                'auth': [
+                    'ApiKeyAuth'
+                ],
+                'endpoint_path': '/v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/reference-profile',
+                'operation_id': 'create_reference_profile',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'org_id',
+                    'dataset_id',
+                    'create_reference_profile_request',
+                ],
+                'required': [
+                    'org_id',
+                    'dataset_id',
+                    'create_reference_profile_request',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'org_id':
+                        (str,),
+                    'dataset_id':
+                        (str,),
+                    'create_reference_profile_request':
+                        (CreateReferenceProfileRequest,),
+                },
+                'attribute_map': {
+                    'org_id': 'org_id',
+                    'dataset_id': 'dataset_id',
+                },
+                'location_map': {
+                    'org_id': 'path',
+                    'dataset_id': 'path',
+                    'create_reference_profile_request': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.delete_analyzer_results_endpoint = _Endpoint(
             settings={
                 'response_type': (DeleteAnalyzerResultsResponse,),
                 'auth': [
                     'ApiKeyAuth'
                 ],
                 'endpoint_path': '/v0/organizations/{org_id}/dataset-profiles/models/{dataset_id}/analyzer-results',
@@ -374,14 +440,93 @@
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
+    def create_reference_profile(
+        self,
+        org_id,
+        dataset_id,
+        create_reference_profile_request,
+        **kwargs
+    ):
+        """Returns data needed to uploading the reference profile  # noqa: E501
+
+        Returns data needed to upload the reference profile. Supports uploading segmented reference profiles.              If segments are omitted, provides data needed to upload a single reference profile.              This replaces the deprecated LogReference operation.           # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_reference_profile(org_id, dataset_id, create_reference_profile_request, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            org_id (str): Your company's unique organization ID
+            dataset_id (str): The unique model ID in your company.
+            create_reference_profile_request (CreateReferenceProfileRequest):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            CreateReferenceProfileResponse
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['org_id'] = \
+            org_id
+        kwargs['dataset_id'] = \
+            dataset_id
+        kwargs['create_reference_profile_request'] = \
+            create_reference_profile_request
+        return self.create_reference_profile_endpoint.call_with_http_info(**kwargs)
+
     def delete_analyzer_results(
         self,
         org_id,
         dataset_id,
         **kwargs
     ):
         """Deletes a set of analyzer results  # noqa: E501
```

### Comparing `whylabs-client-0.5.0/whylabs_client/api/feature_weights_api.py` & `whylabs-client-0.5.1/whylabs_client/api/feature_weights_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/log_api.py` & `whylabs-client-0.5.1/whylabs_client/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/membership_api.py` & `whylabs-client-0.5.1/whylabs_client/api/membership_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/models_api.py` & `whylabs-client-0.5.1/whylabs_client/api/models_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/monitor_api.py` & `whylabs-client-0.5.1/whylabs_client/api/monitor_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/notification_settings_api.py` & `whylabs-client-0.5.1/whylabs_client/api/notification_settings_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/schema_api.py` & `whylabs-client-0.5.1/whylabs_client/api/schema_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api/sessions_api.py` & `whylabs-client-0.5.1/whylabs_client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/api_client.py` & `whylabs-client-0.5.1/whylabs_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -769,18 +769,18 @@
         return params
 
     def __call__(self, *args, **kwargs):
         """ This method is invoked when endpoints are called
         Example:
 
         api_instance = DatasetProfileApi()
-        api_instance.delete_analyzer_results  # this is an instance of the class Endpoint
-        api_instance.delete_analyzer_results()  # this invokes api_instance.delete_analyzer_results.__call__()
+        api_instance.create_reference_profile  # this is an instance of the class Endpoint
+        api_instance.create_reference_profile()  # this invokes api_instance.create_reference_profile.__call__()
         which then invokes the callable functions stored in that endpoint at
-        api_instance.delete_analyzer_results.callable or self.callable in this class
+        api_instance.create_reference_profile.callable or self.callable in this class
 
         """
         return self.callable(self, *args, **kwargs)
 
     def call_with_http_info(self, **kwargs):
 
         try:
```

### Comparing `whylabs-client-0.5.0/whylabs_client/apis/__init__.py` & `whylabs-client-0.5.1/whylabs_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/configuration.py` & `whylabs-client-0.5.1/whylabs_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1\n"\
-               "SDK Package Version: 0.5.0".\
+               "SDK Package Version: 0.5.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `whylabs-client-0.5.0/whylabs_client/exceptions.py` & `whylabs-client-0.5.1/whylabs_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/action_type.py` & `whylabs-client-0.5.1/whylabs_client/model/action_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/add_membership_request.py` & `whylabs-client-0.5.1/whylabs_client/model/add_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/async_log_response.py` & `whylabs-client-0.5.1/whylabs_client/model/async_log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/aws_marketplace_metadata.py` & `whylabs-client-0.5.1/whylabs_client/model/aws_marketplace_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/batch_log_reference_request.py` & `whylabs-client-0.5.1/whylabs_client/model/batch_log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/batch_log_session_reference_response.py` & `whylabs-client-0.5.1/whylabs_client/model/batch_log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/column_schema.py` & `whylabs-client-0.5.1/whylabs_client/model/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/create_session_request.py` & `whylabs-client-0.5.1/whylabs_client/model/create_session_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/create_session_response.py` & `whylabs-client-0.5.1/whylabs_client/model/create_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/create_user_request.py` & `whylabs-client-0.5.1/whylabs_client/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/databricks_connection.py` & `whylabs-client-0.5.1/whylabs_client/model/databricks_connection.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dataset_request_monitor_config.py` & `whylabs-client-0.5.1/whylabs_client/model/dataset_request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/datatype_monitor_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/datatype_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/delete_analyzer_results_response.py` & `whylabs-client-0.5.1/whylabs_client/model/delete_analyzer_results_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/delete_dataset_profiles_response.py` & `whylabs-client-0.5.1/whylabs_client/model/delete_dataset_profiles_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/distribution_monitor_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/distribution_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_auto_scale_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_clusters_auto_scale_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_attributes_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_clusters_aws_attributes_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_aws_availability_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_clusters_aws_availability_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_clusters_cluster_log_conf_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_clusters_dbfs_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_clusters_s3_storage_info_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_clusters_s3_storage_info_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_ebs_volume_type_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_ebs_volume_type_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_cron_schedule_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_cron_schedule_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_data_security_mode_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_data_security_mode_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_job_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_email_notifications_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_job_email_notifications_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_job_settings_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_job_settings_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_new_cluster_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_new_cluster_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_notebook_task_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_notebook_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_jar_task_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_spark_jar_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_python_task_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_spark_python_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/dto_jobs_spark_submit_task_dto.py` & `whylabs-client-0.5.1/whylabs_client/model/dto_jobs_spark_submit_task_dto.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/email_notification_action.py` & `whylabs-client-0.5.1/whylabs_client/model/email_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/entity_schema.py` & `whylabs-client-0.5.1/whylabs_client/model/entity_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/entity_search_result.py` & `whylabs-client-0.5.1/whylabs_client/model/entity_search_result.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/entity_weight_record.py` & `whylabs-client-0.5.1/whylabs_client/model/entity_weight_record.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/entity_weight_record_metadata.py` & `whylabs-client-0.5.1/whylabs_client/model/entity_weight_record_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/feature_flags.py` & `whylabs-client-0.5.1/whylabs_client/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_connection_request.py` & `whylabs-client-0.5.1/whylabs_client/model/get_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_connection_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_dataset_metadata_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_dataset_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_default_membership_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_default_membership_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_marketplace_metadata_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_marketplace_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_memberships_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_monitor_config_v2_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_monitor_config_v2_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_notification_settings_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_notification_settings_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/get_session_response.py` & `whylabs-client-0.5.1/whylabs_client/model/get_session_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/list_jobs_request.py` & `whylabs-client-0.5.1/whylabs_client/model/list_jobs_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/list_jobs_response.py` & `whylabs-client-0.5.1/whylabs_client/model/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/list_models_response.py` & `whylabs-client-0.5.1/whylabs_client/model/list_models_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/list_organization_memberships_response.py` & `whylabs-client-0.5.1/whylabs_client/model/list_organization_memberships_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/list_user_api_keys.py` & `whylabs-client-0.5.1/whylabs_client/model/list_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/log_async_request.py` & `whylabs-client-0.5.1/whylabs_client/model/log_async_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/log_reference_request.py` & `whylabs-client-0.5.1/whylabs_client/model/log_reference_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/log_reference_response.py` & `whylabs-client-0.5.1/whylabs_client/model/log_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/log_response.py` & `whylabs-client-0.5.1/whylabs_client/model/log_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/log_session_reference_response.py` & `whylabs-client-0.5.1/whylabs_client/model/log_session_reference_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/marketplace_dimensions.py` & `whylabs-client-0.5.1/whylabs_client/model/marketplace_dimensions.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/membership.py` & `whylabs-client-0.5.1/whylabs_client/model/membership.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/membership_metadata.py` & `whylabs-client-0.5.1/whylabs_client/model/membership_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/metric_schema.py` & `whylabs-client-0.5.1/whylabs_client/model/metric_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/missing_recent_data_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/missing_recent_data_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/missing_recent_profiles_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/missing_recent_profiles_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/missing_values_monitor_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/missing_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/model_metadata_response.py` & `whylabs-client-0.5.1/whylabs_client/model/model_metadata_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/model_type.py` & `whylabs-client-0.5.1/whylabs_client/model/model_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/monitor_config.py` & `whylabs-client-0.5.1/whylabs_client/model/monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/monitor_config_version.py` & `whylabs-client-0.5.1/whylabs_client/model/monitor_config_version.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference.py` & `whylabs-client-0.5.1/whylabs_client/model/monitor_request_reference.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/monitor_request_reference_type.py` & `whylabs-client-0.5.1/whylabs_client/model/monitor_request_reference_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/notification_action.py` & `whylabs-client-0.5.1/whylabs_client/model/notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/notification_settings.py` & `whylabs-client-0.5.1/whylabs_client/model/notification_settings.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/notification_settings_day.py` & `whylabs-client-0.5.1/whylabs_client/model/notification_settings_day.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/notification_sqs_message_cadence.py` & `whylabs-client-0.5.1/whylabs_client/model/notification_sqs_message_cadence.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/organization_metadata.py` & `whylabs-client-0.5.1/whylabs_client/model/organization_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/organization_summary.py` & `whylabs-client-0.5.1/whylabs_client/model/organization_summary.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/pager_duty_notification_action.py` & `whylabs-client-0.5.1/whylabs_client/model/pager_duty_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provided_config.py` & `whylabs-client-0.5.1/whylabs_client/model/provided_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_request.py` & `whylabs-client-0.5.1/whylabs_client/model/provision_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provision_databricks_connection_response.py` & `whylabs-client-0.5.1/whylabs_client/model/provision_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provision_new_aws_marketplace_user_response.py` & `whylabs-client-0.5.1/whylabs_client/model/provision_new_aws_marketplace_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provision_new_marketplace_user_request.py` & `whylabs-client-0.5.1/whylabs_client/model/provision_new_marketplace_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provision_new_user_request.py` & `whylabs-client-0.5.1/whylabs_client/model/provision_new_user_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/provision_new_user_response.py` & `whylabs-client-0.5.1/whylabs_client/model/provision_new_user_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/reference_profile_item_response.py` & `whylabs-client-0.5.1/whylabs_client/model/create_reference_profile_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from whylabs_client.exceptions import ApiAttributeError
 
 
 
-class ReferenceProfileItemResponse(ModelNormal):
+class CreateReferenceProfileResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,47 +78,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'org_id': (str,),  # noqa: E501
-            'model_id': (str,),  # noqa: E501
-            'alias': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
+            'alias': (str,),  # noqa: E501
+            'dataset_id': (str,),  # noqa: E501
             'upload_timestamp': (int,),  # noqa: E501
-            'dataset_timestamp': (int, none_type,),  # noqa: E501
-            'download_url': (str, none_type,),  # noqa: E501
+            'segments': ([str],),  # noqa: E501
+            'upload_urls': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'org_id': 'orgId',  # noqa: E501
-        'model_id': 'modelId',  # noqa: E501
-        'alias': 'alias',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'alias': 'alias',  # noqa: E501
+        'dataset_id': 'datasetId',  # noqa: E501
         'upload_timestamp': 'uploadTimestamp',  # noqa: E501
-        'dataset_timestamp': 'datasetTimestamp',  # noqa: E501
-        'download_url': 'downloadUrl',  # noqa: E501
+        'segments': 'segments',  # noqa: E501
+        'upload_urls': 'uploadUrls',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ReferenceProfileItemResponse - a model defined in OpenAPI
+        """CreateReferenceProfileResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -143,21 +141,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str): [optional]  # noqa: E501
-            model_id (str): [optional]  # noqa: E501
-            alias (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
+            alias (str): [optional]  # noqa: E501
+            dataset_id (str): [optional]  # noqa: E501
             upload_timestamp (int): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            download_url (str, none_type): [optional]  # noqa: E501
+            segments ([str]): [optional]  # noqa: E501
+            upload_urls ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -198,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ReferenceProfileItemResponse - a model defined in OpenAPI
+        """CreateReferenceProfileResponse - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -231,21 +228,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            org_id (str): [optional]  # noqa: E501
-            model_id (str): [optional]  # noqa: E501
-            alias (str): [optional]  # noqa: E501
             id (str): [optional]  # noqa: E501
+            alias (str): [optional]  # noqa: E501
+            dataset_id (str): [optional]  # noqa: E501
             upload_timestamp (int): [optional]  # noqa: E501
-            dataset_timestamp (int, none_type): [optional]  # noqa: E501
-            download_url (str, none_type): [optional]  # noqa: E501
+            segments ([str]): [optional]  # noqa: E501
+            upload_urls ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `whylabs-client-0.5.0/whylabs_client/model/refresh_access_token_request.py` & `whylabs-client-0.5.1/whylabs_client/model/refresh_access_token_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/refresh_connection_by_org_id_response.py` & `whylabs-client-0.5.1/whylabs_client/model/refresh_connection_by_org_id_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/refresh_connection_request.py` & `whylabs-client-0.5.1/whylabs_client/model/refresh_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_request.py` & `whylabs-client-0.5.1/whylabs_client/model/register_databricks_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/register_databricks_connection_response.py` & `whylabs-client-0.5.1/whylabs_client/model/register_databricks_connection_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/remove_membership_request.py` & `whylabs-client-0.5.1/whylabs_client/model/remove_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/request_feature_monitor_config.py` & `whylabs-client-0.5.1/whylabs_client/model/request_feature_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/request_monitor_config.py` & `whylabs-client-0.5.1/whylabs_client/model/request_monitor_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/response.py` & `whylabs-client-0.5.1/whylabs_client/model/response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/role.py` & `whylabs-client-0.5.1/whylabs_client/model/role.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/run_job_request.py` & `whylabs-client-0.5.1/whylabs_client/model/run_job_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/run_job_response.py` & `whylabs-client-0.5.1/whylabs_client/model/run_job_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/schema_metadata.py` & `whylabs-client-0.5.1/whylabs_client/model/schema_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/search_index_request.py` & `whylabs-client-0.5.1/whylabs_client/model/search_index_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/search_index_type.py` & `whylabs-client-0.5.1/whylabs_client/model/search_index_type.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/search_response.py` & `whylabs-client-0.5.1/whylabs_client/model/search_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/seasonal_arima_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/seasonal_arima_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/segment.py` & `whylabs-client-0.5.1/whylabs_client/model/segment.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/segment_tag.py` & `whylabs-client-0.5.1/whylabs_client/model/segment_tag.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/segment_weight.py` & `whylabs-client-0.5.1/whylabs_client/model/segment_weight.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/session_metadata.py` & `whylabs-client-0.5.1/whylabs_client/model/session_metadata.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/set_default_membership_request.py` & `whylabs-client-0.5.1/whylabs_client/model/set_default_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/slack_notification_action.py` & `whylabs-client-0.5.1/whylabs_client/model/slack_notification_action.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/subscription_tier.py` & `whylabs-client-0.5.1/whylabs_client/model/subscription_tier.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/time_period.py` & `whylabs-client-0.5.1/whylabs_client/model/time_period.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/uber_notification_schedule.py` & `whylabs-client-0.5.1/whylabs_client/model/uber_notification_schedule.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/unique_values_monitor_request_config.py` & `whylabs-client-0.5.1/whylabs_client/model/unique_values_monitor_request_config.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/update_connection_changes.py` & `whylabs-client-0.5.1/whylabs_client/model/update_connection_changes.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/update_connection_request.py` & `whylabs-client-0.5.1/whylabs_client/model/update_connection_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/update_membership_request.py` & `whylabs-client-0.5.1/whylabs_client/model/update_membership_request.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/user.py` & `whylabs-client-0.5.1/whylabs_client/model/user.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/user_api_key.py` & `whylabs-client-0.5.1/whylabs_client/model/user_api_key.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/user_api_key_response.py` & `whylabs-client-0.5.1/whylabs_client/model/user_api_key_response.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model/why_logs_metric.py` & `whylabs-client-0.5.1/whylabs_client/model/why_logs_metric.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/model_utils.py` & `whylabs-client-0.5.1/whylabs_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client/models/__init__.py` & `whylabs-client-0.5.1/whylabs_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from whylabs_client.model.aws_marketplace_metadata import AWSMarketplaceMetadata
 from whylabs_client.model.action_type import ActionType
 from whylabs_client.model.add_membership_request import AddMembershipRequest
 from whylabs_client.model.async_log_response import AsyncLogResponse
 from whylabs_client.model.batch_log_reference_request import BatchLogReferenceRequest
 from whylabs_client.model.batch_log_session_reference_response import BatchLogSessionReferenceResponse
 from whylabs_client.model.column_schema import ColumnSchema
+from whylabs_client.model.create_reference_profile_request import CreateReferenceProfileRequest
+from whylabs_client.model.create_reference_profile_response import CreateReferenceProfileResponse
 from whylabs_client.model.create_session_request import CreateSessionRequest
 from whylabs_client.model.create_session_response import CreateSessionResponse
 from whylabs_client.model.create_user_request import CreateUserRequest
 from whylabs_client.model.dto_clusters_auto_scale_dto import DTOClustersAutoScaleDTO
 from whylabs_client.model.dto_clusters_aws_attributes_dto import DTOClustersAwsAttributesDTO
 from whylabs_client.model.dto_clusters_aws_availability_dto import DTOClustersAwsAvailabilityDTO
 from whylabs_client.model.dto_clusters_cluster_log_conf_dto import DTOClustersClusterLogConfDTO
```

### Comparing `whylabs-client-0.5.0/whylabs_client/rest.py` & `whylabs-client-0.5.1/whylabs_client/rest.py`

 * *Files identical despite different names*

### Comparing `whylabs-client-0.5.0/whylabs_client.egg-info/PKG-INFO` & `whylabs-client-0.5.1/whylabs_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-client
-Version: 0.5.0
+Version: 0.5.1
 Summary: WhyLabs API client
 Home-page: UNKNOWN
 Author: WhyLabs
 Author-email: support@whylabs.ai
 License: Apache License 2.0
 Keywords: OpenAPI,OpenAPI-Generator,WhyLabs API client
 Platform: UNKNOWN
@@ -75,14 +75,15 @@
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
 # Configure API key authorization: ApiKeyAuth
 configuration.api_key['ApiKeyAuth'] = 'YOUR_API_KEY'
+configuration.discard_unknown_keys = True
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['ApiKeyAuth'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
 with whylabs_client.ApiClient(configuration) as api_client:
```

### Comparing `whylabs-client-0.5.0/whylabs_client.egg-info/SOURCES.txt` & `whylabs-client-0.5.1/whylabs_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 whylabs_client/model/action_type.py
 whylabs_client/model/add_membership_request.py
 whylabs_client/model/async_log_response.py
 whylabs_client/model/aws_marketplace_metadata.py
 whylabs_client/model/batch_log_reference_request.py
 whylabs_client/model/batch_log_session_reference_response.py
 whylabs_client/model/column_schema.py
+whylabs_client/model/create_reference_profile_request.py
+whylabs_client/model/create_reference_profile_response.py
 whylabs_client/model/create_session_request.py
 whylabs_client/model/create_session_response.py
 whylabs_client/model/create_user_request.py
 whylabs_client/model/databricks_connection.py
 whylabs_client/model/dataset_request_monitor_config.py
 whylabs_client/model/datatype_monitor_request_config.py
 whylabs_client/model/delete_analyzer_results_response.py
```

