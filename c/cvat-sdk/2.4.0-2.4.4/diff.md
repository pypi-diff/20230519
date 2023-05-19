# Comparing `tmp/cvat_sdk-2.4.0.tar.gz` & `tmp/cvat_sdk-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_sdk-2.4.0.tar", last modified: Thu Mar 16 09:12:09 2023, max compression
+gzip compressed data, was "cvat_sdk-2.4.4.tar", last modified: Fri May 19 11:29:16 2023, max compression
```

## Comparing `cvat_sdk-2.4.0.tar` & `cvat_sdk-2.4.4.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.754482 cvat_sdk-2.4.0/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-03-16 08:50:27.000000 cvat_sdk-2.4.0/MANIFEST.in
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-03-16 09:12:09.754482 cvat_sdk-2.4.0/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-03-16 08:50:27.000000 cvat_sdk-2.4.0/README.md
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.724482 cvat_sdk-2.4.0/cvat_sdk/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.724482 cvat_sdk-2.4.0/cvat_sdk/api_client/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      765 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/__init__.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.724482 cvat_sdk-2.4.0/cvat_sdk/api_client/api/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      501 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    52058 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/auth_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    59367 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/cloudstorages_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33762 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/comments_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15633 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/events_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33077 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/invitations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    34252 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/issues_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    93976 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/jobs_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    28985 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/labels_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    36762 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/lambda_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    27242 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/memberships_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33686 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/organizations_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    92819 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/projects_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11303 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/schema_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    24039 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/server_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)   161610 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/tasks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    33152 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/users_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    72956 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api/webhooks_api.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    45214 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/api_client.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.724482 cvat_sdk-2.4.0/cvat_sdk/api_client/apis/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1709 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/apis/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19675 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/configuration.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5135 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/exceptions.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/cvat_sdk/api_client/model/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13040 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/about.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12458 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/annotation_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15638 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/annotations_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14197 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13993 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12610 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute_val.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12645 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute_val_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14270 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/backup_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14110 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/basic_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13572 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/basic_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12785 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/chunk_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12997 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/client_events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13103 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/client_events_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17363 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/cloud_storage_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17876 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14261 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/comment_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15466 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/comment_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12656 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12741 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/comments_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13253 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/credentials_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15259 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/data_meta_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23386 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12404 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13646 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_format.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12997 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_formats.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14274 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18296 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/event.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18847 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/event_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12986 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/events.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15021 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/events_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13184 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/file_info.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12703 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/file_info_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13642 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/frame_meta.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12969 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/input_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14182 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/invitation_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12805 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15952 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/issue_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14032 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12731 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/issues_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16286 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    20941 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15462 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_read_assignee.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12871 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_stage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12869 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13213 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/jobs_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17308 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/label.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14502 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_data.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14750 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14730 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_image.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14899 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_image_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18092 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18332 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15749 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16060 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12731 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/labels_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12767 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/location_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13018 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/login_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14904 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/membership_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17614 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/meta_user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12581 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/online_function_call_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12953 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/operation_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15422 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/organization_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13860 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13672 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_comment_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13641 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_invitation_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13566 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_issue_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13536 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_job_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13505 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_label_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13641 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_membership_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13551 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_meta_user_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13671 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_organization_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_project_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13551 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_task_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13717 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13596 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_webhook_read_list.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13431 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/password_change_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13632 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/password_reset_confirm_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12415 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17803 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12395 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_comment_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12416 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_data_meta_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12864 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_invitation_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13435 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_issue_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13340 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_job_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16558 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_label_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14785 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_labeled_data_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12512 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_membership_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13895 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_organization_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16057 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14843 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16207 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14830 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16214 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_user_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15353 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13267 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/plugins.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12404 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    19104 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15467 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_read_owner.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14942 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16022 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13161 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/provider_type_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13361 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/register_serializer_ex.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14359 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/register_serializer_ex_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12296 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/rest_auth_detail.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12918 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/role_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13562 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/rq_status.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12935 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/rq_status_state_enum.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13251 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/shape_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12297 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/signing_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12992 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sorting_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13334 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12758 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage_method.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13072 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12837 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17566 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17735 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15223 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_track.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15463 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_track_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15277 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sublabel.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15412 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/sublabel_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16289 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_annotations_update_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14336 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_annotations_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12350 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_file_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    23629 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14930 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_read_target_storage.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17121 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12726 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/tasks_summary.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12253 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/token.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16247 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/tracked_shape.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16353 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/tracked_shape_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    17569 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/user.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12548 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_content_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    16361 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_delivery_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    18533 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_read.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    12769 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_type.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    15739 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_write_request.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    84564 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/model_utils.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/cvat_sdk/api_client/models/
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13503 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/models/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14473 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/api_client/rest.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/cvat_sdk/core/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11842 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/client.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3113 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/downloading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/git.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/helpers.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/progress.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/cvat_sdk/core/proxies/
--rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/annotations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/issues.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/jobs.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/model_proxy.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/organizations.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/projects.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    14224 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/tasks.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/proxies/users.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    13947 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/uploading.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/core/utils.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/exceptions.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/models.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/cvat_sdk/pytorch/
--rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/pytorch/__init__.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/pytorch/caching.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/pytorch/common.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/pytorch/project_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/pytorch/task_dataset.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/pytorch/transforms.py
--rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/cvat_sdk/version.py
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/cvat_sdk.egg-info/
--rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-03-16 09:12:09.000000 cvat_sdk-2.4.0/cvat_sdk.egg-info/PKG-INFO
--rw-r--r--   0 andrey    (1000) andrey    (1000)     9179 2023-03-16 09:12:09.000000 cvat_sdk-2.4.0/cvat_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-03-16 09:12:09.000000 cvat_sdk-2.4.0/cvat_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-03-16 09:12:09.000000 cvat_sdk-2.4.0/cvat_sdk.egg-info/requires.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-03-16 09:12:09.000000 cvat_sdk-2.4.0/cvat_sdk.egg-info/top_level.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2023-03-16 08:50:27.000000 cvat_sdk-2.4.0/pyproject.toml
-drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-03-16 09:12:09.744482 cvat_sdk-2.4.0/requirements/
--rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/requirements/api_client.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-03-16 08:50:27.000000 cvat_sdk-2.4.0/requirements/base.txt
--rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-03-16 09:12:09.754482 cvat_sdk-2.4.0/setup.cfg
--rw-r--r--   0 andrey    (1000) andrey    (1000)     2751 2023-03-16 09:11:04.000000 cvat_sdk-2.4.0/setup.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       83 2023-04-05 10:02:25.000000 cvat_sdk-2.4.4/MANIFEST.in
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      989 2023-04-05 10:02:25.000000 cvat_sdk-2.4.4/README.md
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.051894 cvat_sdk-2.4.4/cvat_sdk/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.061894 cvat_sdk-2.4.4/cvat_sdk/api_client/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      767 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/__init__.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.061894 cvat_sdk-2.4.4/cvat_sdk/api_client/api/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      503 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    51130 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/auth_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    59211 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/cloudstorages_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33454 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/comments_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15480 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/events_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    32769 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/invitations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33944 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/issues_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    86553 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/jobs_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    28832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/labels_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    36609 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/lambda_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    27089 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/memberships_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    33378 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/organizations_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    78780 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/projects_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11305 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/schema_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    24041 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/server_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)   140016 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/tasks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    32999 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/users_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    72493 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api/webhooks_api.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    45222 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/api_client.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.061894 cvat_sdk-2.4.4/cvat_sdk/api_client/apis/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1711 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/apis/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19679 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/configuration.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5132 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/exceptions.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.071894 cvat_sdk-2.4.4/cvat_sdk/api_client/model/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13042 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/about.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12460 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotation_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15640 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotations_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14199 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13995 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12612 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12647 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14272 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/backup_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14112 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13574 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12787 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/chunk_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13105 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17365 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18328 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14263 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15468 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12658 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12743 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/comments_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13414 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/credentials_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15261 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_meta_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    28377 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13648 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_format.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12999 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_formats.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14276 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18298 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/event.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18849 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/event_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12988 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/events.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15575 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/events_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13186 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12705 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13644 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/frame_meta.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12971 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/input_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14184 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12807 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15954 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14034 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/issues_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16288 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    20943 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15464 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read_assignee.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12873 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_stage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12871 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13215 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/jobs_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17310 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/label.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14504 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14752 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14732 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14901 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18094 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18334 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15751 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16062 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12590 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/labels_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12769 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/location_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13020 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/login_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14906 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/membership_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17616 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/meta_user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12583 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/online_function_call_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12955 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/operation_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15424 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13862 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13674 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_comment_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_invitation_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13568 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_issue_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13538 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_job_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13507 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_label_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13643 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_membership_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_meta_user_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13673 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_organization_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_project_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13553 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_task_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13719 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13598 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_read_list.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13433 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_change_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13634 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_confirm_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12417 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18255 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12397 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_comment_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12418 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_data_meta_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12866 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_invitation_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13069 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_issue_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13342 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_job_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16560 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_label_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14787 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_labeled_data_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12514 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_membership_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13897 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_organization_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16059 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14845 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16209 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16216 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_user_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14962 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13269 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/plugins.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12406 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    19106 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15469 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_owner.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14944 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16024 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13163 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/provider_type_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13363 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14361 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12298 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/rest_auth_detail.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12920 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/role_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13564 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12937 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status_state_enum.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13253 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/shape_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12299 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/signing_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12994 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sorting_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13336 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12760 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_method.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13074 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12839 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17568 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17737 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15225 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15465 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15279 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15414 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16291 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_update_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14338 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12352 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_file_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    23631 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14932 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read_target_storage.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17123 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12728 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/tasks_summary.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12255 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/token.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16249 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16355 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    17571 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/user.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12550 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_content_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    16363 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_delivery_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    18535 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_read.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12771 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_type.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    15742 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_write_request.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    84566 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/model_utils.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.071894 cvat_sdk-2.4.4/cvat_sdk/api_client/models/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13505 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/models/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14475 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/api_client/rest.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk/core/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      188 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    12038 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/client.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3115 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/downloading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      353 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/git.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3061 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/helpers.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     3147 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/progress.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk/core/proxies/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2116 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/annotations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1737 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/issues.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5550 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/jobs.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     5824 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/model_proxy.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      967 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/organizations.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6652 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/projects.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    14224 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/tasks.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      832 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/proxies/users.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    13947 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/uploading.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2103 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/core/utils.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      325 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/exceptions.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      167 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/models.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk/pytorch/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      362 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/__init__.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)    11405 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/caching.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      969 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/common.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     4303 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/project_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     6982 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/task_dataset.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2885 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/pytorch/transforms.py
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       18 2023-05-19 11:27:40.000000 cvat_sdk-2.4.4/cvat_sdk/version.py
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/cvat_sdk.egg-info/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     1463 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     9179 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        1 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      202 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/requires.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)        9 2023-05-19 11:29:16.000000 cvat_sdk-2.4.4/cvat_sdk.egg-info/top_level.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      383 2022-12-22 11:37:46.000000 cvat_sdk-2.4.4/pyproject.toml
+drwxr-xr-x   0 andrey    (1000) andrey    (1000)        0 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/requirements/
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       64 2023-05-19 11:27:39.000000 cvat_sdk-2.4.4/requirements/api_client.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)      206 2023-04-05 10:02:25.000000 cvat_sdk-2.4.4/requirements/base.txt
+-rw-r--r--   0 andrey    (1000) andrey    (1000)       38 2023-05-19 11:29:16.081894 cvat_sdk-2.4.4/setup.cfg
+-rw-r--r--   0 andrey    (1000) andrey    (1000)     2753 2023-05-19 11:27:39.000000 cvat_sdk-2.4.4/setup.py
```

### Comparing `cvat_sdk-2.4.0/PKG-INFO` & `cvat_sdk-2.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat_sdk
-Version: 2.4.0
+Version: 2.4.4
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.0/README.md` & `cvat_sdk-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/__init__.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
-__version__ = "2.4.0"
+__version__ = "2.4.4"
 
 from cvat_sdk.api_client.api_client import ApiClient
 
 from cvat_sdk.api_client.configuration import Configuration
 
 from cvat_sdk.api_client.exceptions import OpenApiException
 from cvat_sdk.api_client.exceptions import ApiAttributeError
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/auth_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/auth_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -115,18 +115,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_logout_endpoint = _Endpoint(
             settings={
                 'response_schema': (RestAuthDetail,),
@@ -252,18 +249,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_password_reset_endpoint = _Endpoint(
             settings={
                 'response_schema': (RestAuthDetail,),
@@ -326,18 +320,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_password_reset_confirm_endpoint = _Endpoint(
             settings={
                 'response_schema': (RestAuthDetail,),
@@ -400,18 +391,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_register_endpoint = _Endpoint(
             settings={
                 'response_schema': (RegisterSerializerEx,),
@@ -474,18 +462,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_signing_endpoint = _Endpoint(
             settings={
                 'response_schema': (str,),
@@ -548,18 +533,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_rules_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/cloudstorages_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/cloudstorages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -111,17 +111,15 @@
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -236,15 +234,16 @@
                 },
                 'allowed_values': {
                     ('credentials_type',): {
 
                         "KEY_SECRET_KEY_PAIR": "KEY_SECRET_KEY_PAIR",
                         "ACCOUNT_NAME_TOKEN_PAIR": "ACCOUNT_NAME_TOKEN_PAIR",
                         "KEY_FILE_PATH": "KEY_FILE_PATH",
-                        "ANONYMOUS_ACCESS": "ANONYMOUS_ACCESS"
+                        "ANONYMOUS_ACCESS": "ANONYMOUS_ACCESS",
+                        "CONNECTION_STRING": "CONNECTION_STRING"
                     },
                     ('provider_type',): {
 
                         "AWS_S3_BUCKET": "AWS_S3_BUCKET",
                         "AZURE_CONTAINER": "AZURE_CONTAINER",
                         "GOOGLE_DRIVE": "GOOGLE_DRIVE",
                         "GOOGLE_CLOUD_STORAGE": "GOOGLE_CLOUD_STORAGE"
@@ -387,17 +386,15 @@
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (CloudStorageRead,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/comments_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/comments_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -110,18 +110,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -365,18 +362,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (CommentRead,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/events_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -108,18 +108,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.list_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/invitations_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/invitations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -110,18 +110,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -350,18 +347,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (InvitationRead,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/issues_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/issues_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -110,18 +110,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -375,18 +372,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (IssueRead,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/jobs_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/jobs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -150,17 +150,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.destroy_annotations_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -445,18 +443,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.partial_update_annotations_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -536,107 +531,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
-                ]
-            },
-            api_client=api_client
-        )
-        self.partial_update_annotations_file_endpoint = _Endpoint(
-            settings={
-                'response_schema': None,
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/jobs/{id}/annotations/{file_id}',
-                'operation_id': 'partial_update_annotations_file',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'file_id',
-                    'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'body',
-                ],
-                'required': [
-                    'file_id',
-                    'id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'file_id',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('file_id',): {
-
-                        'regex': {
-                            'pattern': r'^\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b$',  # noqa: E501
-                        },
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'file_id':
-                        (str,),
-                    'id':
-                        (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'body':
-                        (file_type,),
-                },
-                'attribute_map': {
-                    'file_id': 'file_id',
-                    'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'file_id': 'path',
-                    'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (JobRead,),
@@ -1237,17 +1140,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
 
     def create_annotations(
         self,
@@ -1672,99 +1573,14 @@
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['action'] = action
         kwargs['id'] = id
         return self.partial_update_annotations_endpoint.call_with_http_info(**kwargs)
 
-    def partial_update_annotations_file(
-        self,
-        file_id: str,
-        id: int,
-        *,
-        _parse_response: bool = True,
-        _request_timeout: typing.Union[int, float, tuple] = None,
-        _validate_inputs: bool = True,
-        _validate_outputs: bool = True,
-        _check_status: bool = True,
-        _spec_property_naming: bool = False,
-        _content_type: typing.Optional[str] = None,
-        _host_index: typing.Optional[int] = None,
-        _request_auths: typing.Optional[typing.List] = None,
-        _async_call: bool = False,
-        **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Allows to upload an annotation file chunk. Implements TUS file uploading protocol.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass _async_call=True
-
-        >>> thread = api.partial_update_annotations_file(file_id, id, _async_call=True)
-        >>> result = thread.get()
-
-        Args:
-            file_id (str):
-            id (int): A unique integer value identifying this job.
-
-        Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            body (file_type): [optional]
-            _parse_response (bool): if False, the response data will not be parsed,
-                None is returned for data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _validate_inputs (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _validate_outputs (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _check_status (bool): whether to check response status
-                for being positive or not.
-                Default is True
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            _async_call (bool): execute request asynchronously
-
-        Returns:
-            (None, HTTPResponse)
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['_async_call'] = _async_call
-        kwargs['_parse_response'] = _parse_response
-        kwargs['_request_timeout'] = _request_timeout
-        kwargs['_validate_inputs'] = _validate_inputs
-        kwargs['_validate_outputs'] = _validate_outputs
-        kwargs['_check_status'] = _check_status
-        kwargs['_spec_property_naming'] = _spec_property_naming
-        kwargs['_content_type'] = _content_type
-        kwargs['_host_index'] = _host_index
-        kwargs['_request_auths'] = _request_auths
-        kwargs['file_id'] = file_id
-        kwargs['id'] = id
-        return self.partial_update_annotations_file_endpoint.call_with_http_info(**kwargs)
-
     def retrieve(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/labels_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/labels_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -324,18 +324,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (Label,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/lambda_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/lambda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -117,18 +117,15 @@
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_requests_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/memberships_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/memberships_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -288,18 +288,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (MembershipRead,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/organizations_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/organizations_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -110,18 +110,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -360,18 +357,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (OrganizationRead,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/projects_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/projects_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -113,18 +113,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_backup_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -206,17 +203,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.create_dataset_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -315,17 +310,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -576,192 +569,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
-                ]
-            },
-            api_client=api_client
-        )
-        self.partial_update_backup_file_endpoint = _Endpoint(
-            settings={
-                'response_schema': None,
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/projects/backup/{file_id}',
-                'operation_id': 'partial_update_backup_file',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'file_id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'body',
-                ],
-                'required': [
-                    'file_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'file_id',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('file_id',): {
-
-                        'regex': {
-                            'pattern': r'^\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b$',  # noqa: E501
-                        },
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'file_id':
-                        (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'body':
-                        (file_type,),
-                },
-                'attribute_map': {
-                    'file_id': 'file_id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'file_id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
-                ]
-            },
-            api_client=api_client
-        )
-        self.partial_update_dataset_file_endpoint = _Endpoint(
-            settings={
-                'response_schema': None,
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/projects/{id}/dataset/{file_id}',
-                'operation_id': 'partial_update_dataset_file',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'file_id',
-                    'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'body',
-                ],
-                'required': [
-                    'file_id',
-                    'id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'file_id',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('file_id',): {
-
-                        'regex': {
-                            'pattern': r'^\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b$',  # noqa: E501
-                        },
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'file_id':
-                        (str,),
-                    'id':
-                        (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'body':
-                        (file_type,),
-                },
-                'attribute_map': {
-                    'file_id': 'file_id',
-                    'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'file_id': 'path',
-                    'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (ProjectRead,),
@@ -1723,181 +1539,14 @@
         kwargs['_spec_property_naming'] = _spec_property_naming
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['id'] = id
         return self.partial_update_endpoint.call_with_http_info(**kwargs)
 
-    def partial_update_backup_file(
-        self,
-        file_id: str,
-        *,
-        _parse_response: bool = True,
-        _request_timeout: typing.Union[int, float, tuple] = None,
-        _validate_inputs: bool = True,
-        _validate_outputs: bool = True,
-        _check_status: bool = True,
-        _spec_property_naming: bool = False,
-        _content_type: typing.Optional[str] = None,
-        _host_index: typing.Optional[int] = None,
-        _request_auths: typing.Optional[typing.List] = None,
-        _async_call: bool = False,
-        **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Allows to upload a file chunk. Implements TUS file uploading protocol.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass _async_call=True
-
-        >>> thread = api.partial_update_backup_file(file_id, _async_call=True)
-        >>> result = thread.get()
-
-        Args:
-            file_id (str):
-
-        Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            body (file_type): [optional]
-            _parse_response (bool): if False, the response data will not be parsed,
-                None is returned for data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _validate_inputs (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _validate_outputs (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _check_status (bool): whether to check response status
-                for being positive or not.
-                Default is True
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            _async_call (bool): execute request asynchronously
-
-        Returns:
-            (None, HTTPResponse)
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['_async_call'] = _async_call
-        kwargs['_parse_response'] = _parse_response
-        kwargs['_request_timeout'] = _request_timeout
-        kwargs['_validate_inputs'] = _validate_inputs
-        kwargs['_validate_outputs'] = _validate_outputs
-        kwargs['_check_status'] = _check_status
-        kwargs['_spec_property_naming'] = _spec_property_naming
-        kwargs['_content_type'] = _content_type
-        kwargs['_host_index'] = _host_index
-        kwargs['_request_auths'] = _request_auths
-        kwargs['file_id'] = file_id
-        return self.partial_update_backup_file_endpoint.call_with_http_info(**kwargs)
-
-    def partial_update_dataset_file(
-        self,
-        file_id: str,
-        id: int,
-        *,
-        _parse_response: bool = True,
-        _request_timeout: typing.Union[int, float, tuple] = None,
-        _validate_inputs: bool = True,
-        _validate_outputs: bool = True,
-        _check_status: bool = True,
-        _spec_property_naming: bool = False,
-        _content_type: typing.Optional[str] = None,
-        _host_index: typing.Optional[int] = None,
-        _request_auths: typing.Optional[typing.List] = None,
-        _async_call: bool = False,
-        **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Allows to upload a file chunk. Implements TUS file uploading protocol.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass _async_call=True
-
-        >>> thread = api.partial_update_dataset_file(file_id, id, _async_call=True)
-        >>> result = thread.get()
-
-        Args:
-            file_id (str):
-            id (int): A unique integer value identifying this project.
-
-        Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            body (file_type): [optional]
-            _parse_response (bool): if False, the response data will not be parsed,
-                None is returned for data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _validate_inputs (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _validate_outputs (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _check_status (bool): whether to check response status
-                for being positive or not.
-                Default is True
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            _async_call (bool): execute request asynchronously
-
-        Returns:
-            (None, HTTPResponse)
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['_async_call'] = _async_call
-        kwargs['_parse_response'] = _parse_response
-        kwargs['_request_timeout'] = _request_timeout
-        kwargs['_validate_inputs'] = _validate_inputs
-        kwargs['_validate_outputs'] = _validate_outputs
-        kwargs['_check_status'] = _check_status
-        kwargs['_spec_property_naming'] = _spec_property_naming
-        kwargs['_content_type'] = _content_type
-        kwargs['_host_index'] = _host_index
-        kwargs['_request_auths'] = _request_auths
-        kwargs['file_id'] = file_id
-        kwargs['id'] = id
-        return self.partial_update_dataset_file_endpoint.call_with_http_info(**kwargs)
-
     def retrieve(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/schema_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/server_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/tasks_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/tasks_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -125,18 +125,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_endpoint = _Endpoint(
             settings={
                 'response_schema': (TaskRead,),
@@ -199,18 +196,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_annotations_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -309,17 +303,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.create_backup_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -402,17 +394,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.create_data_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -495,17 +485,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.destroy_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -860,18 +848,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.partial_update_annotations_endpoint = _Endpoint(
             settings={
                 'response_schema': (LabeledData,),
@@ -953,281 +938,15 @@
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
-                ]
-            },
-            api_client=api_client
-        )
-        self.partial_update_annotations_file_endpoint = _Endpoint(
-            settings={
-                'response_schema': None,
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/tasks/{id}/annotations/{file_id}',
-                'operation_id': 'partial_update_annotations_file',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'file_id',
-                    'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'body',
-                ],
-                'required': [
-                    'file_id',
-                    'id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'file_id',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('file_id',): {
-
-                        'regex': {
-                            'pattern': r'^\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b$',  # noqa: E501
-                        },
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'file_id':
-                        (str,),
-                    'id':
-                        (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'body':
-                        (file_type,),
-                },
-                'attribute_map': {
-                    'file_id': 'file_id',
-                    'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'file_id': 'path',
-                    'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
-                ]
-            },
-            api_client=api_client
-        )
-        self.partial_update_backup_file_endpoint = _Endpoint(
-            settings={
-                'response_schema': None,
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/tasks/backup/{file_id}',
-                'operation_id': 'partial_update_backup_file',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'file_id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'body',
-                ],
-                'required': [
-                    'file_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'file_id',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('file_id',): {
-
-                        'regex': {
-                            'pattern': r'^\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b$',  # noqa: E501
-                        },
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'file_id':
-                        (str,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'body':
-                        (file_type,),
-                },
-                'attribute_map': {
-                    'file_id': 'file_id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'file_id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
-                ]
-            },
-            api_client=api_client
-        )
-        self.partial_update_data_file_endpoint = _Endpoint(
-            settings={
-                'response_schema': None,
-                'auth': [
-                    'basicAuth',
-                    'csrfAuth',
-                    'sessionAuth',
-                    'signatureAuth',
-                    'tokenAuth'
-                ],
-                'endpoint_path': '/api/tasks/{id}/data/{file_id}',
-                'operation_id': 'partial_update_data_file',
-                'http_method': 'PATCH',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'file_id',
-                    'id',
-                    'x_organization',
-                    'org',
-                    'org_id',
-                    'body',
-                ],
-                'required': [
-                    'file_id',
-                    'id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                    'file_id',
-                ]
-            },
-            root_map={
-                'validations': {
-                    ('file_id',): {
-
-                        'regex': {
-                            'pattern': r'^\b[0-9a-f]{8}\b-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-\b[0-9a-f]{12}\b$',  # noqa: E501
-                        },
-                    },
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'file_id':
-                        (str,),
-                    'id':
-                        (int,),
-                    'x_organization':
-                        (str,),
-                    'org':
-                        (str,),
-                    'org_id':
-                        (int,),
-                    'body':
-                        (file_type,),
-                },
-                'attribute_map': {
-                    'file_id': 'file_id',
-                    'id': 'id',
-                    'x_organization': 'X-Organization',
-                    'org': 'org',
-                    'org_id': 'org_id',
-                },
-                'location_map': {
-                    'file_id': 'path',
-                    'id': 'path',
-                    'x_organization': 'header',
-                    'org': 'query',
-                    'org_id': 'query',
-                    'body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [],
-                'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
         self.partial_update_data_meta_endpoint = _Endpoint(
             settings={
                 'response_schema': (DataMetaRead,),
@@ -1295,18 +1014,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (TaskRead,),
@@ -2080,17 +1796,15 @@
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [],
                 'content_type': [
                     'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'multipart/form-data'
                 ]
             },
             api_client=api_client
         )
 
     def jobs_partial_update_data_meta(
         self,
@@ -2930,266 +2644,14 @@
         kwargs['_content_type'] = _content_type
         kwargs['_host_index'] = _host_index
         kwargs['_request_auths'] = _request_auths
         kwargs['action'] = action
         kwargs['id'] = id
         return self.partial_update_annotations_endpoint.call_with_http_info(**kwargs)
 
-    def partial_update_annotations_file(
-        self,
-        file_id: str,
-        id: int,
-        *,
-        _parse_response: bool = True,
-        _request_timeout: typing.Union[int, float, tuple] = None,
-        _validate_inputs: bool = True,
-        _validate_outputs: bool = True,
-        _check_status: bool = True,
-        _spec_property_naming: bool = False,
-        _content_type: typing.Optional[str] = None,
-        _host_index: typing.Optional[int] = None,
-        _request_auths: typing.Optional[typing.List] = None,
-        _async_call: bool = False,
-        **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Allows to upload an annotation file chunk. Implements TUS file uploading protocol.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass _async_call=True
-
-        >>> thread = api.partial_update_annotations_file(file_id, id, _async_call=True)
-        >>> result = thread.get()
-
-        Args:
-            file_id (str):
-            id (int): A unique integer value identifying this task.
-
-        Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            body (file_type): [optional]
-            _parse_response (bool): if False, the response data will not be parsed,
-                None is returned for data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _validate_inputs (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _validate_outputs (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _check_status (bool): whether to check response status
-                for being positive or not.
-                Default is True
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            _async_call (bool): execute request asynchronously
-
-        Returns:
-            (None, HTTPResponse)
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['_async_call'] = _async_call
-        kwargs['_parse_response'] = _parse_response
-        kwargs['_request_timeout'] = _request_timeout
-        kwargs['_validate_inputs'] = _validate_inputs
-        kwargs['_validate_outputs'] = _validate_outputs
-        kwargs['_check_status'] = _check_status
-        kwargs['_spec_property_naming'] = _spec_property_naming
-        kwargs['_content_type'] = _content_type
-        kwargs['_host_index'] = _host_index
-        kwargs['_request_auths'] = _request_auths
-        kwargs['file_id'] = file_id
-        kwargs['id'] = id
-        return self.partial_update_annotations_file_endpoint.call_with_http_info(**kwargs)
-
-    def partial_update_backup_file(
-        self,
-        file_id: str,
-        *,
-        _parse_response: bool = True,
-        _request_timeout: typing.Union[int, float, tuple] = None,
-        _validate_inputs: bool = True,
-        _validate_outputs: bool = True,
-        _check_status: bool = True,
-        _spec_property_naming: bool = False,
-        _content_type: typing.Optional[str] = None,
-        _host_index: typing.Optional[int] = None,
-        _request_auths: typing.Optional[typing.List] = None,
-        _async_call: bool = False,
-        **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Allows to upload a file chunk. Implements TUS file uploading protocol.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass _async_call=True
-
-        >>> thread = api.partial_update_backup_file(file_id, _async_call=True)
-        >>> result = thread.get()
-
-        Args:
-            file_id (str):
-
-        Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            body (file_type): [optional]
-            _parse_response (bool): if False, the response data will not be parsed,
-                None is returned for data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _validate_inputs (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _validate_outputs (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _check_status (bool): whether to check response status
-                for being positive or not.
-                Default is True
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            _async_call (bool): execute request asynchronously
-
-        Returns:
-            (None, HTTPResponse)
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['_async_call'] = _async_call
-        kwargs['_parse_response'] = _parse_response
-        kwargs['_request_timeout'] = _request_timeout
-        kwargs['_validate_inputs'] = _validate_inputs
-        kwargs['_validate_outputs'] = _validate_outputs
-        kwargs['_check_status'] = _check_status
-        kwargs['_spec_property_naming'] = _spec_property_naming
-        kwargs['_content_type'] = _content_type
-        kwargs['_host_index'] = _host_index
-        kwargs['_request_auths'] = _request_auths
-        kwargs['file_id'] = file_id
-        return self.partial_update_backup_file_endpoint.call_with_http_info(**kwargs)
-
-    def partial_update_data_file(
-        self,
-        file_id: str,
-        id: int,
-        *,
-        _parse_response: bool = True,
-        _request_timeout: typing.Union[int, float, tuple] = None,
-        _validate_inputs: bool = True,
-        _validate_outputs: bool = True,
-        _check_status: bool = True,
-        _spec_property_naming: bool = False,
-        _content_type: typing.Optional[str] = None,
-        _host_index: typing.Optional[int] = None,
-        _request_auths: typing.Optional[typing.List] = None,
-        _async_call: bool = False,
-        **kwargs,
-    ) -> typing.Tuple[typing.Optional[None], urllib3.HTTPResponse]:
-        """Allows to upload a file chunk. Implements TUS file uploading protocol.  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass _async_call=True
-
-        >>> thread = api.partial_update_data_file(file_id, id, _async_call=True)
-        >>> result = thread.get()
-
-        Args:
-            file_id (str):
-            id (int): A unique integer value identifying this task.
-
-        Keyword Args:
-            x_organization (str): [optional]
-            org (str): Organization unique slug. [optional]
-            org_id (int): Organization identifier. [optional]
-            body (file_type): [optional]
-            _parse_response (bool): if False, the response data will not be parsed,
-                None is returned for data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _validate_inputs (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _validate_outputs (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _check_status (bool): whether to check response status
-                for being positive or not.
-                Default is True
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            _request_auths (list): set to override the auth_settings for an a single
-                request; this effectively ignores the authentication
-                in the spec for a single request.
-                Default is None
-            _async_call (bool): execute request asynchronously
-
-        Returns:
-            (None, HTTPResponse)
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['_async_call'] = _async_call
-        kwargs['_parse_response'] = _parse_response
-        kwargs['_request_timeout'] = _request_timeout
-        kwargs['_validate_inputs'] = _validate_inputs
-        kwargs['_validate_outputs'] = _validate_outputs
-        kwargs['_check_status'] = _check_status
-        kwargs['_spec_property_naming'] = _spec_property_naming
-        kwargs['_content_type'] = _content_type
-        kwargs['_host_index'] = _host_index
-        kwargs['_request_auths'] = _request_auths
-        kwargs['file_id'] = file_id
-        kwargs['id'] = id
-        return self.partial_update_data_file_endpoint.call_with_http_info(**kwargs)
-
     def partial_update_data_meta(
         self,
         id: int,
         *,
         _parse_response: bool = True,
         _request_timeout: typing.Union[int, float, tuple] = None,
         _validate_inputs: bool = True,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/users_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/users_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -290,18 +290,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (MetaUser,),
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api/webhooks_api.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api/webhooks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -113,18 +113,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.create_deliveries_redelivery_endpoint = _Endpoint(
             settings={
                 'response_schema': None,
@@ -620,18 +617,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
         self.retrieve_endpoint = _Endpoint(
             settings={
                 'response_schema': (WebhookRead,),
@@ -921,18 +915,15 @@
                 }
             },
             headers_map={
                 'accept': [
                     'application/vnd.cvat+json'
                 ],
                 'content_type': [
-                    'application/json',
-                    'application/x-www-form-urlencoded',
-                    'multipart/form-data',
-                    'application/offset+octet-stream'
+                    'application/json'
                 ]
             },
             api_client=api_client
         )
 
     def create(
         self,
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/api_client.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import json
@@ -110,15 +110,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers: typing.Dict[str, str] = headers or {}
         self.cookies = SimpleCookie()
         if cookies:
             self.cookies.update(cookies)
         # Set default User-Agent.
-        self.user_agent = 'cvat_sdk/2.4.0'
+        self.user_agent = 'cvat_sdk/2.4.4'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
@@ -295,15 +295,15 @@
         headers = {}
         headers.update(self.default_headers)
         if self.cookies:
             headers['Cookie'] = self.cookies.output(attrs=[], header="", sep=";").strip()
         return headers
 
     def _update_cookies_from_response(self, response: HTTPResponse):
-        self.cookies.update(SimpleCookie(response.getheader("Set-Cookie")))
+        self.cookies.update(SimpleCookie(response.headers.get("Set-Cookie")))
 
     def parameters_to_multipart(self, params, collection_types):
         """Get parameters as list of tuples, formatting as json if value is collection_types
 
         :param params: Parameters as list of two-tuples
         :param dict collection_types: Parameter collection types
         :return: Parameters as list of tuple or urllib3.fields.RequestField
@@ -362,20 +362,20 @@
 
         if response_schema == (file_type,):
             # TODO: response schema can be "oneOf" with a file option,
             # this implementation does not cover this.
 
             # handle file downloading
             # save response body into a tmp file and return the instance
-            content_disposition = response.getheader("Content-Disposition")
+            content_disposition = response.headers.get("Content-Disposition")
             return deserialize_file(response.data, self.configuration,
                                     content_disposition=content_disposition)
 
         encoding = "utf-8"
-        content_type = response.getheader('content-type')
+        content_type = response.headers.get('content-type')
         if content_type is not None:
             match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
             if match:
                 encoding = match.group(1)
         response_data = response.data.decode(encoding)
 
         # fetch data from response object
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/apis/__init__.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/apis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # Import all APIs into this package.
 # If you have many APIs here with many many models used in each API this may
 # raise a `RecursionError`.
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/configuration.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import copy
 import logging
 import multiprocessing
@@ -484,16 +484,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.5\n"\
-               "SDK Package Version: 2.4.0".\
+               "Version of the API: 2.4.4\n"\
+               "SDK Package Version: 2.4.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/exceptions.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
@@ -101,15 +101,15 @@
 class ApiException(OpenApiException):
 
     def __init__(self, status=None, reason=None, http_resp=None):
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
             self.body = http_resp.data
-            self.headers = http_resp.getheaders()
+            self.headers = http_resp.headers
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/about.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/annotation_file_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotation_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/annotations_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/annotations_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute_val.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/attribute_val_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/attribute_val_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/backup_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/backup_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/basic_user.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/basic_user_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/basic_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/chunk_type.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/chunk_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/client_events.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/client_events_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/client_events_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/cloud_storage_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/cloud_storage_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/cloud_storage_write_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -99,14 +99,19 @@
     """
 
     secret_key: str # noqa: E501
     """
     [optional]
     """
 
+    connection_string: str # noqa: E501
+    """
+    [optional]
+    """
+
     key_file: file_type # noqa: E501
     """
     [optional]
     """
 
     specific_attributes: str # noqa: E501
     """
@@ -147,14 +152,16 @@
 
       account_name (str): [optional]  # noqa: E501
 
       key (str): [optional]  # noqa: E501
 
       secret_key (str): [optional]  # noqa: E501
 
+      connection_string (str): [optional]  # noqa: E501
+
       key_file (file_type): [optional]  # noqa: E501
 
       specific_attributes (str): [optional]  # noqa: E501
 
       description (str): [optional]  # noqa: E501
 
       manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
@@ -198,14 +205,17 @@
         },
         ('key',): {
             'max_length': 40,
         },
         ('secret_key',): {
             'max_length': 44,
         },
+        ('connection_string',): {
+            'max_length': 440,
+        },
         ('specific_attributes',): {
             'max_length': 1024,
         },
     }
 
     @cached_property
     def additional_properties_type():
@@ -235,14 +245,15 @@
             'display_name': (str,),  # noqa: E501
             'credentials_type': (CredentialsTypeEnum,),  # noqa: E501
             'owner': (BasicUserRequest,),  # noqa: E501
             'session_token': (str,),  # noqa: E501
             'account_name': (str,),  # noqa: E501
             'key': (str,),  # noqa: E501
             'secret_key': (str,),  # noqa: E501
+            'connection_string': (str,),  # noqa: E501
             'key_file': (file_type,),  # noqa: E501
             'specific_attributes': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'manifests': ([str],),  # noqa: E501
         }
 
     @cached_property
@@ -257,14 +268,15 @@
         'display_name': 'display_name',  # noqa: E501
         'credentials_type': 'credentials_type',  # noqa: E501
         'owner': 'owner',  # noqa: E501
         'session_token': 'session_token',  # noqa: E501
         'account_name': 'account_name',  # noqa: E501
         'key': 'key',  # noqa: E501
         'secret_key': 'secret_key',  # noqa: E501
+        'connection_string': 'connection_string',  # noqa: E501
         'key_file': 'key_file',  # noqa: E501
         'specific_attributes': 'specific_attributes',  # noqa: E501
         'description': 'description',  # noqa: E501
         'manifests': 'manifests',  # noqa: E501
     }
 
     read_only_vars = {
@@ -290,14 +302,16 @@
 
             account_name (str): [optional]  # noqa: E501
 
             key (str): [optional]  # noqa: E501
 
             secret_key (str): [optional]  # noqa: E501
 
+            connection_string (str): [optional]  # noqa: E501
+
             key_file (file_type): [optional]  # noqa: E501
 
             specific_attributes (str): [optional]  # noqa: E501
 
             description (str): [optional]  # noqa: E501
 
             manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
@@ -404,14 +418,16 @@
 
             account_name (str): [optional]  # noqa: E501
 
             key (str): [optional]  # noqa: E501
 
             secret_key (str): [optional]  # noqa: E501
 
+            connection_string (str): [optional]  # noqa: E501
+
             key_file (file_type): [optional]  # noqa: E501
 
             specific_attributes (str): [optional]  # noqa: E501
 
             description (str): [optional]  # noqa: E501
 
             manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/comment_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/comment_read_owner.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/comment_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/comments_summary.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/comments_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/credentials_type_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/credentials_type_enum.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -53,15 +53,15 @@
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS"  # noqa: E501
+    One of: "KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING"  # noqa: E501
     """
 
 class CredentialsTypeEnum(ModelSimple, ICredentialsTypeEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -82,14 +82,15 @@
 
     allowed_values = {
         ('value',): {
             'KEY_SECRET_KEY_PAIR': "KEY_SECRET_KEY_PAIR",
             'ACCOUNT_NAME_TOKEN_PAIR': "ACCOUNT_NAME_TOKEN_PAIR",
             'KEY_FILE_PATH': "KEY_FILE_PATH",
             'ANONYMOUS_ACCESS': "ANONYMOUS_ACCESS",
+            'CONNECTION_STRING': "CONNECTION_STRING",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -134,18 +135,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """CredentialsTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", ]  # noqa: E501
+            args[0] (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", ]  # noqa: E501
+            value (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -230,18 +231,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """CredentialsTypeEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", ]  # noqa: E501
+            args[0] (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", ]  # noqa: E501
+            value (str):, must be one of ["KEY_SECRET_KEY_PAIR", "ACCOUNT_NAME_TOKEN_PAIR", "KEY_FILE_PATH", "ANONYMOUS_ACCESS", "CONNECTION_STRING", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/data_meta_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/data_meta_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/data_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,185 +41,171 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
     from cvat_sdk.api_client.model.chunk_type import ChunkType
-    from cvat_sdk.api_client.model.sorting_method import SortingMethod
-    from cvat_sdk.api_client.model.storage_method import StorageMethod
-    from cvat_sdk.api_client.model.storage_type import StorageType
+    from cvat_sdk.api_client.model.issues_summary import IssuesSummary
+    from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
+    from cvat_sdk.api_client.model.job_stage import JobStage
+    from cvat_sdk.api_client.model.job_status import JobStatus
+    from cvat_sdk.api_client.model.labels_summary import LabelsSummary
+    from cvat_sdk.api_client.model.operation_status import OperationStatus
     globals()['ChunkType'] = ChunkType
-    globals()['SortingMethod'] = SortingMethod
-    globals()['StorageMethod'] = StorageMethod
-    globals()['StorageType'] = StorageType
+    globals()['IssuesSummary'] = IssuesSummary
+    globals()['JobReadAssignee'] = JobReadAssignee
+    globals()['JobStage'] = JobStage
+    globals()['JobStatus'] = JobStatus
+    globals()['LabelsSummary'] = LabelsSummary
+    globals()['OperationStatus'] = OperationStatus
 
 
 
-class IDataRequest(IModelData):
+class IJobRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    chunk_size: typing.Union[int, none_type] # noqa: E501
+    url: str # noqa: E501
     """
     [optional]
     """
 
-    size: int # noqa: E501
+    id: int # noqa: E501
     """
     [optional]
     """
 
-    image_quality: int # noqa: E501
-    """
-    """
-
-    start_frame: int # noqa: E501
+    task_id: int # noqa: E501
     """
     [optional]
     """
 
-    stop_frame: int # noqa: E501
+    project_id: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
-    frame_filter: str # noqa: E501
+    assignee: JobReadAssignee # noqa: E501
     """
     [optional]
     """
 
-    compressed_chunk_type: ChunkType # noqa: E501
+    dimension: str # noqa: E501
     """
     [optional]
     """
 
-    original_chunk_type: ChunkType # noqa: E501
+    bug_tracker: typing.Union[str, none_type] # noqa: E501
     """
     [optional]
     """
 
-    client_files: typing.List[file_type] # noqa: E501
-    """
-    [optional, default: []]
-    [file_type]
-    """
-
-    server_files: typing.List[str] # noqa: E501
+    status: typing.Union[typing.Any, none_type] # noqa: E501
     """
-    [optional, default: []]
-    [str]
+    [optional]
     """
 
-    remote_files: typing.List[str] # noqa: E501
+    stage: typing.Union[typing.Any, none_type] # noqa: E501
     """
-    [optional, default: []]
-    [str]
+    [optional]
     """
 
-    use_zip_chunks: bool # noqa: E501
+    state: typing.Union[typing.Any, none_type] # noqa: E501
     """
-    [optional, default: False]
+    [optional]
     """
 
-    cloud_storage_id: typing.Union[int, none_type] # noqa: E501
+    mode: str # noqa: E501
     """
     [optional]
     """
 
-    use_cache: bool # noqa: E501
+    start_frame: int # noqa: E501
     """
-    [optional, default: False]
+    [optional]
     """
 
-    copy_data: bool # noqa: E501
+    stop_frame: int # noqa: E501
     """
-    [optional, default: False]
+    [optional]
     """
 
-    storage_method: StorageMethod # noqa: E501
+    data_chunk_size: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
-    storage: StorageType # noqa: E501
+    data_compressed_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
     """
 
-    sorting_method: SortingMethod # noqa: E501
+    updated_date: datetime # noqa: E501
     """
     [optional]
     """
 
-    filename_pattern: typing.Union[str, none_type] # noqa: E501
+    issues: IssuesSummary # noqa: E501
     """
-    [optional]
     """
 
-    job_file_mapping: typing.List[typing.List[str]] # noqa: E501
+    labels: LabelsSummary # noqa: E501
     """
-    [optional]
-    [[str]]
-     Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ]  Files in the jobs must not overlap and repeat. .
     """
 
 
-class DataRequest(ModelNormal, IDataRequest):
+class JobRead(ModelNormal, IJobRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      image_quality (int):
-
-      chunk_size (int, none_type): [optional]  # noqa: E501
+      issues (IssuesSummary):
 
-      size (int): [optional]  # noqa: E501
+      labels (LabelsSummary):
 
-      start_frame (int): [optional]  # noqa: E501
-
-      stop_frame (int): [optional]  # noqa: E501
+      url (str): [optional]  # noqa: E501
 
-      frame_filter (str): [optional]  # noqa: E501
+      id (int): [optional]  # noqa: E501
 
-      compressed_chunk_type (ChunkType): [optional]  # noqa: E501
+      task_id (int): [optional]  # noqa: E501
 
-      original_chunk_type (ChunkType): [optional]  # noqa: E501
+      project_id (int, none_type): [optional]  # noqa: E501
 
-      client_files ([file_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+      assignee (JobReadAssignee): [optional]  # noqa: E501
 
-      server_files ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+      dimension (str): [optional]  # noqa: E501
 
-      remote_files ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+      bug_tracker (str, none_type): [optional]  # noqa: E501
 
-      use_zip_chunks (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+      status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-      cloud_storage_id (int, none_type): [optional]  # noqa: E501
+      stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-      use_cache (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+      state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-      copy_data (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+      mode (str): [optional]  # noqa: E501
 
-      storage_method (StorageMethod): [optional]  # noqa: E501
+      start_frame (int): [optional]  # noqa: E501
 
-      storage (StorageType): [optional]  # noqa: E501
+      stop_frame (int): [optional]  # noqa: E501
 
-      sorting_method (SortingMethod): [optional]  # noqa: E501
+      data_chunk_size (int, none_type): [optional]  # noqa: E501
 
-      filename_pattern (str, none_type): [optional]  # noqa: E501
+      data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-      job_file_mapping ([[str]]):  Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ]  Files in the jobs must not overlap and repeat. . [optional]  # noqa: E501
+      updated_date (datetime): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -236,39 +222,31 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('image_quality',): {
-            'inclusive_maximum': 100,
-            'inclusive_minimum': 0,
+        ('dimension',): {
+            'max_length': 2,
         },
-        ('chunk_size',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': 0,
-        },
-        ('size',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': 0,
+        ('bug_tracker',): {
+            'max_length': 2000,
         },
         ('start_frame',): {
             'inclusive_maximum': 2147483647,
-            'inclusive_minimum': 0,
+            'inclusive_minimum': -2147483648,
         },
         ('stop_frame',): {
             'inclusive_maximum': 2147483647,
-            'inclusive_minimum': 0,
-        },
-        ('frame_filter',): {
-            'max_length': 256,
+            'inclusive_minimum': -2147483648,
         },
-        ('filename_pattern',): {
-            'min_length': 1,
+        ('data_chunk_size',): {
+            'inclusive_maximum': 2147483647,
+            'inclusive_minimum': 0,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -287,116 +265,122 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'image_quality': (int,),  # noqa: E501
-            'chunk_size': (int, none_type,),  # noqa: E501
-            'size': (int,),  # noqa: E501
+            'issues': (IssuesSummary,),  # noqa: E501
+            'labels': (LabelsSummary,),  # noqa: E501
+            'url': (str,),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'task_id': (int,),  # noqa: E501
+            'project_id': (int, none_type,),  # noqa: E501
+            'assignee': (JobReadAssignee,),  # noqa: E501
+            'dimension': (str,),  # noqa: E501
+            'bug_tracker': (str, none_type,),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'stage': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'state': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'mode': (str,),  # noqa: E501
             'start_frame': (int,),  # noqa: E501
             'stop_frame': (int,),  # noqa: E501
-            'frame_filter': (str,),  # noqa: E501
-            'compressed_chunk_type': (ChunkType,),  # noqa: E501
-            'original_chunk_type': (ChunkType,),  # noqa: E501
-            'client_files': ([file_type],),  # noqa: E501
-            'server_files': ([str],),  # noqa: E501
-            'remote_files': ([str],),  # noqa: E501
-            'use_zip_chunks': (bool,),  # noqa: E501
-            'cloud_storage_id': (int, none_type,),  # noqa: E501
-            'use_cache': (bool,),  # noqa: E501
-            'copy_data': (bool,),  # noqa: E501
-            'storage_method': (StorageMethod,),  # noqa: E501
-            'storage': (StorageType,),  # noqa: E501
-            'sorting_method': (SortingMethod,),  # noqa: E501
-            'filename_pattern': (str, none_type,),  # noqa: E501
-            'job_file_mapping': ([[str]],),  # noqa: E501
+            'data_chunk_size': (int, none_type,),  # noqa: E501
+            'data_compressed_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'updated_date': (datetime,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'image_quality': 'image_quality',  # noqa: E501
-        'chunk_size': 'chunk_size',  # noqa: E501
-        'size': 'size',  # noqa: E501
+        'issues': 'issues',  # noqa: E501
+        'labels': 'labels',  # noqa: E501
+        'url': 'url',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'task_id': 'task_id',  # noqa: E501
+        'project_id': 'project_id',  # noqa: E501
+        'assignee': 'assignee',  # noqa: E501
+        'dimension': 'dimension',  # noqa: E501
+        'bug_tracker': 'bug_tracker',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'stage': 'stage',  # noqa: E501
+        'state': 'state',  # noqa: E501
+        'mode': 'mode',  # noqa: E501
         'start_frame': 'start_frame',  # noqa: E501
         'stop_frame': 'stop_frame',  # noqa: E501
-        'frame_filter': 'frame_filter',  # noqa: E501
-        'compressed_chunk_type': 'compressed_chunk_type',  # noqa: E501
-        'original_chunk_type': 'original_chunk_type',  # noqa: E501
-        'client_files': 'client_files',  # noqa: E501
-        'server_files': 'server_files',  # noqa: E501
-        'remote_files': 'remote_files',  # noqa: E501
-        'use_zip_chunks': 'use_zip_chunks',  # noqa: E501
-        'cloud_storage_id': 'cloud_storage_id',  # noqa: E501
-        'use_cache': 'use_cache',  # noqa: E501
-        'copy_data': 'copy_data',  # noqa: E501
-        'storage_method': 'storage_method',  # noqa: E501
-        'storage': 'storage',  # noqa: E501
-        'sorting_method': 'sorting_method',  # noqa: E501
-        'filename_pattern': 'filename_pattern',  # noqa: E501
-        'job_file_mapping': 'job_file_mapping',  # noqa: E501
+        'data_chunk_size': 'data_chunk_size',  # noqa: E501
+        'data_compressed_chunk_type': 'data_compressed_chunk_type',  # noqa: E501
+        'updated_date': 'updated_date',  # noqa: E501
     }
 
     read_only_vars = {
+        'url',  # noqa: E501
+        'id',  # noqa: E501
+        'task_id',  # noqa: E501
+        'project_id',  # noqa: E501
+        'dimension',  # noqa: E501
+        'bug_tracker',  # noqa: E501
+        'status',  # noqa: E501
+        'stage',  # noqa: E501
+        'state',  # noqa: E501
+        'mode',  # noqa: E501
+        'start_frame',  # noqa: E501
+        'stop_frame',  # noqa: E501
+        'data_chunk_size',  # noqa: E501
+        'data_compressed_chunk_type',  # noqa: E501
+        'updated_date',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, image_quality, *args, **kwargs):  # noqa: E501
-        """DataRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, issues, labels, *args, **kwargs):  # noqa: E501
+        """JobRead - a model defined in OpenAPI
 
         Args:
-            image_quality (int):
+            issues (IssuesSummary):
+            labels (LabelsSummary):
 
         Keyword Args:
-            chunk_size (int, none_type): [optional]  # noqa: E501
-
-            size (int): [optional]  # noqa: E501
-
-            start_frame (int): [optional]  # noqa: E501
-
-            stop_frame (int): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
 
-            frame_filter (str): [optional]  # noqa: E501
+            id (int): [optional]  # noqa: E501
 
-            compressed_chunk_type (ChunkType): [optional]  # noqa: E501
+            task_id (int): [optional]  # noqa: E501
 
-            original_chunk_type (ChunkType): [optional]  # noqa: E501
+            project_id (int, none_type): [optional]  # noqa: E501
 
-            client_files ([file_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            assignee (JobReadAssignee): [optional]  # noqa: E501
 
-            server_files ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            dimension (str): [optional]  # noqa: E501
 
-            remote_files ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            bug_tracker (str, none_type): [optional]  # noqa: E501
 
-            use_zip_chunks (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            cloud_storage_id (int, none_type): [optional]  # noqa: E501
+            stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            use_cache (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+            state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            copy_data (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+            mode (str): [optional]  # noqa: E501
 
-            storage_method (StorageMethod): [optional]  # noqa: E501
+            start_frame (int): [optional]  # noqa: E501
 
-            storage (StorageType): [optional]  # noqa: E501
+            stop_frame (int): [optional]  # noqa: E501
 
-            sorting_method (SortingMethod): [optional]  # noqa: E501
+            data_chunk_size (int, none_type): [optional]  # noqa: E501
 
-            filename_pattern (str, none_type): [optional]  # noqa: E501
+            data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            job_file_mapping ([[str]]):  Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ]  Files in the jobs must not overlap and repeat. . [optional]  # noqa: E501
+            updated_date (datetime): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -452,15 +436,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.image_quality = image_quality
+        self.issues = issues
+        self.labels = labels
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -473,58 +458,53 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, image_quality, *args, **kwargs):  # noqa: E501
-        """DataRequest - a model defined in OpenAPI
+    def __init__(self, issues, labels, *args, **kwargs):  # noqa: E501
+        """JobRead - a model defined in OpenAPI
 
         Args:
-            image_quality (int):
+            issues (IssuesSummary):
+            labels (LabelsSummary):
 
         Keyword Args:
-            chunk_size (int, none_type): [optional]  # noqa: E501
-
-            size (int): [optional]  # noqa: E501
+            url (str): [optional]  # noqa: E501
 
-            start_frame (int): [optional]  # noqa: E501
-
-            stop_frame (int): [optional]  # noqa: E501
+            id (int): [optional]  # noqa: E501
 
-            frame_filter (str): [optional]  # noqa: E501
+            task_id (int): [optional]  # noqa: E501
 
-            compressed_chunk_type (ChunkType): [optional]  # noqa: E501
+            project_id (int, none_type): [optional]  # noqa: E501
 
-            original_chunk_type (ChunkType): [optional]  # noqa: E501
+            assignee (JobReadAssignee): [optional]  # noqa: E501
 
-            client_files ([file_type]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            dimension (str): [optional]  # noqa: E501
 
-            server_files ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            bug_tracker (str, none_type): [optional]  # noqa: E501
 
-            remote_files ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            use_zip_chunks (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+            stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            cloud_storage_id (int, none_type): [optional]  # noqa: E501
+            state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            use_cache (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
+            mode (str): [optional]  # noqa: E501
 
-            copy_data (bool): [optional] if omitted the server will use the default value of False  # noqa: E501
-
-            storage_method (StorageMethod): [optional]  # noqa: E501
+            start_frame (int): [optional]  # noqa: E501
 
-            storage (StorageType): [optional]  # noqa: E501
+            stop_frame (int): [optional]  # noqa: E501
 
-            sorting_method (SortingMethod): [optional]  # noqa: E501
+            data_chunk_size (int, none_type): [optional]  # noqa: E501
 
-            filename_pattern (str, none_type): [optional]  # noqa: E501
+            data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            job_file_mapping ([[str]]):  Represents a file-to-job mapping. Useful to specify a custom job configuration during task creation. This option is not compatible with most other job split-related options.  Example: [     [\"file1.jpg\", \"file2.jpg\"], # job #1 files     [\"file3.png\"], # job #2 files     [\"file4.jpg\", \"file5.png\", \"file6.bmp\"], # job #3 files ]  Files in the jobs must not overlap and repeat. . [optional]  # noqa: E501
+            updated_date (datetime): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -578,15 +558,16 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.image_quality = image_quality
+        self.issues = issues
+        self.labels = labels
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_file_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_format.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_formats.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/dataset_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/dataset_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/event.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/event_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/events.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/events_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/events_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -53,15 +53,15 @@
     Do not edit the class manually.
     """
 
     value: str
     """
     [optional]
 
-    One of: "create:comment", "create:invitation", "create:issue", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:membership", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task"  # noqa: E501
+    One of: "create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task"  # noqa: E501
     """
 
 class EventsEnum(ModelSimple, IEventsEnum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -81,20 +81,24 @@
     """
 
     allowed_values = {
         ('value',): {
             'CREATE:COMMENT': "create:comment",
             'CREATE:INVITATION': "create:invitation",
             'CREATE:ISSUE': "create:issue",
+            'CREATE:JOB': "create:job",
+            'CREATE:MEMBERSHIP': "create:membership",
             'CREATE:PROJECT': "create:project",
             'CREATE:TASK': "create:task",
             'DELETE:COMMENT': "delete:comment",
             'DELETE:INVITATION': "delete:invitation",
             'DELETE:ISSUE': "delete:issue",
+            'DELETE:JOB': "delete:job",
             'DELETE:MEMBERSHIP': "delete:membership",
+            'DELETE:ORGANIZATION': "delete:organization",
             'DELETE:PROJECT': "delete:project",
             'DELETE:TASK': "delete:task",
             'UPDATE:COMMENT': "update:comment",
             'UPDATE:ISSUE': "update:issue",
             'UPDATE:JOB': "update:job",
             'UPDATE:MEMBERSHIP': "update:membership",
             'UPDATE:ORGANIZATION': "update:organization",
@@ -148,18 +152,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """EventsEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:membership", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            args[0] (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:membership", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            value (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -244,18 +248,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """EventsEnum - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:membership", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            args[0] (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:membership", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
+            value (str):, must be one of ["create:comment", "create:invitation", "create:issue", "create:job", "create:membership", "create:project", "create:task", "delete:comment", "delete:invitation", "delete:issue", "delete:job", "delete:membership", "delete:organization", "delete:project", "delete:task", "update:comment", "update:issue", "update:job", "update:membership", "update:organization", "update:project", "update:task", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/file_info.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/file_info_type_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/file_info_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/frame_meta.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/frame_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/input_type_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/input_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/invitation_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/invitation_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/invitation_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/issue_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/issue_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/issue_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/issues_summary.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/tasks_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,15 +41,15 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class IIssuesSummary(IModelData):
+class ITasksSummary(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -61,15 +61,15 @@
 
     url: str # noqa: E501
     """
     [optional]
     """
 
 
-class IssuesSummary(ModelNormal, IIssuesSummary):
+class TasksSummary(ModelNormal, ITasksSummary):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
@@ -143,15 +143,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """IssuesSummary - a model defined in OpenAPI
+        """TasksSummary - a model defined in OpenAPI
 
         Keyword Args:
             count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
             url (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
@@ -233,15 +233,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """IssuesSummary - a model defined in OpenAPI
+        """TasksSummary - a model defined in OpenAPI
 
         Keyword Args:
             count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
 
             url (str): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_annotations_update_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,32 +40,30 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.chunk_type import ChunkType
-    from cvat_sdk.api_client.model.issues_summary import IssuesSummary
     from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
-    from cvat_sdk.api_client.model.job_stage import JobStage
     from cvat_sdk.api_client.model.job_status import JobStatus
     from cvat_sdk.api_client.model.labels_summary import LabelsSummary
-    from cvat_sdk.api_client.model.operation_status import OperationStatus
-    globals()['ChunkType'] = ChunkType
-    globals()['IssuesSummary'] = IssuesSummary
+    from cvat_sdk.api_client.model.project_read_owner import ProjectReadOwner
+    from cvat_sdk.api_client.model.project_read_target_storage import ProjectReadTargetStorage
+    from cvat_sdk.api_client.model.tasks_summary import TasksSummary
     globals()['JobReadAssignee'] = JobReadAssignee
-    globals()['JobStage'] = JobStage
     globals()['JobStatus'] = JobStatus
     globals()['LabelsSummary'] = LabelsSummary
-    globals()['OperationStatus'] = OperationStatus
+    globals()['ProjectReadOwner'] = ProjectReadOwner
+    globals()['ProjectReadTargetStorage'] = ProjectReadTargetStorage
+    globals()['TasksSummary'] = TasksSummary
 
 
 
-class IJobRead(IModelData):
+class IProjectRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -76,136 +74,123 @@
     """
 
     id: int # noqa: E501
     """
     [optional]
     """
 
-    task_id: int # noqa: E501
+    name: str # noqa: E501
     """
     [optional]
     """
 
-    project_id: typing.Union[int, none_type] # noqa: E501
+    owner: ProjectReadOwner # noqa: E501
     """
     [optional]
     """
 
     assignee: JobReadAssignee # noqa: E501
     """
     [optional]
     """
 
-    dimension: str # noqa: E501
+    bug_tracker: str # noqa: E501
     """
     [optional]
     """
 
-    bug_tracker: typing.Union[str, none_type] # noqa: E501
+    task_subsets: typing.List[str] # noqa: E501
     """
     [optional]
+    [str]
     """
 
-    status: typing.Union[typing.Any, none_type] # noqa: E501
-    """
-    [optional]
-    """
-
-    stage: typing.Union[typing.Any, none_type] # noqa: E501
+    created_date: datetime # noqa: E501
     """
     [optional]
     """
 
-    state: typing.Union[typing.Any, none_type] # noqa: E501
-    """
-    [optional]
-    """
-
-    mode: str # noqa: E501
+    updated_date: datetime # noqa: E501
     """
     [optional]
     """
 
-    start_frame: int # noqa: E501
+    status: typing.Union[typing.Any, none_type] # noqa: E501
     """
     [optional]
     """
 
-    stop_frame: int # noqa: E501
+    dimension: typing.Union[str, none_type] # noqa: E501
     """
     [optional]
     """
 
-    data_chunk_size: typing.Union[int, none_type] # noqa: E501
+    organization: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
-    data_compressed_chunk_type: typing.Union[typing.Any, none_type] # noqa: E501
+    target_storage: ProjectReadTargetStorage # noqa: E501
     """
     [optional]
     """
 
-    updated_date: datetime # noqa: E501
+    source_storage: ProjectReadTargetStorage # noqa: E501
     """
     [optional]
     """
 
-    issues: IssuesSummary # noqa: E501
+    tasks: TasksSummary # noqa: E501
     """
     """
 
     labels: LabelsSummary # noqa: E501
     """
     """
 
 
-class JobRead(ModelNormal, IJobRead):
+class ProjectRead(ModelNormal, IProjectRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      issues (IssuesSummary):
+      tasks (TasksSummary):
 
       labels (LabelsSummary):
 
       url (str): [optional]  # noqa: E501
 
       id (int): [optional]  # noqa: E501
 
-      task_id (int): [optional]  # noqa: E501
+      name (str): [optional]  # noqa: E501
 
-      project_id (int, none_type): [optional]  # noqa: E501
+      owner (ProjectReadOwner): [optional]  # noqa: E501
 
       assignee (JobReadAssignee): [optional]  # noqa: E501
 
-      dimension (str): [optional]  # noqa: E501
-
-      bug_tracker (str, none_type): [optional]  # noqa: E501
+      bug_tracker (str): [optional]  # noqa: E501
 
-      status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+      task_subsets ([str]): [optional]  # noqa: E501
 
-      stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+      created_date (datetime): [optional]  # noqa: E501
 
-      state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+      updated_date (datetime): [optional]  # noqa: E501
 
-      mode (str): [optional]  # noqa: E501
+      status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-      start_frame (int): [optional]  # noqa: E501
+      dimension (str, none_type): [optional]  # noqa: E501
 
-      stop_frame (int): [optional]  # noqa: E501
+      organization (int, none_type): [optional]  # noqa: E501
 
-      data_chunk_size (int, none_type): [optional]  # noqa: E501
+      target_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
 
-      data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-
-      updated_date (datetime): [optional]  # noqa: E501
+      source_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -223,30 +208,15 @@
     """
 
     allowed_values = {
     }
 
     validations = {
         ('dimension',): {
-            'max_length': 2,
-        },
-        ('bug_tracker',): {
-            'max_length': 2000,
-        },
-        ('start_frame',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
-        ('stop_frame',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': -2147483648,
-        },
-        ('data_chunk_size',): {
-            'inclusive_maximum': 2147483647,
-            'inclusive_minimum': 0,
+            'max_length': 16,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -265,122 +235,109 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'issues': (IssuesSummary,),  # noqa: E501
+            'tasks': (TasksSummary,),  # noqa: E501
             'labels': (LabelsSummary,),  # noqa: E501
             'url': (str,),  # noqa: E501
             'id': (int,),  # noqa: E501
-            'task_id': (int,),  # noqa: E501
-            'project_id': (int, none_type,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'owner': (ProjectReadOwner,),  # noqa: E501
             'assignee': (JobReadAssignee,),  # noqa: E501
-            'dimension': (str,),  # noqa: E501
-            'bug_tracker': (str, none_type,),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'stage': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'state': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'mode': (str,),  # noqa: E501
-            'start_frame': (int,),  # noqa: E501
-            'stop_frame': (int,),  # noqa: E501
-            'data_chunk_size': (int, none_type,),  # noqa: E501
-            'data_compressed_chunk_type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'bug_tracker': (str,),  # noqa: E501
+            'task_subsets': ([str],),  # noqa: E501
+            'created_date': (datetime,),  # noqa: E501
             'updated_date': (datetime,),  # noqa: E501
+            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'dimension': (str, none_type,),  # noqa: E501
+            'organization': (int, none_type,),  # noqa: E501
+            'target_storage': (ProjectReadTargetStorage,),  # noqa: E501
+            'source_storage': (ProjectReadTargetStorage,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'issues': 'issues',  # noqa: E501
+        'tasks': 'tasks',  # noqa: E501
         'labels': 'labels',  # noqa: E501
         'url': 'url',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'task_id': 'task_id',  # noqa: E501
-        'project_id': 'project_id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'owner': 'owner',  # noqa: E501
         'assignee': 'assignee',  # noqa: E501
-        'dimension': 'dimension',  # noqa: E501
         'bug_tracker': 'bug_tracker',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'stage': 'stage',  # noqa: E501
-        'state': 'state',  # noqa: E501
-        'mode': 'mode',  # noqa: E501
-        'start_frame': 'start_frame',  # noqa: E501
-        'stop_frame': 'stop_frame',  # noqa: E501
-        'data_chunk_size': 'data_chunk_size',  # noqa: E501
-        'data_compressed_chunk_type': 'data_compressed_chunk_type',  # noqa: E501
+        'task_subsets': 'task_subsets',  # noqa: E501
+        'created_date': 'created_date',  # noqa: E501
         'updated_date': 'updated_date',  # noqa: E501
+        'status': 'status',  # noqa: E501
+        'dimension': 'dimension',  # noqa: E501
+        'organization': 'organization',  # noqa: E501
+        'target_storage': 'target_storage',  # noqa: E501
+        'source_storage': 'source_storage',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
         'id',  # noqa: E501
-        'task_id',  # noqa: E501
-        'project_id',  # noqa: E501
-        'dimension',  # noqa: E501
+        'name',  # noqa: E501
         'bug_tracker',  # noqa: E501
-        'status',  # noqa: E501
-        'stage',  # noqa: E501
-        'state',  # noqa: E501
-        'mode',  # noqa: E501
-        'start_frame',  # noqa: E501
-        'stop_frame',  # noqa: E501
-        'data_chunk_size',  # noqa: E501
-        'data_compressed_chunk_type',  # noqa: E501
+        'task_subsets',  # noqa: E501
+        'created_date',  # noqa: E501
         'updated_date',  # noqa: E501
+        'status',  # noqa: E501
+        'dimension',  # noqa: E501
+        'organization',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, issues, labels, *args, **kwargs):  # noqa: E501
-        """JobRead - a model defined in OpenAPI
+    def _from_openapi_data(cls, tasks, labels, *args, **kwargs):  # noqa: E501
+        """ProjectRead - a model defined in OpenAPI
 
         Args:
-            issues (IssuesSummary):
+            tasks (TasksSummary):
             labels (LabelsSummary):
 
         Keyword Args:
             url (str): [optional]  # noqa: E501
 
             id (int): [optional]  # noqa: E501
 
-            task_id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
 
-            project_id (int, none_type): [optional]  # noqa: E501
+            owner (ProjectReadOwner): [optional]  # noqa: E501
 
             assignee (JobReadAssignee): [optional]  # noqa: E501
 
-            dimension (str): [optional]  # noqa: E501
-
-            bug_tracker (str, none_type): [optional]  # noqa: E501
+            bug_tracker (str): [optional]  # noqa: E501
 
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-
-            stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            task_subsets ([str]): [optional]  # noqa: E501
 
-            state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            created_date (datetime): [optional]  # noqa: E501
 
-            mode (str): [optional]  # noqa: E501
+            updated_date (datetime): [optional]  # noqa: E501
 
-            start_frame (int): [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            stop_frame (int): [optional]  # noqa: E501
+            dimension (str, none_type): [optional]  # noqa: E501
 
-            data_chunk_size (int, none_type): [optional]  # noqa: E501
+            organization (int, none_type): [optional]  # noqa: E501
 
-            data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            target_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
 
-            updated_date (datetime): [optional]  # noqa: E501
+            source_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -436,15 +393,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.issues = issues
+        self.tasks = tasks
         self.labels = labels
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -458,53 +415,49 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, issues, labels, *args, **kwargs):  # noqa: E501
-        """JobRead - a model defined in OpenAPI
+    def __init__(self, tasks, labels, *args, **kwargs):  # noqa: E501
+        """ProjectRead - a model defined in OpenAPI
 
         Args:
-            issues (IssuesSummary):
+            tasks (TasksSummary):
             labels (LabelsSummary):
 
         Keyword Args:
             url (str): [optional]  # noqa: E501
 
             id (int): [optional]  # noqa: E501
 
-            task_id (int): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
 
-            project_id (int, none_type): [optional]  # noqa: E501
+            owner (ProjectReadOwner): [optional]  # noqa: E501
 
             assignee (JobReadAssignee): [optional]  # noqa: E501
 
-            dimension (str): [optional]  # noqa: E501
+            bug_tracker (str): [optional]  # noqa: E501
 
-            bug_tracker (str, none_type): [optional]  # noqa: E501
+            task_subsets ([str]): [optional]  # noqa: E501
 
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            created_date (datetime): [optional]  # noqa: E501
 
-            stage (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-
-            state (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-
-            mode (str): [optional]  # noqa: E501
+            updated_date (datetime): [optional]  # noqa: E501
 
-            start_frame (int): [optional]  # noqa: E501
+            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
 
-            stop_frame (int): [optional]  # noqa: E501
+            dimension (str, none_type): [optional]  # noqa: E501
 
-            data_chunk_size (int, none_type): [optional]  # noqa: E501
+            organization (int, none_type): [optional]  # noqa: E501
 
-            data_compressed_chunk_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            target_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
 
-            updated_date (datetime): [optional]  # noqa: E501
+            source_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -558,15 +511,15 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.issues = issues
+        self.tasks = tasks
         self.labels = labels
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_read_assignee.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_read_assignee.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_stage.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/job_status.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/jobs_summary.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/jobs_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/label.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/label.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_data.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_data_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_data_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_image.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_image_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_shape.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_shape_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_track.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labeled_track_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/labels_summary.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/labels_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -50,37 +50,37 @@
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    count: int # noqa: E501
+    url: str # noqa: E501
     """
-    [optional, default: 0]
+    [optional]
     """
 
-    url: str # noqa: E501
+    count: int # noqa: E501
     """
     [optional]
     """
 
 
 class LabelsSummary(ModelNormal, ILabelsSummary):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
       url (str): [optional]  # noqa: E501
 
+      count (int): [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -119,45 +119,46 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'count': (int,),  # noqa: E501
             'url': (str,),  # noqa: E501
+            'count': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'count': 'count',  # noqa: E501
         'url': 'url',  # noqa: E501
+        'count': 'count',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
+        'count',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """LabelsSummary - a model defined in OpenAPI
 
         Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
             url (str): [optional]  # noqa: E501
 
+            count (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -236,18 +237,18 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """LabelsSummary - a model defined in OpenAPI
 
         Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
             url (str): [optional]  # noqa: E501
 
+            count (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/location_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/location_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/login_serializer_ex_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/login_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/membership_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/membership_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/meta_user.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/meta_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/online_function_call_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/online_function_call_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/operation_status.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/operation_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/organization_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/organization_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/organization_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_cloud_storage_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_comment_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_comment_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_invitation_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_invitation_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_issue_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_issue_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_job_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_job_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_label_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_label_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_membership_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_membership_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_meta_user_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_meta_user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_organization_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_organization_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_project_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_project_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_task_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_task_read_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_delivery_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/paginated_webhook_read_list.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/paginated_webhook_read_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/password_change_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_change_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/password_reset_confirm_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_confirm_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/password_reset_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_delivery_read.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,133 +39,105 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
-def lazy_import():
-    from cvat_sdk.api_client.model.basic_user_request import BasicUserRequest
-    from cvat_sdk.api_client.model.credentials_type_enum import CredentialsTypeEnum
-    from cvat_sdk.api_client.model.provider_type_enum import ProviderTypeEnum
-    globals()['BasicUserRequest'] = BasicUserRequest
-    globals()['CredentialsTypeEnum'] = CredentialsTypeEnum
-    globals()['ProviderTypeEnum'] = ProviderTypeEnum
 
 
-
-class IPatchedCloudStorageWriteRequest(IModelData):
+class IWebhookDeliveryRead(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    provider_type: ProviderTypeEnum # noqa: E501
+    id: int # noqa: E501
     """
     [optional]
     """
 
-    resource: str # noqa: E501
+    webhook_id: int # noqa: E501
     """
     [optional]
     """
 
-    display_name: str # noqa: E501
+    event: str # noqa: E501
     """
     [optional]
     """
 
-    owner: BasicUserRequest # noqa: E501
+    status_code: int # noqa: E501
     """
     [optional]
     """
 
-    credentials_type: CredentialsTypeEnum # noqa: E501
+    redelivery: bool # noqa: E501
     """
     [optional]
     """
 
-    session_token: str # noqa: E501
+    created_date: datetime # noqa: E501
     """
     [optional]
     """
 
-    account_name: str # noqa: E501
+    updated_date: datetime # noqa: E501
     """
     [optional]
     """
 
-    key: str # noqa: E501
+    changed_fields: str # noqa: E501
     """
     [optional]
     """
 
-    secret_key: str # noqa: E501
+    request: typing.Dict[str, typing.Union[typing.Any, none_type]] # noqa: E501
     """
     [optional]
+    {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
     """
 
-    key_file: file_type # noqa: E501
+    response: typing.Dict[str, typing.Union[typing.Any, none_type]] # noqa: E501
     """
     [optional]
+    {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
     """
 
-    specific_attributes: str # noqa: E501
-    """
-    [optional]
-    """
 
-    description: str # noqa: E501
-    """
-    [optional]
-    """
-
-    manifests: typing.List[str] # noqa: E501
-    """
-    [optional, default: []]
-    [str]
-    """
-
-
-class PatchedCloudStorageWriteRequest(ModelNormal, IPatchedCloudStorageWriteRequest):
+class WebhookDeliveryRead(ModelNormal, IWebhookDeliveryRead):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      provider_type (ProviderTypeEnum): [optional]  # noqa: E501
-
-      resource (str): [optional]  # noqa: E501
-
-      display_name (str): [optional]  # noqa: E501
+      id (int): [optional]  # noqa: E501
 
-      owner (BasicUserRequest): [optional]  # noqa: E501
+      webhook_id (int): [optional]  # noqa: E501
 
-      credentials_type (CredentialsTypeEnum): [optional]  # noqa: E501
+      event (str): [optional]  # noqa: E501
 
-      session_token (str): [optional]  # noqa: E501
+      status_code (int): [optional]  # noqa: E501
 
-      account_name (str): [optional]  # noqa: E501
+      redelivery (bool): [optional]  # noqa: E501
 
-      key (str): [optional]  # noqa: E501
+      created_date (datetime): [optional]  # noqa: E501
 
-      secret_key (str): [optional]  # noqa: E501
+      updated_date (datetime): [optional]  # noqa: E501
 
-      key_file (file_type): [optional]  # noqa: E501
+      changed_fields (str): [optional]  # noqa: E501
 
-      specific_attributes (str): [optional]  # noqa: E501
+      request ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
 
-      description (str): [optional]  # noqa: E501
-
-      manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+      response ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -182,135 +154,108 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('resource',): {
-            'max_length': 222,
-            'min_length': 1,
-        },
-        ('display_name',): {
-            'max_length': 63,
-            'min_length': 1,
-        },
-        ('session_token',): {
-            'max_length': 440,
-        },
-        ('account_name',): {
-            'max_length': 24,
-        },
-        ('key',): {
-            'max_length': 40,
-        },
-        ('secret_key',): {
-            'max_length': 44,
-        },
-        ('specific_attributes',): {
-            'max_length': 1024,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'provider_type': (ProviderTypeEnum,),  # noqa: E501
-            'resource': (str,),  # noqa: E501
-            'display_name': (str,),  # noqa: E501
-            'owner': (BasicUserRequest,),  # noqa: E501
-            'credentials_type': (CredentialsTypeEnum,),  # noqa: E501
-            'session_token': (str,),  # noqa: E501
-            'account_name': (str,),  # noqa: E501
-            'key': (str,),  # noqa: E501
-            'secret_key': (str,),  # noqa: E501
-            'key_file': (file_type,),  # noqa: E501
-            'specific_attributes': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'manifests': ([str],),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'webhook_id': (int,),  # noqa: E501
+            'event': (str,),  # noqa: E501
+            'status_code': (int,),  # noqa: E501
+            'redelivery': (bool,),  # noqa: E501
+            'created_date': (datetime,),  # noqa: E501
+            'updated_date': (datetime,),  # noqa: E501
+            'changed_fields': (str,),  # noqa: E501
+            'request': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'response': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'provider_type': 'provider_type',  # noqa: E501
-        'resource': 'resource',  # noqa: E501
-        'display_name': 'display_name',  # noqa: E501
-        'owner': 'owner',  # noqa: E501
-        'credentials_type': 'credentials_type',  # noqa: E501
-        'session_token': 'session_token',  # noqa: E501
-        'account_name': 'account_name',  # noqa: E501
-        'key': 'key',  # noqa: E501
-        'secret_key': 'secret_key',  # noqa: E501
-        'key_file': 'key_file',  # noqa: E501
-        'specific_attributes': 'specific_attributes',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'manifests': 'manifests',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'webhook_id': 'webhook_id',  # noqa: E501
+        'event': 'event',  # noqa: E501
+        'status_code': 'status_code',  # noqa: E501
+        'redelivery': 'redelivery',  # noqa: E501
+        'created_date': 'created_date',  # noqa: E501
+        'updated_date': 'updated_date',  # noqa: E501
+        'changed_fields': 'changed_fields',  # noqa: E501
+        'request': 'request',  # noqa: E501
+        'response': 'response',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
+        'webhook_id',  # noqa: E501
+        'event',  # noqa: E501
+        'status_code',  # noqa: E501
+        'redelivery',  # noqa: E501
+        'created_date',  # noqa: E501
+        'updated_date',  # noqa: E501
+        'changed_fields',  # noqa: E501
+        'request',  # noqa: E501
+        'response',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchedCloudStorageWriteRequest - a model defined in OpenAPI
+        """WebhookDeliveryRead - a model defined in OpenAPI
 
         Keyword Args:
-            provider_type (ProviderTypeEnum): [optional]  # noqa: E501
-
-            resource (str): [optional]  # noqa: E501
+            id (int): [optional]  # noqa: E501
 
-            display_name (str): [optional]  # noqa: E501
+            webhook_id (int): [optional]  # noqa: E501
 
-            owner (BasicUserRequest): [optional]  # noqa: E501
+            event (str): [optional]  # noqa: E501
 
-            credentials_type (CredentialsTypeEnum): [optional]  # noqa: E501
+            status_code (int): [optional]  # noqa: E501
 
-            session_token (str): [optional]  # noqa: E501
+            redelivery (bool): [optional]  # noqa: E501
 
-            account_name (str): [optional]  # noqa: E501
+            created_date (datetime): [optional]  # noqa: E501
 
-            key (str): [optional]  # noqa: E501
+            updated_date (datetime): [optional]  # noqa: E501
 
-            secret_key (str): [optional]  # noqa: E501
+            changed_fields (str): [optional]  # noqa: E501
 
-            key_file (file_type): [optional]  # noqa: E501
+            request ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
 
-            specific_attributes (str): [optional]  # noqa: E501
-
-            description (str): [optional]  # noqa: E501
-
-            manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            response ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -387,42 +332,36 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchedCloudStorageWriteRequest - a model defined in OpenAPI
+        """WebhookDeliveryRead - a model defined in OpenAPI
 
         Keyword Args:
-            provider_type (ProviderTypeEnum): [optional]  # noqa: E501
-
-            resource (str): [optional]  # noqa: E501
-
-            display_name (str): [optional]  # noqa: E501
-
-            owner (BasicUserRequest): [optional]  # noqa: E501
+            id (int): [optional]  # noqa: E501
 
-            credentials_type (CredentialsTypeEnum): [optional]  # noqa: E501
+            webhook_id (int): [optional]  # noqa: E501
 
-            session_token (str): [optional]  # noqa: E501
+            event (str): [optional]  # noqa: E501
 
-            account_name (str): [optional]  # noqa: E501
+            status_code (int): [optional]  # noqa: E501
 
-            key (str): [optional]  # noqa: E501
+            redelivery (bool): [optional]  # noqa: E501
 
-            secret_key (str): [optional]  # noqa: E501
+            created_date (datetime): [optional]  # noqa: E501
 
-            key_file (file_type): [optional]  # noqa: E501
+            updated_date (datetime): [optional]  # noqa: E501
 
-            specific_attributes (str): [optional]  # noqa: E501
+            changed_fields (str): [optional]  # noqa: E501
 
-            description (str): [optional]  # noqa: E501
+            request ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
 
-            manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
+            response ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_comment_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_comment_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_data_meta_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_data_meta_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_invitation_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_invitation_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_issue_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_issue_write_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -61,19 +61,14 @@
     """
 
     assignee: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
     """
 
-    message: str # noqa: E501
-    """
-    [optional]
-    """
-
     resolved: bool # noqa: E501
     """
     [optional]
     """
 
 
 class PatchedIssueWriteRequest(ModelNormal, IPatchedIssueWriteRequest):
@@ -84,16 +79,14 @@
     Do not edit the class manually.
 
     Attributes:
       position ([float]): [optional]  # noqa: E501
 
       assignee (int, none_type): [optional]  # noqa: E501
 
-      message (str): [optional]  # noqa: E501
-
       resolved (bool): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
@@ -111,17 +104,14 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('message',): {
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -139,28 +129,26 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'position': ([float],),  # noqa: E501
             'assignee': (int, none_type,),  # noqa: E501
-            'message': (str,),  # noqa: E501
             'resolved': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
         'position': 'position',  # noqa: E501
         'assignee': 'assignee',  # noqa: E501
-        'message': 'message',  # noqa: E501
         'resolved': 'resolved',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -171,16 +159,14 @@
         """PatchedIssueWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
             position ([float]): [optional]  # noqa: E501
 
             assignee (int, none_type): [optional]  # noqa: E501
 
-            message (str): [optional]  # noqa: E501
-
             resolved (bool): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -265,16 +251,14 @@
         """PatchedIssueWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
             position ([float]): [optional]  # noqa: E501
 
             assignee (int, none_type): [optional]  # noqa: E501
 
-            message (str): [optional]  # noqa: E501
-
             resolved (bool): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_job_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_job_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_label_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_label_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_labeled_data_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_labeled_data_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_membership_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_membership_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_organization_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_organization_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_project_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_project_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_task_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_task_write_request_target_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_user_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/patched_webhook_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_webhook_write_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -86,19 +86,14 @@
     """
 
     enable_ssl: bool # noqa: E501
     """
     [optional]
     """
 
-    project_id: typing.Union[int, none_type] # noqa: E501
-    """
-    [optional]
-    """
-
     events: typing.List[EventsEnum] # noqa: E501
     """
     [optional]
     [EventsEnum]
     """
 
 
@@ -118,16 +113,14 @@
 
       secret (str): [optional]  # noqa: E501
 
       is_active (bool): [optional]  # noqa: E501
 
       enable_ssl (bool): [optional]  # noqa: E501
 
-      project_id (int, none_type): [optional]  # noqa: E501
-
       events ([EventsEnum]): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
@@ -146,15 +139,15 @@
     """
 
     allowed_values = {
     }
 
     validations = {
         ('target_url',): {
-            'max_length': 200,
+            'max_length': 8192,
             'min_length': 1,
         },
         ('description',): {
             'max_length': 128,
         },
         ('secret',): {
             'max_length': 64,
@@ -186,15 +179,14 @@
         return {
             'target_url': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'content_type': (WebhookContentType,),  # noqa: E501
             'secret': (str,),  # noqa: E501
             'is_active': (bool,),  # noqa: E501
             'enable_ssl': (bool,),  # noqa: E501
-            'project_id': (int, none_type,),  # noqa: E501
             'events': ([EventsEnum],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -203,15 +195,14 @@
     attribute_map = {
         'target_url': 'target_url',  # noqa: E501
         'description': 'description',  # noqa: E501
         'content_type': 'content_type',  # noqa: E501
         'secret': 'secret',  # noqa: E501
         'is_active': 'is_active',  # noqa: E501
         'enable_ssl': 'enable_ssl',  # noqa: E501
-        'project_id': 'project_id',  # noqa: E501
         'events': 'events',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -230,16 +221,14 @@
 
             secret (str): [optional]  # noqa: E501
 
             is_active (bool): [optional]  # noqa: E501
 
             enable_ssl (bool): [optional]  # noqa: E501
 
-            project_id (int, none_type): [optional]  # noqa: E501
-
             events ([EventsEnum]): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -332,16 +321,14 @@
 
             secret (str): [optional]  # noqa: E501
 
             is_active (bool): [optional]  # noqa: E501
 
             enable_ssl (bool): [optional]  # noqa: E501
 
-            project_id (int, none_type): [optional]  # noqa: E501
-
             events ([EventsEnum]): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/plugins.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_file_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_file_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/patched_cloud_storage_write_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -40,157 +40,139 @@
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 def lazy_import():
-    from cvat_sdk.api_client.model.job_read_assignee import JobReadAssignee
-    from cvat_sdk.api_client.model.job_status import JobStatus
-    from cvat_sdk.api_client.model.labels_summary import LabelsSummary
-    from cvat_sdk.api_client.model.project_read_owner import ProjectReadOwner
-    from cvat_sdk.api_client.model.project_read_target_storage import ProjectReadTargetStorage
-    from cvat_sdk.api_client.model.tasks_summary import TasksSummary
-    globals()['JobReadAssignee'] = JobReadAssignee
-    globals()['JobStatus'] = JobStatus
-    globals()['LabelsSummary'] = LabelsSummary
-    globals()['ProjectReadOwner'] = ProjectReadOwner
-    globals()['ProjectReadTargetStorage'] = ProjectReadTargetStorage
-    globals()['TasksSummary'] = TasksSummary
+    from cvat_sdk.api_client.model.basic_user_request import BasicUserRequest
+    from cvat_sdk.api_client.model.credentials_type_enum import CredentialsTypeEnum
+    from cvat_sdk.api_client.model.provider_type_enum import ProviderTypeEnum
+    globals()['BasicUserRequest'] = BasicUserRequest
+    globals()['CredentialsTypeEnum'] = CredentialsTypeEnum
+    globals()['ProviderTypeEnum'] = ProviderTypeEnum
 
 
 
-class IProjectRead(IModelData):
+class IPatchedCloudStorageWriteRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    url: str # noqa: E501
+    provider_type: ProviderTypeEnum # noqa: E501
     """
     [optional]
     """
 
-    id: int # noqa: E501
+    resource: str # noqa: E501
     """
     [optional]
     """
 
-    name: str # noqa: E501
+    display_name: str # noqa: E501
     """
     [optional]
     """
 
-    owner: ProjectReadOwner # noqa: E501
+    owner: BasicUserRequest # noqa: E501
     """
     [optional]
     """
 
-    assignee: JobReadAssignee # noqa: E501
+    credentials_type: CredentialsTypeEnum # noqa: E501
     """
     [optional]
     """
 
-    bug_tracker: str # noqa: E501
+    session_token: str # noqa: E501
     """
     [optional]
     """
 
-    task_subsets: typing.List[str] # noqa: E501
-    """
-    [optional]
-    [str]
-    """
-
-    created_date: datetime # noqa: E501
+    account_name: str # noqa: E501
     """
     [optional]
     """
 
-    updated_date: datetime # noqa: E501
+    key: str # noqa: E501
     """
     [optional]
     """
 
-    status: typing.Union[typing.Any, none_type] # noqa: E501
+    secret_key: str # noqa: E501
     """
     [optional]
     """
 
-    dimension: typing.Union[str, none_type] # noqa: E501
+    connection_string: str # noqa: E501
     """
     [optional]
     """
 
-    organization: typing.Union[int, none_type] # noqa: E501
+    key_file: file_type # noqa: E501
     """
     [optional]
     """
 
-    target_storage: ProjectReadTargetStorage # noqa: E501
+    specific_attributes: str # noqa: E501
     """
     [optional]
     """
 
-    source_storage: ProjectReadTargetStorage # noqa: E501
+    description: str # noqa: E501
     """
     [optional]
     """
 
-    tasks: TasksSummary # noqa: E501
-    """
-    """
-
-    labels: LabelsSummary # noqa: E501
+    manifests: typing.List[str] # noqa: E501
     """
+    [optional, default: []]
+    [str]
     """
 
 
-class ProjectRead(ModelNormal, IProjectRead):
+class PatchedCloudStorageWriteRequest(ModelNormal, IPatchedCloudStorageWriteRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      tasks (TasksSummary):
-
-      labels (LabelsSummary):
+      provider_type (ProviderTypeEnum): [optional]  # noqa: E501
 
-      url (str): [optional]  # noqa: E501
+      resource (str): [optional]  # noqa: E501
 
-      id (int): [optional]  # noqa: E501
+      display_name (str): [optional]  # noqa: E501
 
-      name (str): [optional]  # noqa: E501
+      owner (BasicUserRequest): [optional]  # noqa: E501
 
-      owner (ProjectReadOwner): [optional]  # noqa: E501
+      credentials_type (CredentialsTypeEnum): [optional]  # noqa: E501
 
-      assignee (JobReadAssignee): [optional]  # noqa: E501
+      session_token (str): [optional]  # noqa: E501
 
-      bug_tracker (str): [optional]  # noqa: E501
+      account_name (str): [optional]  # noqa: E501
 
-      task_subsets ([str]): [optional]  # noqa: E501
+      key (str): [optional]  # noqa: E501
 
-      created_date (datetime): [optional]  # noqa: E501
+      secret_key (str): [optional]  # noqa: E501
 
-      updated_date (datetime): [optional]  # noqa: E501
+      connection_string (str): [optional]  # noqa: E501
 
-      status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+      key_file (file_type): [optional]  # noqa: E501
 
-      dimension (str, none_type): [optional]  # noqa: E501
+      specific_attributes (str): [optional]  # noqa: E501
 
-      organization (int, none_type): [optional]  # noqa: E501
+      description (str): [optional]  # noqa: E501
 
-      target_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
-
-      source_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
+      manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -207,16 +189,39 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('dimension',): {
-            'max_length': 16,
+        ('resource',): {
+            'max_length': 222,
+            'min_length': 1,
+        },
+        ('display_name',): {
+            'max_length': 63,
+            'min_length': 1,
+        },
+        ('session_token',): {
+            'max_length': 440,
+        },
+        ('account_name',): {
+            'max_length': 24,
+        },
+        ('key',): {
+            'max_length': 40,
+        },
+        ('secret_key',): {
+            'max_length': 44,
+        },
+        ('connection_string',): {
+            'max_length': 440,
+        },
+        ('specific_attributes',): {
+            'max_length': 1024,
         },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
@@ -235,109 +240,91 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'tasks': (TasksSummary,),  # noqa: E501
-            'labels': (LabelsSummary,),  # noqa: E501
-            'url': (str,),  # noqa: E501
-            'id': (int,),  # noqa: E501
-            'name': (str,),  # noqa: E501
-            'owner': (ProjectReadOwner,),  # noqa: E501
-            'assignee': (JobReadAssignee,),  # noqa: E501
-            'bug_tracker': (str,),  # noqa: E501
-            'task_subsets': ([str],),  # noqa: E501
-            'created_date': (datetime,),  # noqa: E501
-            'updated_date': (datetime,),  # noqa: E501
-            'status': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'dimension': (str, none_type,),  # noqa: E501
-            'organization': (int, none_type,),  # noqa: E501
-            'target_storage': (ProjectReadTargetStorage,),  # noqa: E501
-            'source_storage': (ProjectReadTargetStorage,),  # noqa: E501
+            'provider_type': (ProviderTypeEnum,),  # noqa: E501
+            'resource': (str,),  # noqa: E501
+            'display_name': (str,),  # noqa: E501
+            'owner': (BasicUserRequest,),  # noqa: E501
+            'credentials_type': (CredentialsTypeEnum,),  # noqa: E501
+            'session_token': (str,),  # noqa: E501
+            'account_name': (str,),  # noqa: E501
+            'key': (str,),  # noqa: E501
+            'secret_key': (str,),  # noqa: E501
+            'connection_string': (str,),  # noqa: E501
+            'key_file': (file_type,),  # noqa: E501
+            'specific_attributes': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'manifests': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'tasks': 'tasks',  # noqa: E501
-        'labels': 'labels',  # noqa: E501
-        'url': 'url',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
+        'provider_type': 'provider_type',  # noqa: E501
+        'resource': 'resource',  # noqa: E501
+        'display_name': 'display_name',  # noqa: E501
         'owner': 'owner',  # noqa: E501
-        'assignee': 'assignee',  # noqa: E501
-        'bug_tracker': 'bug_tracker',  # noqa: E501
-        'task_subsets': 'task_subsets',  # noqa: E501
-        'created_date': 'created_date',  # noqa: E501
-        'updated_date': 'updated_date',  # noqa: E501
-        'status': 'status',  # noqa: E501
-        'dimension': 'dimension',  # noqa: E501
-        'organization': 'organization',  # noqa: E501
-        'target_storage': 'target_storage',  # noqa: E501
-        'source_storage': 'source_storage',  # noqa: E501
+        'credentials_type': 'credentials_type',  # noqa: E501
+        'session_token': 'session_token',  # noqa: E501
+        'account_name': 'account_name',  # noqa: E501
+        'key': 'key',  # noqa: E501
+        'secret_key': 'secret_key',  # noqa: E501
+        'connection_string': 'connection_string',  # noqa: E501
+        'key_file': 'key_file',  # noqa: E501
+        'specific_attributes': 'specific_attributes',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'manifests': 'manifests',  # noqa: E501
     }
 
     read_only_vars = {
-        'url',  # noqa: E501
-        'id',  # noqa: E501
-        'name',  # noqa: E501
-        'bug_tracker',  # noqa: E501
-        'task_subsets',  # noqa: E501
-        'created_date',  # noqa: E501
-        'updated_date',  # noqa: E501
-        'status',  # noqa: E501
-        'dimension',  # noqa: E501
-        'organization',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, tasks, labels, *args, **kwargs):  # noqa: E501
-        """ProjectRead - a model defined in OpenAPI
-
-        Args:
-            tasks (TasksSummary):
-            labels (LabelsSummary):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """PatchedCloudStorageWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            url (str): [optional]  # noqa: E501
+            provider_type (ProviderTypeEnum): [optional]  # noqa: E501
 
-            id (int): [optional]  # noqa: E501
+            resource (str): [optional]  # noqa: E501
 
-            name (str): [optional]  # noqa: E501
+            display_name (str): [optional]  # noqa: E501
 
-            owner (ProjectReadOwner): [optional]  # noqa: E501
+            owner (BasicUserRequest): [optional]  # noqa: E501
 
-            assignee (JobReadAssignee): [optional]  # noqa: E501
+            credentials_type (CredentialsTypeEnum): [optional]  # noqa: E501
 
-            bug_tracker (str): [optional]  # noqa: E501
+            session_token (str): [optional]  # noqa: E501
 
-            task_subsets ([str]): [optional]  # noqa: E501
+            account_name (str): [optional]  # noqa: E501
 
-            created_date (datetime): [optional]  # noqa: E501
+            key (str): [optional]  # noqa: E501
 
-            updated_date (datetime): [optional]  # noqa: E501
+            secret_key (str): [optional]  # noqa: E501
 
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            connection_string (str): [optional]  # noqa: E501
 
-            dimension (str, none_type): [optional]  # noqa: E501
+            key_file (file_type): [optional]  # noqa: E501
 
-            organization (int, none_type): [optional]  # noqa: E501
+            specific_attributes (str): [optional]  # noqa: E501
 
-            target_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
 
-            source_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
+            manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -393,16 +380,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.tasks = tasks
-        self.labels = labels
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -415,49 +400,45 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, tasks, labels, *args, **kwargs):  # noqa: E501
-        """ProjectRead - a model defined in OpenAPI
-
-        Args:
-            tasks (TasksSummary):
-            labels (LabelsSummary):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """PatchedCloudStorageWriteRequest - a model defined in OpenAPI
 
         Keyword Args:
-            url (str): [optional]  # noqa: E501
+            provider_type (ProviderTypeEnum): [optional]  # noqa: E501
 
-            id (int): [optional]  # noqa: E501
+            resource (str): [optional]  # noqa: E501
 
-            name (str): [optional]  # noqa: E501
+            display_name (str): [optional]  # noqa: E501
 
-            owner (ProjectReadOwner): [optional]  # noqa: E501
+            owner (BasicUserRequest): [optional]  # noqa: E501
 
-            assignee (JobReadAssignee): [optional]  # noqa: E501
+            credentials_type (CredentialsTypeEnum): [optional]  # noqa: E501
 
-            bug_tracker (str): [optional]  # noqa: E501
+            session_token (str): [optional]  # noqa: E501
 
-            task_subsets ([str]): [optional]  # noqa: E501
+            account_name (str): [optional]  # noqa: E501
 
-            created_date (datetime): [optional]  # noqa: E501
+            key (str): [optional]  # noqa: E501
 
-            updated_date (datetime): [optional]  # noqa: E501
+            secret_key (str): [optional]  # noqa: E501
 
-            status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            connection_string (str): [optional]  # noqa: E501
 
-            dimension (str, none_type): [optional]  # noqa: E501
+            key_file (file_type): [optional]  # noqa: E501
 
-            organization (int, none_type): [optional]  # noqa: E501
+            specific_attributes (str): [optional]  # noqa: E501
 
-            target_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
+            description (str): [optional]  # noqa: E501
 
-            source_storage (ProjectReadTargetStorage): [optional]  # noqa: E501
+            manifests ([str]): [optional] if omitted the server will use the default value of []  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -511,16 +492,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.tasks = tasks
-        self.labels = labels
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_read_owner.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_owner.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_read_target_storage.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_read_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/project_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/project_write_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/provider_type_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/provider_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/register_serializer_ex.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/register_serializer_ex_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/register_serializer_ex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/rest_auth_detail.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/rest_auth_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/role_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/role_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/rq_status.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/rq_status_state_enum.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/rq_status_state_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/shape_type.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/shape_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/signing_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/signing_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sorting_method.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sorting_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage_method.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/storage_type.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/storage_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_shape.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_shape_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_track.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sub_labeled_track_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sub_labeled_track_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sublabel.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/sublabel_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/sublabel_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_annotations_update_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_annotations_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_annotations_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_file_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_file_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_read_target_storage.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_read_target_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/task_write_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/task_write_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/tasks_summary.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/issues_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -41,46 +41,46 @@
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
 
 
-class ITasksSummary(IModelData):
+class IIssuesSummary(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    count: int # noqa: E501
+    url: str # noqa: E501
     """
-    [optional, default: 0]
+    [optional]
     """
 
-    url: str # noqa: E501
+    count: int # noqa: E501
     """
     [optional]
     """
 
 
-class TasksSummary(ModelNormal, ITasksSummary):
+class IssuesSummary(ModelNormal, IIssuesSummary):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
       url (str): [optional]  # noqa: E501
 
+      count (int): [optional]  # noqa: E501
+
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
           and the value is json key in definition.
@@ -119,45 +119,46 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'count': (int,),  # noqa: E501
             'url': (str,),  # noqa: E501
+            'count': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'count': 'count',  # noqa: E501
         'url': 'url',  # noqa: E501
+        'count': 'count',  # noqa: E501
     }
 
     read_only_vars = {
         'url',  # noqa: E501
+        'count',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """TasksSummary - a model defined in OpenAPI
+        """IssuesSummary - a model defined in OpenAPI
 
         Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
             url (str): [optional]  # noqa: E501
 
+            count (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -233,21 +234,21 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """TasksSummary - a model defined in OpenAPI
+        """IssuesSummary - a model defined in OpenAPI
 
         Keyword Args:
-            count (int): [optional] if omitted the server will use the default value of 0  # noqa: E501
-
             url (str): [optional]  # noqa: E501
 
+            count (int): [optional]  # noqa: E501
+
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/token.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/tracked_shape.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/tracked_shape_request.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/tracked_shape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/user.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_content_type.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_content_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_delivery_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_write_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
@@ -39,105 +39,102 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     # Enable introspection. Can't work normally due to cyclic imports
     from cvat_sdk.api_client.apis import *
     from cvat_sdk.api_client.models import *
 
 
+def lazy_import():
+    from cvat_sdk.api_client.model.events_enum import EventsEnum
+    from cvat_sdk.api_client.model.webhook_content_type import WebhookContentType
+    from cvat_sdk.api_client.model.webhook_type import WebhookType
+    globals()['EventsEnum'] = EventsEnum
+    globals()['WebhookContentType'] = WebhookContentType
+    globals()['WebhookType'] = WebhookType
 
 
-class IWebhookDeliveryRead(IModelData):
+
+class IWebhookWriteRequest(IModelData):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     # member type declarations
-    id: int # noqa: E501
-    """
-    [optional]
-    """
-
-    webhook_id: int # noqa: E501
+    target_url: str # noqa: E501
     """
-    [optional]
     """
 
-    event: str # noqa: E501
+    description: str # noqa: E501
     """
     [optional]
     """
 
-    status_code: int # noqa: E501
+    type: WebhookType # noqa: E501
     """
-    [optional]
     """
 
-    redelivery: bool # noqa: E501
+    content_type: WebhookContentType # noqa: E501
     """
     [optional]
     """
 
-    created_date: datetime # noqa: E501
+    secret: str # noqa: E501
     """
     [optional]
     """
 
-    updated_date: datetime # noqa: E501
+    is_active: bool # noqa: E501
     """
     [optional]
     """
 
-    changed_fields: str # noqa: E501
+    enable_ssl: bool # noqa: E501
     """
     [optional]
     """
 
-    request: typing.Dict[str, typing.Union[typing.Any, none_type]] # noqa: E501
+    project_id: typing.Union[int, none_type] # noqa: E501
     """
     [optional]
-    {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
     """
 
-    response: typing.Dict[str, typing.Union[typing.Any, none_type]] # noqa: E501
+    events: typing.List[EventsEnum] # noqa: E501
     """
-    [optional]
-    {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+    [EventsEnum]
     """
 
 
-class WebhookDeliveryRead(ModelNormal, IWebhookDeliveryRead):
+class WebhookWriteRequest(ModelNormal, IWebhookWriteRequest):
     """
     NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
-      id (int): [optional]  # noqa: E501
+      target_url (str):
 
-      webhook_id (int): [optional]  # noqa: E501
+      type (WebhookType):
 
-      event (str): [optional]  # noqa: E501
+      events ([EventsEnum]):
 
-      status_code (int): [optional]  # noqa: E501
+      description (str): [optional]  # noqa: E501
 
-      redelivery (bool): [optional]  # noqa: E501
+      content_type (WebhookContentType): [optional]  # noqa: E501
 
-      created_date (datetime): [optional]  # noqa: E501
+      secret (str): [optional]  # noqa: E501
 
-      updated_date (datetime): [optional]  # noqa: E501
+      is_active (bool): [optional]  # noqa: E501
 
-      changed_fields (str): [optional]  # noqa: E501
+      enable_ssl (bool): [optional]  # noqa: E501
 
-      request ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-
-      response ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+      project_id (int, none_type): [optional]  # noqa: E501
 
 
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
       attribute_map (dict): The key is attribute name
@@ -154,108 +151,105 @@
 
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('target_url',): {
+            'max_length': 8192,
+            'min_length': 1,
+        },
+        ('description',): {
+            'max_length': 128,
+        },
+        ('secret',): {
+            'max_length': 64,
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'id': (int,),  # noqa: E501
-            'webhook_id': (int,),  # noqa: E501
-            'event': (str,),  # noqa: E501
-            'status_code': (int,),  # noqa: E501
-            'redelivery': (bool,),  # noqa: E501
-            'created_date': (datetime,),  # noqa: E501
-            'updated_date': (datetime,),  # noqa: E501
-            'changed_fields': (str,),  # noqa: E501
-            'request': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'response': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'target_url': (str,),  # noqa: E501
+            'type': (WebhookType,),  # noqa: E501
+            'events': ([EventsEnum],),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'content_type': (WebhookContentType,),  # noqa: E501
+            'secret': (str,),  # noqa: E501
+            'is_active': (bool,),  # noqa: E501
+            'enable_ssl': (bool,),  # noqa: E501
+            'project_id': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'webhook_id': 'webhook_id',  # noqa: E501
-        'event': 'event',  # noqa: E501
-        'status_code': 'status_code',  # noqa: E501
-        'redelivery': 'redelivery',  # noqa: E501
-        'created_date': 'created_date',  # noqa: E501
-        'updated_date': 'updated_date',  # noqa: E501
-        'changed_fields': 'changed_fields',  # noqa: E501
-        'request': 'request',  # noqa: E501
-        'response': 'response',  # noqa: E501
+        'target_url': 'target_url',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'events': 'events',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'content_type': 'content_type',  # noqa: E501
+        'secret': 'secret',  # noqa: E501
+        'is_active': 'is_active',  # noqa: E501
+        'enable_ssl': 'enable_ssl',  # noqa: E501
+        'project_id': 'project_id',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
-        'webhook_id',  # noqa: E501
-        'event',  # noqa: E501
-        'status_code',  # noqa: E501
-        'redelivery',  # noqa: E501
-        'created_date',  # noqa: E501
-        'updated_date',  # noqa: E501
-        'changed_fields',  # noqa: E501
-        'request',  # noqa: E501
-        'response',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WebhookDeliveryRead - a model defined in OpenAPI
+    def _from_openapi_data(cls, target_url, type, events, *args, **kwargs):  # noqa: E501
+        """WebhookWriteRequest - a model defined in OpenAPI
 
-        Keyword Args:
-            id (int): [optional]  # noqa: E501
+        Args:
+            target_url (str):
+            type (WebhookType):
+            events ([EventsEnum]):
 
-            webhook_id (int): [optional]  # noqa: E501
-
-            event (str): [optional]  # noqa: E501
-
-            status_code (int): [optional]  # noqa: E501
-
-            redelivery (bool): [optional]  # noqa: E501
+        Keyword Args:
+            description (str): [optional]  # noqa: E501
 
-            created_date (datetime): [optional]  # noqa: E501
+            content_type (WebhookContentType): [optional]  # noqa: E501
 
-            updated_date (datetime): [optional]  # noqa: E501
+            secret (str): [optional]  # noqa: E501
 
-            changed_fields (str): [optional]  # noqa: E501
+            is_active (bool): [optional]  # noqa: E501
 
-            request ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            enable_ssl (bool): [optional]  # noqa: E501
 
-            response ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            project_id (int, none_type): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -311,14 +305,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.target_url = target_url
+        self.type = type
+        self.events = events
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -331,37 +328,34 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """WebhookDeliveryRead - a model defined in OpenAPI
+    def __init__(self, target_url, type, events, *args, **kwargs):  # noqa: E501
+        """WebhookWriteRequest - a model defined in OpenAPI
 
-        Keyword Args:
-            id (int): [optional]  # noqa: E501
+        Args:
+            target_url (str):
+            type (WebhookType):
+            events ([EventsEnum]):
 
-            webhook_id (int): [optional]  # noqa: E501
-
-            event (str): [optional]  # noqa: E501
-
-            status_code (int): [optional]  # noqa: E501
-
-            redelivery (bool): [optional]  # noqa: E501
+        Keyword Args:
+            description (str): [optional]  # noqa: E501
 
-            created_date (datetime): [optional]  # noqa: E501
+            content_type (WebhookContentType): [optional]  # noqa: E501
 
-            updated_date (datetime): [optional]  # noqa: E501
+            secret (str): [optional]  # noqa: E501
 
-            changed_fields (str): [optional]  # noqa: E501
+            is_active (bool): [optional]  # noqa: E501
 
-            request ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            enable_ssl (bool): [optional]  # noqa: E501
 
-            response ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            project_id (int, none_type): [optional]  # noqa: E501
 
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -415,14 +409,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.target_url = target_url
+        self.type = type
+        self.events = events
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_read.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model/webhook_type.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model/webhook_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from __future__ import annotations
 
 import typing
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/model_utils.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/models/__init__.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/api_client/rest.py` & `cvat_sdk-2.4.4/cvat_sdk/api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import io
 import json
 import logging
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/client.py` & `cvat_sdk-2.4.4/cvat_sdk/core/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import urllib.parse
 from contextlib import contextmanager, suppress
 from pathlib import Path
 from time import sleep
 from typing import Any, Dict, Iterator, Optional, Sequence, Tuple, TypeVar
 
 import attrs
+import packaging.specifiers as specifiers
 import packaging.version as pv
 import platformdirs
 import urllib3
 import urllib3.exceptions
 
 from cvat_sdk.api_client import ApiClient, Configuration, exceptions, models
 from cvat_sdk.core.exceptions import IncompatibleVersionException, InvalidHostException
@@ -57,18 +58,14 @@
 class Client:
     """
     Provides session management, implements authentication operations
     and simplifies access to server APIs.
     """
 
     SUPPORTED_SERVER_VERSIONS = (
-        pv.Version("2.0"),
-        pv.Version("2.1"),
-        pv.Version("2.2"),
-        pv.Version("2.3"),
         pv.Version("2.4"),
         pv.Version("2.5"),
     )
 
     def __init__(
         self,
         url: str,
@@ -253,33 +250,37 @@
                 "Some SDK functions may not work properly with this server."
             ) % (e,)
             self.logger.warning(msg)
             if fail_if_unsupported:
                 raise IncompatibleVersionException(msg)
             return
 
-        sdk_version = pv.Version(VERSION)
-
-        # We only check base version match. Micro releases and fixes do not affect
-        # API compatibility in general.
-        if all(
-            server_version.base_version != sv.base_version for sv in self.SUPPORTED_SERVER_VERSIONS
+        if not any(
+            self._is_version_compatible(server_version, supported_version)
+            for supported_version in self.SUPPORTED_SERVER_VERSIONS
         ):
             msg = (
                 "Server version '%s' is not compatible with SDK version '%s'. "
                 "Some SDK functions may not work properly with this server. "
                 "You can continue using this SDK, or you can "
                 "try to update with 'pip install cvat-sdk'."
-            ) % (server_version, sdk_version)
+            ) % (server_version, pv.Version(VERSION))
             self.logger.warning(msg)
             if fail_if_unsupported:
                 raise IncompatibleVersionException(msg)
 
+    def _is_version_compatible(self, current: pv.Version, target: pv.Version) -> bool:
+        # Check for (major, minor) compatibility.
+        # Micro releases and fixes do not affect API compatibility in general.
+        epoch = f"{target.epoch}!" if target.epoch else ""  # 1.0 ~= 0!1.0 is false
+        return current in specifiers.Specifier(
+            f"~= {epoch}{target.major}.{target.minor}.{target.micro}"
+        )
+
     def get_server_version(self) -> pv.Version:
-        # TODO: allow to use this endpoint unauthorized
         (about, _) = self.api_client.server_api.retrieve_about()
         return pv.Version(about.version)
 
     def _get_repo(self, repo_type: _RepoType) -> _RepoType:
         repo = self._repos.get(repo_type, None)
         if repo is None:
             repo = repo_type(self)
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/downloading.py` & `cvat_sdk-2.4.4/cvat_sdk/core/downloading.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             url,
             _request_timeout=timeout,
             headers=self._client.api_client.get_common_headers(),
             _parse_response=False,
         )
         with closing(response):
             try:
-                file_size = int(response.getheader("Content-Length", 0))
+                file_size = int(response.headers.get("Content-Length", 0))
             except ValueError:
                 file_size = None
 
             with atomic_writer(output_path, "wb") as fd:
                 if pbar is not None:
                     pbar.start(file_size, desc="Downloading")
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/git.py` & `cvat_sdk-2.4.4/cvat_sdk/core/git.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/helpers.py` & `cvat_sdk-2.4.4/cvat_sdk/core/helpers.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/progress.py` & `cvat_sdk-2.4.4/cvat_sdk/core/progress.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/annotations.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/annotations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/issues.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/issues.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/jobs.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/jobs.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/model_proxy.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/model_proxy.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/organizations.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/organizations.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/projects.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/projects.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/tasks.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/tasks.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/proxies/users.py` & `cvat_sdk-2.4.4/cvat_sdk/core/proxies/users.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/uploading.py` & `cvat_sdk-2.4.4/cvat_sdk/core/uploading.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/core/utils.py` & `cvat_sdk-2.4.4/cvat_sdk/core/utils.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/pytorch/caching.py` & `cvat_sdk-2.4.4/cvat_sdk/pytorch/caching.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/pytorch/common.py` & `cvat_sdk-2.4.4/cvat_sdk/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/pytorch/project_dataset.py` & `cvat_sdk-2.4.4/cvat_sdk/pytorch/project_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/pytorch/task_dataset.py` & `cvat_sdk-2.4.4/cvat_sdk/pytorch/task_dataset.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk/pytorch/transforms.py` & `cvat_sdk-2.4.4/cvat_sdk/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/cvat_sdk.egg-info/PKG-INFO` & `cvat_sdk-2.4.4/cvat_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-sdk
-Version: 2.4.0
+Version: 2.4.4
 Summary: CVAT REST API
 Home-page: https://github.com/cvat-ai/cvat
 Author: CVAT.ai team
 Author-email: support@cvat.ai
 License: MIT License
 Keywords: OpenAPI,OpenAPI-Generator,CVAT REST API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cvat_sdk-2.4.0/cvat_sdk.egg-info/SOURCES.txt` & `cvat_sdk-2.4.4/cvat_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvat_sdk-2.4.0/setup.py` & `cvat_sdk-2.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 # CVAT REST API
 #
 # REST API for Computer Vision Annotation Tool (CVAT)  # noqa: E501
 #
-# The version of the OpenAPI document: 2.5
+# The version of the OpenAPI document: 2.4.4
 # Contact: support@cvat.ai
 # Generated by: https://openapi-generator.tech
 
 
 import os.path as osp
 import re
 from setuptools import find_packages, setup
```

