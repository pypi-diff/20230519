# Comparing `tmp/kdp-api-python-client-4.8.0.tar.gz` & `tmp/kdp-api-python-client-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-api-python-client-4.8.0.tar", last modified: Tue Oct 25 22:26:08 2022, max compression
+gzip compressed data, was "kdp-api-python-client-4.9.0.tar", last modified: Wed Oct 26 03:13:21 2022, max compression
```

## Comparing `kdp-api-python-client-4.8.0.tar` & `kdp-api-python-client-4.9.0.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.849774 kdp-api-python-client-4.8.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      401 2022-10-25 22:26:08.853774 kdp-api-python-client-4.8.0/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    21319 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.793773 kdp-api-python-client-4.8.0/kdp_api/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      723 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.797773 kdp-api-python-client-4.8.0/kdp_api/api/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      220 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11229 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/abac_label_parsers_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31024 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/applications_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    32871 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/attribute_assignments_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30817 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/attributes_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10593 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/api/authentication_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31701 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/dataset_permissions_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30607 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/datasets_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31532 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/group_memberships_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30447 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/groups_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30382 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/indexes_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6219 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/ingest_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    25662 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/jobs_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16466 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/query_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16010 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/read_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11851 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/segments_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10958 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/source_types_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30324 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/users_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26228 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/workspaces_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6435 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api/write_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    37683 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/api_client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.797773 kdp-api-python-client-4.8.0/kdp_api/apis/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1436 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/apis/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16532 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/configuration.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5101 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/exceptions.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.821773 kdp-api-python-client-4.8.0/kdp_api/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      348 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/model/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11881 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/abac_label_parser_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11796 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/abac_label_parsers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11669 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/abac_label_parsers_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11755 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/api_error.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14435 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13785 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11583 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11832 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13982 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11503 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application_required_dataset_access.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14321 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/application_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11436 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/applications_required_dataset_access.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12028 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12288 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11443 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11716 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11913 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11320 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11611 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11735 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11551 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11812 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11672 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11903 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/attribute_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12308 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/authentication.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12080 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/authentication_details.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11936 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/authentication_details_authentication.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12004 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/authentication_details_authentication_payload.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14715 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/authentication_details_user.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11631 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/authentication_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12725 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/data_source_params.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13923 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12690 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11617 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_current_user_permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11519 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11792 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12536 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12129 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11762 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11684 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11893 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11621 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11930 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12581 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/dataset_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13617 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/error_code.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12341 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11983 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11487 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12496 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_membership.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11671 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_membership_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11652 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_membership_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11873 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_membership_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11560 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_membership_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11839 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_membership_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11772 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11661 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11983 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/group_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11576 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/index.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11491 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/index_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11772 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/index_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11682 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/ingest_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13864 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/job.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11455 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/job_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11752 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/job_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10857 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/kdp_api/model/json_record.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12743 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/lucene_query_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12846 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/query.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12760 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/query_datasets_summary.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11693 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/query_datasets_summary_datasets.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12805 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/query_datasets_summary_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13223 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/read_range_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12489 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/record_batch.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12020 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/reindex_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13643 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/segment.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11519 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/segment_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11792 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/segment_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12370 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/sequence_read_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11719 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/source_types.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11584 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/source_types_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11525 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/split_points.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12008 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/stripe_latest_charge.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12309 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/stripe_latest_charge1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13103 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/transfer_resource_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11785 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/transfer_resource_request_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13068 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/user.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12784 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/user_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11471 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/user_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11762 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/user_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12805 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/user_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13182 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/user_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11973 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11945 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11551 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11812 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11900 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13735 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_subscription.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11695 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_subscription_subscription_item_ids.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11945 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspace_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13451 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspaces_subscription.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11698 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/workspaces_subscription_subscription_item_ids.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11692 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/kdp_api/model/write_batch_response.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    82108 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/model_utils.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.825774 kdp-api-python-client-4.8.0/kdp_api/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7195 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14218 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/kdp_api/rest.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.825774 kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      401 2022-10-25 22:26:08.000000 kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8986 2022-10-25 22:26:08.000000 kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-25 22:26:08.000000 kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2022-10-25 22:26:08.000000 kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2022-10-25 22:26:08.000000 kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/top_level.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       69 2022-10-25 22:26:08.853774 kdp-api-python-client-4.8.0/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1137 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/setup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-25 22:26:08.849774 kdp-api-python-client-4.8.0/test/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      979 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_abac_label_parser_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      794 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_abac_label_parsers.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1004 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_abac_label_parsers_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      934 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_abac_label_parsers_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      737 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_api_error.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      933 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1030 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      875 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      927 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1023 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      907 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application_required_dataset_access.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1030 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_application_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1646 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_applications_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      914 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_applications_required_dataset_access.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      956 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignment.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      907 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignment_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      965 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignment_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1017 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignment_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      900 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignment_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      907 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignment_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1831 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_attribute_assignments_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      836 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      905 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      829 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      836 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_attribute_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1597 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_attributes_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      778 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_authentication.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      967 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_authentication_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1162 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_authentication_details.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1143 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_authentication_details_authentication.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_authentication_details_authentication_payload.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      857 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_authentication_details_user.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      908 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_authentication_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      794 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_data_source_params.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      893 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      822 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      886 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_current_user_permissions.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      831 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      883 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      815 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      800 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      893 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_permission_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      943 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_permission_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      995 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_permission_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      886 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_permission_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      893 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_permission_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1790 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_dataset_permissions_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      822 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_dataset_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1545 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_datasets_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      744 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_error_code.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      715 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      809 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      912 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_membership.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      879 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_membership_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      921 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_membership_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      973 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_membership_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      872 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_membership_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      879 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_membership_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1775 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_group_memberships_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      801 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_group_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1543 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_groups_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      715 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_index.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      809 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_index_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_index_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1515 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_indexes_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      720 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_ingest_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      926 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_ingest_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      701 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_job.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      787 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_job_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      839 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_job_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1308 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_jobs_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      751 2022-10-25 22:26:01.000000 kdp-api-python-client-4.8.0/test/test_json_record.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_lucene_query_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      715 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_query.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1035 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_query_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      982 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_query_datasets_summary.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      879 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_query_datasets_summary_datasets.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      872 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_query_datasets_summary_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1028 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_read_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      794 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_read_range_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      844 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_record_batch.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      844 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_reindex_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      729 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_segment.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      831 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_segment_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      883 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_segment_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      902 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_segments_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      815 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_sequence_read_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      758 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_source_types.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      940 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_source_types_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      877 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_source_types_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      758 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_split_points.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_stripe_latest_charge.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      815 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_stripe_latest_charge1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      843 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_transfer_resource_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1011 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_transfer_resource_request_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      831 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_user.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      801 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_user_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      798 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_user_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_user_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      913 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_user_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      801 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_user_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1502 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_users_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      873 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      970 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_create_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_list.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      905 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_paginator.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      963 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_patch_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1037 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_subscription.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      964 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_subscription_subscription_item_ids.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      970 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspace_update_request.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1425 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_workspaces_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1048 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspaces_subscription.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      971 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_workspaces_subscription_subscription_item_ids.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      712 2022-10-25 22:26:03.000000 kdp-api-python-client-4.8.0/test/test_write_api.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-25 22:26:02.000000 kdp-api-python-client-4.8.0/test/test_write_batch_response.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.298091 kdp-api-python-client-4.9.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      401 2022-10-26 03:13:21.298091 kdp-api-python-client-4.9.0/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    21319 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.246090 kdp-api-python-client-4.9.0/kdp_api/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      723 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.250090 kdp-api-python-client-4.9.0/kdp_api/api/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      220 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11229 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/abac_label_parsers_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31024 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/applications_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    32871 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/attribute_assignments_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30817 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/attributes_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10593 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api/authentication_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31701 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/dataset_permissions_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30607 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/datasets_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31532 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/group_memberships_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30447 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/groups_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30382 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/indexes_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6219 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api/ingest_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    25662 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/jobs_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16466 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api/query_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16010 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api/read_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11851 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/segments_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10958 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/source_types_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    30324 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/users_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26228 2022-10-26 03:13:16.000000 kdp-api-python-client-4.9.0/kdp_api/api/workspaces_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6435 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api/write_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    37683 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/api_client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.250090 kdp-api-python-client-4.9.0/kdp_api/apis/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1436 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/apis/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16532 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/configuration.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5101 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/exceptions.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.270091 kdp-api-python-client-4.9.0/kdp_api/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      348 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/model/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11881 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/abac_label_parser_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11796 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/abac_label_parsers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11669 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/abac_label_parsers_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11755 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/api_error.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14435 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13785 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11583 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11832 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13982 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11503 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application_required_dataset_access.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14321 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/application_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11436 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/applications_required_dataset_access.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12028 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12288 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11443 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11716 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11913 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11320 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11611 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11735 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11551 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11812 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11672 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11903 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/attribute_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12308 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/authentication.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12080 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/authentication_details.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11936 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/authentication_details_authentication.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12004 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/authentication_details_authentication_payload.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14715 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/authentication_details_user.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11631 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/authentication_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12725 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/data_source_params.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13923 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12690 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11617 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_current_user_permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11519 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11792 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12536 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12129 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11762 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11684 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11893 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11621 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11930 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12581 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/dataset_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13617 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/error_code.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12341 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11983 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11487 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12496 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_membership.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11671 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_membership_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11652 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_membership_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11873 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_membership_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11560 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_membership_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11839 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_membership_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11772 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11661 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11983 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/group_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11576 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/index.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11491 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/index_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11772 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/index_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11682 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/ingest_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13864 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/job.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11455 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/job_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11752 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/job_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10857 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/json_record.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12743 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/lucene_query_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12846 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/query.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12760 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/query_datasets_summary.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11693 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/query_datasets_summary_datasets.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12805 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/query_datasets_summary_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13223 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/read_range_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12489 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/record_batch.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12020 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/reindex_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13643 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/segment.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11519 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/segment_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11792 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/segment_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12370 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/sequence_read_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11719 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/source_types.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11584 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/source_types_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11525 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/split_points.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12008 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/stripe_latest_charge.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12309 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/stripe_latest_charge1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13103 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/transfer_resource_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11785 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/transfer_resource_request_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13068 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/user.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12784 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/user_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11471 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/user_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11762 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/user_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    12805 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/user_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13182 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/user_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11973 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11945 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11551 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11812 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11900 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13735 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_subscription.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11695 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_subscription_subscription_item_ids.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11945 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspace_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13451 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspaces_subscription.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11698 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/model/workspaces_subscription_subscription_item_ids.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11692 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/model/write_batch_response.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    82108 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/model_utils.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.270091 kdp-api-python-client-4.9.0/kdp_api/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7195 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    14218 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/kdp_api/rest.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.274091 kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      401 2022-10-26 03:13:21.000000 kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8986 2022-10-26 03:13:21.000000 kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-10-26 03:13:21.000000 kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2022-10-26 03:13:21.000000 kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        8 2022-10-26 03:13:21.000000 kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/top_level.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       69 2022-10-26 03:13:21.298091 kdp-api-python-client-4.9.0/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1137 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-26 03:13:21.298091 kdp-api-python-client-4.9.0/test/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      979 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_abac_label_parser_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      794 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_abac_label_parsers.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1004 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_abac_label_parsers_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      934 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_abac_label_parsers_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      737 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_api_error.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      933 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1030 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      875 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      927 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1023 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      907 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application_required_dataset_access.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1030 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_application_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1646 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_applications_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      914 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_applications_required_dataset_access.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      743 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_attribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      956 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignment.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      907 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignment_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      965 2022-10-26 03:13:13.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignment_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1017 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignment_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      900 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignment_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      907 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignment_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1831 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_attribute_assignments_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      836 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      905 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      829 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      836 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_attribute_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1597 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_attributes_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      778 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_authentication.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      967 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_authentication_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1162 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_authentication_details.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1143 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_authentication_details_authentication.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_authentication_details_authentication_payload.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      857 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_authentication_details_user.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      908 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_authentication_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      794 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_data_source_params.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      893 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      822 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      886 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_current_user_permissions.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      831 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      883 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      815 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      800 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      893 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_permission_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      943 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_permission_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      995 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_permission_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      886 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_permission_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      893 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_permission_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1790 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_dataset_permissions_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      822 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_dataset_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1545 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_datasets_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      744 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_error_code.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      715 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      809 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      912 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_membership.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      879 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_membership_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      921 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_membership_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      973 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_membership_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      872 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_membership_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      879 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_membership_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1775 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_group_memberships_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      801 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_group_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1543 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_groups_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      715 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_index.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      809 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_index_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_index_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1515 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_indexes_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      720 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_ingest_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      926 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_ingest_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      701 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_job.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      787 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_job_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      839 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_job_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1308 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_jobs_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      751 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_json_record.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_lucene_query_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      715 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_query.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1035 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_query_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      982 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_query_datasets_summary.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      879 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_query_datasets_summary_datasets.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      872 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_query_datasets_summary_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1028 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_read_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      794 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_read_range_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      844 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_record_batch.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      844 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_reindex_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      729 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_segment.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      831 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_segment_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      883 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_segment_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      902 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_segments_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      815 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_sequence_read_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      758 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_source_types.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      940 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_source_types_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      877 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_source_types_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      758 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_split_points.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_stripe_latest_charge.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      815 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_stripe_latest_charge1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      843 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_transfer_resource_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1011 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_transfer_resource_request_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      831 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_user.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      801 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_user_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      798 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_user_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_user_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      913 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_user_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      801 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_user_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1502 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_users_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      873 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      970 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_create_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_list.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      905 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_paginator.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      963 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_patch_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1037 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_subscription.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      964 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_subscription_subscription_item_ids.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      970 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspace_update_request.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1425 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_workspaces_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1048 2022-10-26 03:13:14.000000 kdp-api-python-client-4.9.0/test/test_workspaces_subscription.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      971 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_workspaces_subscription_subscription_item_ids.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      712 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_write_api.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      808 2022-10-26 03:13:15.000000 kdp-api-python-client-4.9.0/test/test_write_batch_response.py
```

### Comparing `kdp-api-python-client-4.8.0/README.md` & `kdp-api-python-client-4.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # kdp-api-python-client
 The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 4.8.0
-- Package version: 4.8.0
+- API version: 4.9.0
+- Package version: 4.9.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/__init__.py` & `kdp-api-python-client-4.9.0/kdp_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "4.8.0"
+__version__ = "4.9.0"
 
 # import ApiClient
 from kdp_api.api_client import ApiClient
 
 # import Configuration
 from kdp_api.configuration import Configuration
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/abac_label_parsers_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/abac_label_parsers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/applications_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/applications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/attribute_assignments_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/attribute_assignments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/attributes_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/attributes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/authentication_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/dataset_permissions_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/dataset_permissions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/datasets_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/datasets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/group_memberships_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/group_memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/groups_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/indexes_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/indexes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/ingest_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/ingest_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/jobs_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/query_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/query_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/read_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/read_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/segments_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/segments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/source_types_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/source_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/users_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/workspaces_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/workspaces_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api/write_api.py` & `kdp-api-python-client-4.9.0/kdp_api/api/write_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/api_client.py` & `kdp-api-python-client-4.9.0/kdp_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/4.8.0/python'
+        self.user_agent = 'OpenAPI-Generator/4.9.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/apis/__init__.py` & `kdp-api-python-client-4.9.0/kdp_api/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `kdp-api-python-client-4.8.0/kdp_api/configuration.py` & `kdp-api-python-client-4.9.0/kdp_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -384,16 +384,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.8.0\n"\
-               "SDK Package Version: 4.8.0".\
+               "Version of the API: 4.9.0\n"\
+               "SDK Package Version: 4.9.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/exceptions.py` & `kdp-api-python-client-4.9.0/kdp_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/abac_label_parser_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/abac_label_parser_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/abac_label_parsers.py` & `kdp-api-python-client-4.9.0/kdp_api/model/abac_label_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/abac_label_parsers_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/abac_label_parsers_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/api_error.py` & `kdp-api-python-client-4.9.0/kdp_api/model/api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application_required_dataset_access.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application_required_dataset_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/application_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/application_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/applications_required_dataset_access.py` & `kdp-api-python-client-4.9.0/kdp_api/model/applications_required_dataset_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_assignment_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_assignment_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/attribute_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/attribute_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/authentication.py` & `kdp-api-python-client-4.9.0/kdp_api/model/authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/authentication_details.py` & `kdp-api-python-client-4.9.0/kdp_api/model/authentication_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/authentication_details_authentication.py` & `kdp-api-python-client-4.9.0/kdp_api/model/authentication_details_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/authentication_details_authentication_payload.py` & `kdp-api-python-client-4.9.0/kdp_api/model/authentication_details_authentication_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/authentication_details_user.py` & `kdp-api-python-client-4.9.0/kdp_api/model/authentication_details_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/authentication_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/authentication_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/data_source_params.py` & `kdp-api-python-client-4.9.0/kdp_api/model/data_source_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_current_user_permissions.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_current_user_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_permission_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_permission_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/dataset_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/dataset_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/error_code.py` & `kdp-api-python-client-4.9.0/kdp_api/model/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_membership.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_membership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_membership_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_membership_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_membership_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_membership_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_membership_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_membership_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_membership_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_membership_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_membership_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_membership_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/group_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/group_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/index.py` & `kdp-api-python-client-4.9.0/kdp_api/model/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/index_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/index_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/index_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/index_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/ingest_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/ingest_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/job.py` & `kdp-api-python-client-4.9.0/kdp_api/model/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/job_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/job_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/job_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/job_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/json_record.py` & `kdp-api-python-client-4.9.0/kdp_api/model/json_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/lucene_query_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/lucene_query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/query.py` & `kdp-api-python-client-4.9.0/kdp_api/model/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/query_datasets_summary.py` & `kdp-api-python-client-4.9.0/kdp_api/model/query_datasets_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/query_datasets_summary_datasets.py` & `kdp-api-python-client-4.9.0/kdp_api/model/query_datasets_summary_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/query_datasets_summary_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/query_datasets_summary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/read_range_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/read_range_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/record_batch.py` & `kdp-api-python-client-4.9.0/kdp_api/model/record_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/reindex_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/reindex_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/segment.py` & `kdp-api-python-client-4.9.0/kdp_api/model/segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/segment_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/segment_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/segment_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/segment_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/sequence_read_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/sequence_read_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/source_types.py` & `kdp-api-python-client-4.9.0/kdp_api/model/source_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/source_types_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/source_types_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/split_points.py` & `kdp-api-python-client-4.9.0/kdp_api/model/split_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/stripe_latest_charge.py` & `kdp-api-python-client-4.9.0/kdp_api/model/stripe_latest_charge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/stripe_latest_charge1.py` & `kdp-api-python-client-4.9.0/kdp_api/model/stripe_latest_charge1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/transfer_resource_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/transfer_resource_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/transfer_resource_request_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/transfer_resource_request_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/user.py` & `kdp-api-python-client-4.9.0/kdp_api/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/user_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/user_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/user_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/user_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/user_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/user_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/user_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/user_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/user_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/user_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_create_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_list.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_paginator.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_patch_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_subscription.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_subscription_subscription_item_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspace_update_request.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspace_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspaces_subscription.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspaces_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/workspaces_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.9.0/kdp_api/model/workspaces_subscription_subscription_item_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model/write_batch_response.py` & `kdp-api-python-client-4.9.0/kdp_api/model/write_batch_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/model_utils.py` & `kdp-api-python-client-4.9.0/kdp_api/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api/models/__init__.py` & `kdp-api-python-client-4.9.0/kdp_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kdp-api-python-client-4.8.0/kdp_api/rest.py` & `kdp-api-python-client-4.9.0/kdp_api/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `kdp-api-python-client-4.8.0/kdp_api_python_client.egg-info/SOURCES.txt` & `kdp-api-python-client-4.9.0/kdp_api_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kdp-api-python-client-4.8.0/setup.py` & `kdp-api-python-client-4.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kdp-api-python-client"
-VERSION = "4.8.0"
+VERSION = "4.9.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kdp-api-python-client-4.8.0/test/test_abac_label_parser_paginator.py` & `kdp-api-python-client-4.9.0/test/test_abac_label_parser_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_abac_label_parsers.py` & `kdp-api-python-client-4.9.0/test/test_abac_label_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_abac_label_parsers_api.py` & `kdp-api-python-client-4.9.0/test/test_abac_label_parsers_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_abac_label_parsers_list.py` & `kdp-api-python-client-4.9.0/test/test_abac_label_parsers_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_api_error.py` & `kdp-api-python-client-4.9.0/test/test_api_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application.py` & `kdp-api-python-client-4.9.0/test/test_application.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application_create_request.py` & `kdp-api-python-client-4.9.0/test/test_application_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application_list.py` & `kdp-api-python-client-4.9.0/test/test_application_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application_paginator.py` & `kdp-api-python-client-4.9.0/test/test_application_paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_application_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application_required_dataset_access.py` & `kdp-api-python-client-4.9.0/test/test_application_required_dataset_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_application_update_request.py` & `kdp-api-python-client-4.9.0/test/test_application_update_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_applications_api.py` & `kdp-api-python-client-4.9.0/test/test_applications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_applications_required_dataset_access.py` & `kdp-api-python-client-4.9.0/test/test_applications_required_dataset_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute.py` & `kdp-api-python-client-4.9.0/test/test_attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignment.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignment_create_request.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignment_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignment_list.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignment_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignment_paginator.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignment_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignment_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignment_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignment_update_request.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignment_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_assignments_api.py` & `kdp-api-python-client-4.9.0/test/test_attribute_assignments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_create_request.py` & `kdp-api-python-client-4.9.0/test/test_attribute_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_list.py` & `kdp-api-python-client-4.9.0/test/test_attribute_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_paginator.py` & `kdp-api-python-client-4.9.0/test/test_attribute_paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_attribute_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attribute_update_request.py` & `kdp-api-python-client-4.9.0/test/test_attribute_update_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_attributes_api.py` & `kdp-api-python-client-4.9.0/test/test_attributes_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication.py` & `kdp-api-python-client-4.9.0/test/test_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication_api.py` & `kdp-api-python-client-4.9.0/test/test_authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication_details.py` & `kdp-api-python-client-4.9.0/test/test_authentication_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication_details_authentication.py` & `kdp-api-python-client-4.9.0/test/test_authentication_details_authentication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication_details_authentication_payload.py` & `kdp-api-python-client-4.9.0/test/test_authentication_details_authentication_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication_details_user.py` & `kdp-api-python-client-4.9.0/test/test_authentication_details_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_authentication_list.py` & `kdp-api-python-client-4.9.0/test/test_authentication_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_data_source_params.py` & `kdp-api-python-client-4.9.0/test/test_data_source_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset.py` & `kdp-api-python-client-4.9.0/test/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_create_request.py` & `kdp-api-python-client-4.9.0/test/test_dataset_create_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_current_user_permissions.py` & `kdp-api-python-client-4.9.0/test/test_dataset_current_user_permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_list.py` & `kdp-api-python-client-4.9.0/test/test_job_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.dataset import Dataset
-globals()['Dataset'] = Dataset
-from kdp_api.model.dataset_list import DatasetList
+from kdp_api.model.job import Job
+globals()['Job'] = Job
+from kdp_api.model.job_list import JobList
 
 
-class TestDatasetList(unittest.TestCase):
-    """DatasetList unit test stubs"""
+class TestJobList(unittest.TestCase):
+    """JobList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetList(self):
-        """Test DatasetList"""
+    def testJobList(self):
+        """Test JobList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetList()  # noqa: E501
+        # model = JobList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_paginator.py` & `kdp-api-python-client-4.9.0/test/test_dataset_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_dataset_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permission.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permission_create_request.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permission_create_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permission_list.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permission_paginator.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permission_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permission_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permission_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permission_update_request.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permission_update_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_permissions_api.py` & `kdp-api-python-client-4.9.0/test/test_dataset_permissions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_dataset_update_request.py` & `kdp-api-python-client-4.9.0/test/test_dataset_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_datasets_api.py` & `kdp-api-python-client-4.9.0/test/test_datasets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_error_code.py` & `kdp-api-python-client-4.9.0/test/test_error_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group.py` & `kdp-api-python-client-4.9.0/test/test_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_create_request.py` & `kdp-api-python-client-4.9.0/test/test_group_create_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_list.py` & `kdp-api-python-client-4.9.0/test/test_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_membership.py` & `kdp-api-python-client-4.9.0/test/test_group_membership.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_membership_create_request.py` & `kdp-api-python-client-4.9.0/test/test_group_membership_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_membership_list.py` & `kdp-api-python-client-4.9.0/test/test_group_membership_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_membership_paginator.py` & `kdp-api-python-client-4.9.0/test/test_group_membership_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_membership_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_group_membership_patch_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_membership_update_request.py` & `kdp-api-python-client-4.9.0/test/test_group_membership_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_memberships_api.py` & `kdp-api-python-client-4.9.0/test/test_group_memberships_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_paginator.py` & `kdp-api-python-client-4.9.0/test/test_group_paginator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_group_patch_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_group_update_request.py` & `kdp-api-python-client-4.9.0/test/test_group_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_groups_api.py` & `kdp-api-python-client-4.9.0/test/test_groups_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_index.py` & `kdp-api-python-client-4.9.0/test/test_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.index import Index
+from kdp_api.model.job import Job
 
 
-class TestIndex(unittest.TestCase):
-    """Index unit test stubs"""
+class TestJob(unittest.TestCase):
+    """Job unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIndex(self):
-        """Test Index"""
+    def testJob(self):
+        """Test Job"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Index()  # noqa: E501
+        # model = Job()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_index_list.py` & `kdp-api-python-client-4.9.0/test/test_index_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_index_paginator.py` & `kdp-api-python-client-4.9.0/test/test_index_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_indexes_api.py` & `kdp-api-python-client-4.9.0/test/test_indexes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_ingest_api.py` & `kdp-api-python-client-4.9.0/test/test_ingest_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_ingest_create_request.py` & `kdp-api-python-client-4.9.0/test/test_sequence_read_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.data_source_params import DataSourceParams
-globals()['DataSourceParams'] = DataSourceParams
-from kdp_api.model.ingest_create_request import IngestCreateRequest
+from kdp_api.model.sequence_read_request import SequenceReadRequest
 
 
-class TestIngestCreateRequest(unittest.TestCase):
-    """IngestCreateRequest unit test stubs"""
+class TestSequenceReadRequest(unittest.TestCase):
+    """SequenceReadRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIngestCreateRequest(self):
-        """Test IngestCreateRequest"""
+    def testSequenceReadRequest(self):
+        """Test SequenceReadRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IngestCreateRequest()  # noqa: E501
+        # model = SequenceReadRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_job.py` & `kdp-api-python-client-4.9.0/test/test_segment.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.job import Job
+from kdp_api.model.segment import Segment
 
 
-class TestJob(unittest.TestCase):
-    """Job unit test stubs"""
+class TestSegment(unittest.TestCase):
+    """Segment unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testJob(self):
-        """Test Job"""
+    def testSegment(self):
+        """Test Segment"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Job()  # noqa: E501
+        # model = Segment()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_job_list.py` & `kdp-api-python-client-4.9.0/test/test_split_points.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.job import Job
-globals()['Job'] = Job
-from kdp_api.model.job_list import JobList
+from kdp_api.model.split_points import SplitPoints
 
 
-class TestJobList(unittest.TestCase):
-    """JobList unit test stubs"""
+class TestSplitPoints(unittest.TestCase):
+    """SplitPoints unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testJobList(self):
-        """Test JobList"""
+    def testSplitPoints(self):
+        """Test SplitPoints"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = JobList()  # noqa: E501
+        # model = SplitPoints()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_job_paginator.py` & `kdp-api-python-client-4.9.0/test/test_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.job_list import JobList
-globals()['JobList'] = JobList
-from kdp_api.model.job_paginator import JobPaginator
+from kdp_api.model.stripe_latest_charge1 import StripeLatestCharge1
+globals()['StripeLatestCharge1'] = StripeLatestCharge1
+from kdp_api.model.user import User
 
 
-class TestJobPaginator(unittest.TestCase):
-    """JobPaginator unit test stubs"""
+class TestUser(unittest.TestCase):
+    """User unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testJobPaginator(self):
-        """Test JobPaginator"""
+    def testUser(self):
+        """Test User"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = JobPaginator()  # noqa: E501
+        # model = User()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_jobs_api.py` & `kdp-api-python-client-4.9.0/test/test_jobs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_json_record.py` & `kdp-api-python-client-4.9.0/test/test_json_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_lucene_query_request.py` & `kdp-api-python-client-4.9.0/test/test_lucene_query_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_query.py` & `kdp-api-python-client-4.9.0/test/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_query_api.py` & `kdp-api-python-client-4.9.0/test/test_query_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_query_datasets_summary.py` & `kdp-api-python-client-4.9.0/test/test_query_datasets_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_query_datasets_summary_datasets.py` & `kdp-api-python-client-4.9.0/test/test_query_datasets_summary_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_query_datasets_summary_request.py` & `kdp-api-python-client-4.9.0/test/test_query_datasets_summary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_read_api.py` & `kdp-api-python-client-4.9.0/test/test_read_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_read_range_request.py` & `kdp-api-python-client-4.9.0/test/test_read_range_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_record_batch.py` & `kdp-api-python-client-4.9.0/test/test_record_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_reindex_request.py` & `kdp-api-python-client-4.9.0/test/test_reindex_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_segment.py` & `kdp-api-python-client-4.9.0/test/test_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.segment import Segment
+from kdp_api.model.index import Index
 
 
-class TestSegment(unittest.TestCase):
-    """Segment unit test stubs"""
+class TestIndex(unittest.TestCase):
+    """Index unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSegment(self):
-        """Test Segment"""
+    def testIndex(self):
+        """Test Index"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Segment()  # noqa: E501
+        # model = Index()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_segment_list.py` & `kdp-api-python-client-4.9.0/test/test_segment_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_segment_paginator.py` & `kdp-api-python-client-4.9.0/test/test_segment_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_segments_api.py` & `kdp-api-python-client-4.9.0/test/test_segments_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_sequence_read_request.py` & `kdp-api-python-client-4.9.0/test/test_source_types_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.sequence_read_request import SequenceReadRequest
+from kdp_api.api.source_types_api import SourceTypesApi  # noqa: E501
 
 
-class TestSequenceReadRequest(unittest.TestCase):
-    """SequenceReadRequest unit test stubs"""
+class TestSourceTypesApi(unittest.TestCase):
+    """SourceTypesApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = SourceTypesApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testSequenceReadRequest(self):
-        """Test SequenceReadRequest"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = SequenceReadRequest()  # noqa: E501
+    def test_get_source_types(self):
+        """Test case for get_source_types
+
+        Retrieves list of Source Types  # noqa: E501
+        """
+        pass
+
+    def test_get_source_types_id(self):
+        """Test case for get_source_types_id
+
+        Retrieves Source Type with the given ID  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_source_types.py` & `kdp-api-python-client-4.9.0/test/test_source_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_source_types_api.py` & `kdp-api-python-client-4.9.0/test/test_write_batch_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
+import sys
 import unittest
 
 import kdp_api
-from kdp_api.api.source_types_api import SourceTypesApi  # noqa: E501
+from kdp_api.model.write_batch_response import WriteBatchResponse
 
 
-class TestSourceTypesApi(unittest.TestCase):
-    """SourceTypesApi unit test stubs"""
+class TestWriteBatchResponse(unittest.TestCase):
+    """WriteBatchResponse unit test stubs"""
 
     def setUp(self):
-        self.api = SourceTypesApi()  # noqa: E501
-
-    def tearDown(self):
         pass
 
-    def test_get_source_types(self):
-        """Test case for get_source_types
-
-        Retrieves list of Source Types  # noqa: E501
-        """
+    def tearDown(self):
         pass
 
-    def test_get_source_types_id(self):
-        """Test case for get_source_types_id
-
-        Retrieves Source Type with the given ID  # noqa: E501
-        """
+    def testWriteBatchResponse(self):
+        """Test WriteBatchResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = WriteBatchResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_source_types_list.py` & `kdp-api-python-client-4.9.0/test/test_source_types_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_split_points.py` & `kdp-api-python-client-4.9.0/test/test_stripe_latest_charge1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.split_points import SplitPoints
+from kdp_api.model.stripe_latest_charge1 import StripeLatestCharge1
 
 
-class TestSplitPoints(unittest.TestCase):
-    """SplitPoints unit test stubs"""
+class TestStripeLatestCharge1(unittest.TestCase):
+    """StripeLatestCharge1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSplitPoints(self):
-        """Test SplitPoints"""
+    def testStripeLatestCharge1(self):
+        """Test StripeLatestCharge1"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SplitPoints()  # noqa: E501
+        # model = StripeLatestCharge1()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_stripe_latest_charge.py` & `kdp-api-python-client-4.9.0/test/test_stripe_latest_charge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_stripe_latest_charge1.py` & `kdp-api-python-client-4.9.0/test/test_user_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.stripe_latest_charge1 import StripeLatestCharge1
+from kdp_api.model.user import User
+globals()['User'] = User
+from kdp_api.model.user_list import UserList
 
 
-class TestStripeLatestCharge1(unittest.TestCase):
-    """StripeLatestCharge1 unit test stubs"""
+class TestUserList(unittest.TestCase):
+    """UserList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStripeLatestCharge1(self):
-        """Test StripeLatestCharge1"""
+    def testUserList(self):
+        """Test UserList"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = StripeLatestCharge1()  # noqa: E501
+        # model = UserList()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_transfer_resource_request.py` & `kdp-api-python-client-4.9.0/test/test_transfer_resource_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_transfer_resource_request_list.py` & `kdp-api-python-client-4.9.0/test/test_transfer_resource_request_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_user.py` & `kdp-api-python-client-4.9.0/test/test_user_patch_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.stripe_latest_charge1 import StripeLatestCharge1
-globals()['StripeLatestCharge1'] = StripeLatestCharge1
-from kdp_api.model.user import User
+from kdp_api.model.stripe_latest_charge import StripeLatestCharge
+globals()['StripeLatestCharge'] = StripeLatestCharge
+from kdp_api.model.user_patch_request import UserPatchRequest
 
 
-class TestUser(unittest.TestCase):
-    """User unit test stubs"""
+class TestUserPatchRequest(unittest.TestCase):
+    """UserPatchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUser(self):
-        """Test User"""
+    def testUserPatchRequest(self):
+        """Test UserPatchRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = User()  # noqa: E501
+        # model = UserPatchRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_user_create_request.py` & `kdp-api-python-client-4.9.0/test/test_user_create_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_user_list.py` & `kdp-api-python-client-4.9.0/test/test_write_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.user import User
-globals()['User'] = User
-from kdp_api.model.user_list import UserList
+from kdp_api.api.write_api import WriteApi  # noqa: E501
 
 
-class TestUserList(unittest.TestCase):
-    """UserList unit test stubs"""
+class TestWriteApi(unittest.TestCase):
+    """WriteApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = WriteApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testUserList(self):
-        """Test UserList"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = UserList()  # noqa: E501
+    def test_post_write_id(self):
+        """Test case for post_write_id
+
+        Write records  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_user_paginator.py` & `kdp-api-python-client-4.9.0/test/test_user_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_user_patch_request.py` & `kdp-api-python-client-4.9.0/test/test_user_update_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.stripe_latest_charge import StripeLatestCharge
-globals()['StripeLatestCharge'] = StripeLatestCharge
-from kdp_api.model.user_patch_request import UserPatchRequest
+from kdp_api.model.user_update_request import UserUpdateRequest
 
 
-class TestUserPatchRequest(unittest.TestCase):
-    """UserPatchRequest unit test stubs"""
+class TestUserUpdateRequest(unittest.TestCase):
+    """UserUpdateRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserPatchRequest(self):
-        """Test UserPatchRequest"""
+    def testUserUpdateRequest(self):
+        """Test UserUpdateRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UserPatchRequest()  # noqa: E501
+        # model = UserUpdateRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_user_update_request.py` & `kdp-api-python-client-4.9.0/test/test_workspace_patch_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.user_update_request import UserUpdateRequest
+from kdp_api.model.workspaces_subscription import WorkspacesSubscription
+globals()['WorkspacesSubscription'] = WorkspacesSubscription
+from kdp_api.model.workspace_patch_request import WorkspacePatchRequest
 
 
-class TestUserUpdateRequest(unittest.TestCase):
-    """UserUpdateRequest unit test stubs"""
+class TestWorkspacePatchRequest(unittest.TestCase):
+    """WorkspacePatchRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testUserUpdateRequest(self):
-        """Test UserUpdateRequest"""
+    def testWorkspacePatchRequest(self):
+        """Test WorkspacePatchRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = UserUpdateRequest()  # noqa: E501
+        # model = WorkspacePatchRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kdp-api-python-client-4.8.0/test/test_users_api.py` & `kdp-api-python-client-4.9.0/test/test_users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace.py` & `kdp-api-python-client-4.9.0/test/test_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace_create_request.py` & `kdp-api-python-client-4.9.0/test/test_workspace_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace_list.py` & `kdp-api-python-client-4.9.0/test/test_workspace_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace_paginator.py` & `kdp-api-python-client-4.9.0/test/test_workspace_paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace_subscription.py` & `kdp-api-python-client-4.9.0/test/test_workspace_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.9.0/test/test_workspace_subscription_subscription_item_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspace_update_request.py` & `kdp-api-python-client-4.9.0/test/test_workspace_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspaces_api.py` & `kdp-api-python-client-4.9.0/test/test_workspaces_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import kdp_api
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspaces_subscription.py` & `kdp-api-python-client-4.9.0/test/test_workspaces_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_workspaces_subscription_subscription_item_ids.py` & `kdp-api-python-client-4.9.0/test/test_workspaces_subscription_subscription_item_ids.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `kdp-api-python-client-4.8.0/test/test_write_batch_response.py` & `kdp-api-python-client-4.9.0/test/test_job_paginator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     Koverse Data Platform (KDP) API
 
     The KDP API is a REST API that can be used to create, access, and update data in KDP Workspaces  # noqa: E501
 
-    The version of the OpenAPI document: 4.8.0
+    The version of the OpenAPI document: 4.9.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import kdp_api
-from kdp_api.model.write_batch_response import WriteBatchResponse
+from kdp_api.model.job_list import JobList
+globals()['JobList'] = JobList
+from kdp_api.model.job_paginator import JobPaginator
 
 
-class TestWriteBatchResponse(unittest.TestCase):
-    """WriteBatchResponse unit test stubs"""
+class TestJobPaginator(unittest.TestCase):
+    """JobPaginator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testWriteBatchResponse(self):
-        """Test WriteBatchResponse"""
+    def testJobPaginator(self):
+        """Test JobPaginator"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = WriteBatchResponse()  # noqa: E501
+        # model = JobPaginator()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

