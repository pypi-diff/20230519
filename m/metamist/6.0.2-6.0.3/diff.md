# Comparing `tmp/metamist-6.0.2.tar.gz` & `tmp/metamist-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.0.2.tar", last modified: Wed May  3 09:59:32 2023, max compression
+gzip compressed data, was "metamist-6.0.3.tar", last modified: Fri May 19 02:37:25 2023, max compression
```

## Comparing `metamist-6.0.2.tar` & `metamist-6.0.3.tar`

### file list

```diff
@@ -1,105 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.287104 metamist-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-03 09:53:22.000000 metamist-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 09:53:22.000000 metamist-6.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-03 09:59:32.287104 metamist-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-03 09:53:22.000000 metamist-6.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.247102 metamist-6.0.2/metamist/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.255103 metamist-6.0.2/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33327 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41921 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53135 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18099 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.255103 metamist-6.0.2/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.255103 metamist-6.0.2/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-03 09:56:31.000000 metamist-6.0.2/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.263103 metamist-6.0.2/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_family.py
--rw-r--r--   0 runner    (1001) docker     (123)    13126 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/project_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-05-03 09:56:23.000000 metamist-6.0.2/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12993 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.263103 metamist-6.0.2/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.267103 metamist-6.0.2/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31001 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50478 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-03 09:53:22.000000 metamist-6.0.2/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-03 09:56:24.000000 metamist-6.0.2/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.251103 metamist-6.0.2/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 09:59:32.000000 metamist-6.0.2/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-03 09:53:22.000000 metamist-6.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 09:59:32.287104 metamist-6.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-03 09:53:22.000000 metamist-6.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 09:59:32.287104 metamist-6.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10907 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-03 09:53:22.000000 metamist-6.0.2/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-03 09:53:22.000000 metamist-6.0.2/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.122965 metamist-6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-19 02:31:41.000000 metamist-6.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 02:31:41.000000 metamist-6.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-19 02:37:25.118965 metamist-6.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-05-19 02:31:41.000000 metamist-6.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.058964 metamist-6.0.3/metamist/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.070964 metamist-6.0.3/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41903 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.070964 metamist-6.0.3/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17054 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.074964 metamist-6.0.3/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-19 02:34:36.000000 metamist-6.0.3/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.094965 metamist-6.0.3/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_assays_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-05-19 02:34:31.000000 metamist-6.0.3/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.094965 metamist-6.0.3/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.098965 metamist-6.0.3/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50764 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-19 02:31:41.000000 metamist-6.0.3/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-05-19 02:34:32.000000 metamist-6.0.3/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.062964 metamist-6.0.3/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-19 02:37:25.000000 metamist-6.0.3/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 02:37:24.000000 metamist-6.0.3/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-19 02:31:41.000000 metamist-6.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 02:37:25.122965 metamist-6.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-19 02:31:41.000000 metamist-6.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 02:37:25.118965 metamist-6.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19216 2023-05-19 02:31:41.000000 metamist-6.0.3/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-05-19 02:31:41.000000 metamist-6.0.3/test/testbase.py
```

### Comparing `metamist-6.0.2/LICENSE` & `metamist-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/PKG-INFO` & `metamist-6.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.2
+Version: 6.0.3
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.2/README.md` & `metamist-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/metamist/__init__.py` & `metamist-6.0.3/metamist/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-6.0.2/metamist/api/analysis_api.py` & `metamist-6.0.3/metamist/api/analysis_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/api/assay_api.py` & `metamist-6.0.3/metamist/api/assay_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -322,15 +322,14 @@
                 'endpoint_path': '/api/v1/assay/criteria',
                 'operation_id': 'get_assays_by_criteria',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'active',
                     'body_get_assays_by_criteria',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
@@ -339,24 +338,20 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'active':
-                        (bool,),
                     'body_get_assays_by_criteria':
                         (BodyGetAssaysByCriteria,),
                 },
                 'attribute_map': {
-                    'active': 'active',
                 },
                 'location_map': {
-                    'active': 'query',
                     'body_get_assays_by_criteria': 'body',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
@@ -793,15 +788,14 @@
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_assays_by_criteria(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
-            active (bool): [optional] if omitted the server will use the default value of True
             body_get_assays_by_criteria (BodyGetAssaysByCriteria): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
```

### Comparing `metamist-6.0.2/metamist/api/default_api.py` & `metamist-6.0.3/metamist/api/sequencing_group_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -18,132 +18,151 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
+from metamist.model.http_validation_error import HTTPValidationError
 
 
-class DefaultApi(object):
+class SequencingGroupApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-        self.handle_http_get_graphql_get_async = async_wrap(self.handle_http_get_graphql_get)
-        self.handle_http_get_graphql_get_endpoint = _Endpoint(
+        self.get_all_sequencing_group_ids_by_sample_by_type_async = async_wrap(self.get_all_sequencing_group_ids_by_sample_by_type)
+        self.get_all_sequencing_group_ids_by_sample_by_type_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
-                'endpoint_path': '/graphql',
-                'operation_id': 'handle_http_get_graphql_get',
+                'endpoint_path': '/api/v1/sequencing-group/project/{project}',
+                'operation_id': 'get_all_sequencing_group_ids_by_sample_by_type',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'project',
+                ],
+                'required': [
+                    'project',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'project':
+                        (str,),
                 },
                 'attribute_map': {
+                    'project': 'project',
                 },
                 'location_map': {
+                    'project': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-        self.handle_http_post_graphql_post_async = async_wrap(self.handle_http_post_graphql_post)
-        self.handle_http_post_graphql_post_endpoint = _Endpoint(
+        self.get_sequencing_group_async = async_wrap(self.get_sequencing_group)
+        self.get_sequencing_group_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
-                'endpoint_path': '/graphql',
-                'operation_id': 'handle_http_post_graphql_post',
-                'http_method': 'POST',
+                'endpoint_path': '/api/v1/sequencing-group{sequencing_group_id}',
+                'operation_id': 'get_sequencing_group',
+                'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
+                    'sequencing_group_id',
+                ],
+                'required': [
+                    'sequencing_group_id',
                 ],
-                'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
+                    'sequencing_group_id':
+                        (str,),
                 },
                 'attribute_map': {
+                    'sequencing_group_id': 'sequencing_group_id',
                 },
                 'location_map': {
+                    'sequencing_group_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-    def handle_http_get_graphql_get(
+    def get_all_sequencing_group_ids_by_sample_by_type(
         self,
+        project,
         **kwargs
     ):
-        """Handle Http Get  # noqa: E501
+        """Get All Sequencing Group Ids By Sample By Type  # noqa: E501
 
+        Creates a new sample, and returns the internal sample ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.handle_http_get_graphql_get(async_req=True)
+        >>> thread = api.get_all_sequencing_group_ids_by_sample_by_type(project, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            project (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -187,28 +206,34 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.handle_http_get_graphql_get_endpoint.call_with_http_info(**kwargs)
+        kwargs['project'] = \
+            project
+        return self.get_all_sequencing_group_ids_by_sample_by_type_endpoint.call_with_http_info(**kwargs)
 
-    def handle_http_post_graphql_post(
+    def get_sequencing_group(
         self,
+        sequencing_group_id,
         **kwargs
     ):
-        """Handle Http Post  # noqa: E501
+        """Get Sequencing Group  # noqa: E501
 
+        Creates a new sample, and returns the internal sample ID  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.handle_http_post_graphql_post(async_req=True)
+        >>> thread = api.get_sequencing_group(sequencing_group_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            sequencing_group_id (str):
 
         Keyword Args:
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -252,9 +277,11 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        return self.handle_http_post_graphql_post_endpoint.call_with_http_info(**kwargs)
+        kwargs['sequencing_group_id'] = \
+            sequencing_group_id
+        return self.get_sequencing_group_endpoint.call_with_http_info(**kwargs)
```

### Comparing `metamist-6.0.2/metamist/api/enums_api.py` & `metamist-6.0.3/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/api/family_api.py` & `metamist-6.0.3/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/api/import_api.py` & `metamist-6.0.3/metamist/api/import_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/api/participant_api.py` & `metamist-6.0.3/metamist/api/participant_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -461,15 +461,15 @@
             },
             api_client=api_client
         )
 
         self.upsert_participants_async = async_wrap(self.upsert_participants)
         self.upsert_participants_endpoint = _Endpoint(
             settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/participant/{project}/upsert-many',
                 'operation_id': 'upsert_participants',
                 'http_method': 'PUT',
                 'servers': None,
@@ -1074,15 +1074,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+            bool, date, datetime, dict, float, int, list, str, none_type
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.0.2/metamist/api/project_api.py` & `metamist-6.0.3/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/api/sample_api.py` & `metamist-6.0.3/metamist/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -607,15 +607,15 @@
             },
             api_client=api_client
         )
 
         self.upsert_samples_async = async_wrap(self.upsert_samples)
         self.upsert_samples_endpoint = _Endpoint(
             settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/sample/{project}/upsert-many',
                 'operation_id': 'upsert_samples',
                 'http_method': 'PUT',
                 'servers': None,
@@ -1435,15 +1435,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+            bool, date, datetime, dict, float, int, list, str, none_type
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.0.2/metamist/api/seqr_api.py` & `metamist-6.0.3/metamist/api/seqr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/api/web_api.py` & `metamist-6.0.3/metamist/api/web_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -19,15 +19,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types,
     async_wrap
 )
 from metamist.model.http_validation_error import HTTPValidationError
-from metamist.model.project_summary_response import ProjectSummaryResponse
+from metamist.model.project_summary import ProjectSummary
 from metamist.model.search_item import SearchItem
 from metamist.model.search_response_model import SearchResponseModel
 
 
 class WebApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
@@ -39,15 +39,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
         self.get_project_summary_async = async_wrap(self.get_project_summary)
         self.get_project_summary_endpoint = _Endpoint(
             settings={
-                'response_type': (ProjectSummaryResponse,),
+                'response_type': (ProjectSummary,),
                 'auth': [
                     'HTTPBearer'
                 ],
                 'endpoint_path': '/api/v1/web/{project}/summary',
                 'operation_id': 'get_project_summary',
                 'http_method': 'POST',
                 'servers': None,
@@ -299,15 +299,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            ProjectSummaryResponse
+            ProjectSummary
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `metamist-6.0.2/metamist/api_client.py` & `metamist-6.0.3/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-6.0.2/metamist/apis/__init__.py` & `metamist-6.0.3/metamist/apis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from metamist.api.analysis_api import AnalysisApi
 from metamist.api.assay_api import AssayApi
-from metamist.api.default_api import DefaultApi
 from metamist.api.enums_api import EnumsApi
 from metamist.api.family_api import FamilyApi
 from metamist.api.import_api import ImportApi
 from metamist.api.participant_api import ParticipantApi
 from metamist.api.project_api import ProjectApi
 from metamist.api.sample_api import SampleApi
 from metamist.api.seqr_api import SeqrApi
```

### Comparing `metamist-6.0.2/metamist/configuration.py` & `metamist-6.0.3/metamist/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -401,15 +401,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.0.2\n"\
+               "Version of the API: 6.0.3\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-6.0.2/metamist/exceptions.py` & `metamist-6.0.3/metamist/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-6.0.2/metamist/graphql/__init__.py` & `metamist-6.0.3/metamist/graphql/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Dict, Any
 
 from gql import Client, gql as gql_constructor
 from gql.transport.aiohttp import AIOHTTPTransport
 from gql.transport.requests import RequestsHTTPTransport
 
 from cpg_utils.cloud import get_google_identity_token
+
 # this does not import itself, it imports the module
 from graphql import DocumentNode  # type: ignore
 
 import metamist.configuration
 
 
 _sync_client: Client | None = None
```

### Comparing `metamist-6.0.2/metamist/model/analysis.py` & `metamist-6.0.3/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/analysis_query_model.py` & `metamist-6.0.3/metamist/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/analysis_status.py` & `metamist-6.0.3/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/analysis_update_model.py` & `metamist-6.0.3/metamist/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/assay_upsert.py` & `metamist-6.0.3/metamist/model/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class AssayUpsert(ModelNormal):
+class Project(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,42 +78,44 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (int,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'external_ids': ({str: (str,)},),  # noqa: E501
-            'sample_id': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'dataset': (str,),  # noqa: E501
             'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'read_group_name': (str,),  # noqa: E501
+            'write_group_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'external_ids': 'external_ids',  # noqa: E501
-        'sample_id': 'sample_id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'dataset': 'dataset',  # noqa: E501
         'meta': 'meta',  # noqa: E501
+        'read_group_name': 'read_group_name',  # noqa: E501
+        'write_group_name': 'write_group_name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AssayUpsert - a model defined in OpenAPI
+        """Project - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -139,18 +141,19 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (int): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            external_ids ({str: (str,)}): [optional]  # noqa: E501
-            sample_id (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            dataset (str): [optional]  # noqa: E501
             meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            read_group_name (str): [optional]  # noqa: E501
+            write_group_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +194,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AssayUpsert - a model defined in OpenAPI
+        """Project - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -225,18 +228,19 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (int): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            external_ids ({str: (str,)}): [optional]  # noqa: E501
-            sample_id (str): [optional]  # noqa: E501
+            name (str): [optional]  # noqa: E501
+            dataset (str): [optional]  # noqa: E501
             meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            read_group_name (str): [optional]  # noqa: E501
+            write_group_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.0.2/metamist/model/body_get_assays_by_criteria.py` & `metamist-6.0.3/metamist/model/body_get_assays_by_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-6.0.3/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/body_get_participants.py` & `metamist-6.0.3/metamist/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/body_get_samples.py` & `metamist-6.0.3/metamist/model/body_get_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/error_response.py` & `metamist-6.0.3/metamist/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/export_type.py` & `metamist-6.0.3/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/extra_participant_importer_handler.py` & `metamist-6.0.3/metamist/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/family_search_response_data.py` & `metamist-6.0.3/metamist/model/family_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/family_update_model.py` & `metamist-6.0.3/metamist/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/http_validation_error.py` & `metamist-6.0.3/metamist/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/meta_search_entity_prefix.py` & `metamist-6.0.3/metamist/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/nested_assay.py` & `metamist-6.0.3/metamist/model/validation_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class NestedAssay(ModelNormal):
+class ValidationError(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,44 +77,44 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (int,),  # noqa: E501
+            'loc': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
+            'msg': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
+        'loc': 'loc',  # noqa: E501
+        'msg': 'msg',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, type, meta, *args, **kwargs):  # noqa: E501
-        """NestedAssay - a model defined in OpenAPI
+    def _from_openapi_data(cls, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
 
         Args:
-            id (int):
+            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
+            msg (str):
             type (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -166,17 +166,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
+        self.loc = loc
+        self.msg = msg
         self.type = type
-        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -189,21 +189,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, type, meta, *args, **kwargs):  # noqa: E501
-        """NestedAssay - a model defined in OpenAPI
+    def __init__(self, loc, msg, type, *args, **kwargs):  # noqa: E501
+        """ValidationError - a model defined in OpenAPI
 
         Args:
-            id (int):
+            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
+            msg (str):
             type (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -253,17 +253,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
+        self.loc = loc
+        self.msg = msg
         self.type = type
-        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.0.2/metamist/model/nested_family.py` & `metamist-6.0.3/metamist/model/family_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class NestedFamily(ModelNormal):
+class FamilySimple(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, external_id, *args, **kwargs):  # noqa: E501
-        """NestedFamily - a model defined in OpenAPI
+        """FamilySimple - a model defined in OpenAPI
 
         Args:
             id (int):
             external_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
@@ -186,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, external_id, *args, **kwargs):  # noqa: E501
-        """NestedFamily - a model defined in OpenAPI
+        """FamilySimple - a model defined in OpenAPI
 
         Args:
             id (int):
             external_id (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `metamist-6.0.2/metamist/model/nested_participant.py` & `metamist-6.0.3/metamist/model/nested_participant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,17 +26,17 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from metamist.model.nested_family import NestedFamily
+    from metamist.model.family_simple import FamilySimple
     from metamist.model.nested_sample import NestedSample
-    globals()['NestedFamily'] = NestedFamily
+    globals()['FamilySimple'] = FamilySimple
     globals()['NestedSample'] = NestedSample
 
 
 class NestedParticipant(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -85,53 +85,55 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'families': ([NestedFamily],),  # noqa: E501
-            'samples': ([NestedSample],),  # noqa: E501
             'id': (int,),  # noqa: E501
-            'external_id': (str,),  # noqa: E501
             'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'samples': ([NestedSample],),  # noqa: E501
+            'families': ([FamilySimple],),  # noqa: E501
+            'external_id': (str,),  # noqa: E501
             'reported_sex': (int,),  # noqa: E501
             'reported_gender': (str,),  # noqa: E501
             'karyotype': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'families': 'families',  # noqa: E501
-        'samples': 'samples',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'external_id': 'external_id',  # noqa: E501
         'meta': 'meta',  # noqa: E501
+        'samples': 'samples',  # noqa: E501
+        'families': 'families',  # noqa: E501
+        'external_id': 'external_id',  # noqa: E501
         'reported_sex': 'reported_sex',  # noqa: E501
         'reported_gender': 'reported_gender',  # noqa: E501
         'karyotype': 'karyotype',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, families, samples, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, meta, samples, families, *args, **kwargs):  # noqa: E501
         """NestedParticipant - a model defined in OpenAPI
 
         Args:
-            families ([NestedFamily]):
+            id (int):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             samples ([NestedSample]):
+            families ([FamilySimple]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -156,17 +158,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
             external_id (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             reported_sex (int): [optional]  # noqa: E501
             reported_gender (str): [optional]  # noqa: E501
             karyotype (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -189,16 +189,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.families = families
+        self.id = id
+        self.meta = meta
         self.samples = samples
+        self.families = families
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -211,20 +213,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, families, samples, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, meta, samples, families, *args, **kwargs):  # noqa: E501
         """NestedParticipant - a model defined in OpenAPI
 
         Args:
-            families ([NestedFamily]):
+            id (int):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             samples ([NestedSample]):
+            families ([FamilySimple]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,17 +253,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
             external_id (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             reported_sex (int): [optional]  # noqa: E501
             reported_gender (str): [optional]  # noqa: E501
             karyotype (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -280,16 +282,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.families = families
+        self.id = id
+        self.meta = meta
         self.samples = samples
+        self.families = families
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.0.2/metamist/model/nested_sample.py` & `metamist-6.0.3/metamist/model/nested_sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,17 +26,17 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from metamist.model.nested_assay import NestedAssay
+    from metamist.model.assay import Assay
     from metamist.model.nested_sequencing_group import NestedSequencingGroup
-    globals()['NestedAssay'] = NestedAssay
+    globals()['Assay'] = Assay
     globals()['NestedSequencingGroup'] = NestedSequencingGroup
 
 
 class NestedSample(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -87,53 +87,51 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'external_id': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
             'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'sequencing_groups': ([NestedSequencingGroup],),  # noqa: E501
-            'non_sequencing_assays': ([NestedAssay],),  # noqa: E501
+            'non_sequencing_assays': ([Assay],),  # noqa: E501
+            'type': (str,),  # noqa: E501
             'created_date': (str,),  # noqa: E501
+            'sequencing_groups': ([NestedSequencingGroup],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
-        'type': 'type',  # noqa: E501
         'meta': 'meta',  # noqa: E501
-        'sequencing_groups': 'sequencing_groups',  # noqa: E501
         'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'created_date': 'created_date',  # noqa: E501
+        'sequencing_groups': 'sequencing_groups',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, external_id, type, meta, sequencing_groups, non_sequencing_assays, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, external_id, meta, non_sequencing_assays, *args, **kwargs):  # noqa: E501
         """NestedSample - a model defined in OpenAPI
 
         Args:
             id (str):
             external_id (str):
-            type (str):
             meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            sequencing_groups ([NestedSequencingGroup]):
-            non_sequencing_assays ([NestedAssay]):
+            non_sequencing_assays ([Assay]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -158,15 +156,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional]  # noqa: E501
             created_date (str): [optional]  # noqa: E501
+            sequencing_groups ([NestedSequencingGroup]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,17 +188,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.external_id = external_id
-        self.type = type
         self.meta = meta
-        self.sequencing_groups = sequencing_groups
         self.non_sequencing_assays = non_sequencing_assays
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -212,24 +210,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, external_id, type, meta, sequencing_groups, non_sequencing_assays, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, external_id, meta, non_sequencing_assays, *args, **kwargs):  # noqa: E501
         """NestedSample - a model defined in OpenAPI
 
         Args:
             id (str):
             external_id (str):
-            type (str):
             meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            sequencing_groups ([NestedSequencingGroup]):
-            non_sequencing_assays ([NestedAssay]):
+            non_sequencing_assays ([Assay]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -254,15 +250,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            type (str): [optional]  # noqa: E501
             created_date (str): [optional]  # noqa: E501
+            sequencing_groups ([NestedSequencingGroup]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -282,17 +280,15 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.external_id = external_id
-        self.type = type
         self.meta = meta
-        self.sequencing_groups = sequencing_groups
         self.non_sequencing_assays = non_sequencing_assays
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `metamist-6.0.2/metamist/model/nested_sequencing_group.py` & `metamist-6.0.3/metamist/model/nested_sequencing_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,16 +26,16 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from metamist.model.nested_assay import NestedAssay
-    globals()['NestedAssay'] = NestedAssay
+    from metamist.model.assay import Assay
+    globals()['Assay'] = Assay
 
 
 class NestedSequencingGroup(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -83,56 +83,55 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (int,),  # noqa: E501
-            'external_ids': ({str: (str,)},),  # noqa: E501
+            'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
             'technology': (str,),  # noqa: E501
             'platform': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'assays': ([NestedAssay],),  # noqa: E501
+            'meta': ({str: (str,)},),  # noqa: E501
+            'external_ids': ({str: (str,)},),  # noqa: E501
+            'assays': ([Assay],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'external_ids': 'external_ids',  # noqa: E501
         'type': 'type',  # noqa: E501
         'technology': 'technology',  # noqa: E501
         'platform': 'platform',  # noqa: E501
         'meta': 'meta',  # noqa: E501
+        'external_ids': 'external_ids',  # noqa: E501
         'assays': 'assays',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, external_ids, type, technology, platform, meta, assays, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, id, type, technology, platform, meta, external_ids, *args, **kwargs):  # noqa: E501
         """NestedSequencingGroup - a model defined in OpenAPI
 
         Args:
-            id (int):
-            external_ids ({str: (str,)}):
+            id (str):
             type (str):
             technology (str):
             platform (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            assays ([NestedAssay]):
+            meta ({str: (str,)}):
+            external_ids ({str: (str,)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -157,14 +156,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            assays ([Assay]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -185,20 +185,19 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.external_ids = external_ids
         self.type = type
         self.technology = technology
         self.platform = platform
         self.meta = meta
-        self.assays = assays
+        self.external_ids = external_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -211,25 +210,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, external_ids, type, technology, platform, meta, assays, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, type, technology, platform, meta, external_ids, *args, **kwargs):  # noqa: E501
         """NestedSequencingGroup - a model defined in OpenAPI
 
         Args:
-            id (int):
-            external_ids ({str: (str,)}):
+            id (str):
             type (str):
             technology (str):
             platform (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
-            assays ([NestedAssay]):
+            meta ({str: (str,)}):
+            external_ids ({str: (str,)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -254,14 +252,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            assays ([Assay]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -280,20 +279,19 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
-        self.external_ids = external_ids
         self.type = type
         self.technology = technology
         self.platform = platform
         self.meta = meta
-        self.assays = assays
+        self.external_ids = external_ids
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.0.2/metamist/model/paging_links.py` & `metamist-6.0.3/metamist/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/participant_search_response_data.py` & `metamist-6.0.3/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/participant_upsert.py` & `metamist-6.0.3/metamist/model/participant_upsert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -83,20 +83,20 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (int,),  # noqa: E501
-            'external_id': (str,),  # noqa: E501
-            'reported_sex': (int,),  # noqa: E501
-            'reported_gender': (str,),  # noqa: E501
-            'karyotype': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'reported_sex': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'reported_gender': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'karyotype': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'samples': ([SampleUpsert],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -148,20 +148,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            external_id (str): [optional]  # noqa: E501
-            reported_sex (int): [optional]  # noqa: E501
-            reported_gender (str): [optional]  # noqa: E501
-            karyotype (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            reported_sex (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            reported_gender (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            karyotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             samples ([SampleUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -236,20 +236,20 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            external_id (str): [optional]  # noqa: E501
-            reported_sex (int): [optional]  # noqa: E501
-            reported_gender (str): [optional]  # noqa: E501
-            karyotype (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            reported_sex (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            reported_gender (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            karyotype (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             samples ([SampleUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `metamist-6.0.2/metamist/model/project.py` & `metamist-6.0.3/metamist/model/sample_upsert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,22 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from metamist.model.assay_upsert import AssayUpsert
+    from metamist.model.sequencing_group_upsert import SequencingGroupUpsert
+    globals()['AssayUpsert'] = AssayUpsert
+    globals()['SequencingGroupUpsert'] = SequencingGroupUpsert
 
-class Project(ModelNormal):
+
+class SampleUpsert(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,60 +68,68 @@
 
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
-            'name': (str,),  # noqa: E501
-            'dataset': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'read_group_name': (str,),  # noqa: E501
-            'write_group_name': (str,),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'project': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'participant_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'active': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sequencing_groups': ([SequencingGroupUpsert],),  # noqa: E501
+            'non_sequencing_assays': ([AssayUpsert],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'dataset': 'dataset',  # noqa: E501
+        'external_id': 'external_id',  # noqa: E501
         'meta': 'meta',  # noqa: E501
-        'read_group_name': 'read_group_name',  # noqa: E501
-        'write_group_name': 'write_group_name',  # noqa: E501
+        'project': 'project',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'participant_id': 'participant_id',  # noqa: E501
+        'active': 'active',  # noqa: E501
+        'sequencing_groups': 'sequencing_groups',  # noqa: E501
+        'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Project - a model defined in OpenAPI
+        """SampleUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,20 +154,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            dataset (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            read_group_name (str): [optional]  # noqa: E501
-            write_group_name (str): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            participant_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sequencing_groups ([SequencingGroupUpsert]): [optional]  # noqa: E501
+            non_sequencing_assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -194,15 +211,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Project - a model defined in OpenAPI
+        """SampleUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -227,20 +244,23 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (int): [optional]  # noqa: E501
-            name (str): [optional]  # noqa: E501
-            dataset (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            read_group_name (str): [optional]  # noqa: E501
-            write_group_name (str): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            project (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            participant_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            active (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sequencing_groups ([SequencingGroupUpsert]): [optional]  # noqa: E501
+            non_sequencing_assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.0.2/metamist/model/project_summary_response.py` & `metamist-6.0.3/metamist/model/project_summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -34,15 +34,15 @@
     from metamist.model.paging_links import PagingLinks
     from metamist.model.web_project import WebProject
     globals()['NestedParticipant'] = NestedParticipant
     globals()['PagingLinks'] = PagingLinks
     globals()['WebProject'] = WebProject
 
 
-class ProjectSummaryResponse(ModelNormal):
+class ProjectSummary(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -88,41 +88,41 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'project': (WebProject,),  # noqa: E501
-            'total_participants': (int,),  # noqa: E501
             'total_samples': (int,),  # noqa: E501
             'total_samples_in_query': (int,),  # noqa: E501
+            'total_participants': (int,),  # noqa: E501
             'total_sequencing_groups': (int,),  # noqa: E501
             'total_assays': (int,),  # noqa: E501
             'cram_seqr_stats': ({str: ({str: (str,)},)},),  # noqa: E501
             'batch_sequencing_group_stats': ({str: ({str: (str,)},)},),  # noqa: E501
             'participants': ([NestedParticipant],),  # noqa: E501
-            'participant_keys': ([[str]],),  # noqa: E501
-            'sample_keys': ([[str]],),  # noqa: E501
-            'sequencing_group_keys': ([[str]],),  # noqa: E501
-            'assay_keys': ([[str]],),  # noqa: E501
+            'participant_keys': ([list],),  # noqa: E501
+            'sample_keys': ([list],),  # noqa: E501
+            'sequencing_group_keys': ([list],),  # noqa: E501
+            'assay_keys': ([list],),  # noqa: E501
             'seqr_links': ({str: (str,)},),  # noqa: E501
             'seqr_sync_types': ([str],),  # noqa: E501
             'links': (PagingLinks,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'project': 'project',  # noqa: E501
-        'total_participants': 'total_participants',  # noqa: E501
         'total_samples': 'total_samples',  # noqa: E501
         'total_samples_in_query': 'total_samples_in_query',  # noqa: E501
+        'total_participants': 'total_participants',  # noqa: E501
         'total_sequencing_groups': 'total_sequencing_groups',  # noqa: E501
         'total_assays': 'total_assays',  # noqa: E501
         'cram_seqr_stats': 'cram_seqr_stats',  # noqa: E501
         'batch_sequencing_group_stats': 'batch_sequencing_group_stats',  # noqa: E501
         'participants': 'participants',  # noqa: E501
         'participant_keys': 'participant_keys',  # noqa: E501
         'sample_keys': 'sample_keys',  # noqa: E501
@@ -136,31 +136,31 @@
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, project, total_participants, total_samples, total_samples_in_query, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, *args, **kwargs):  # noqa: E501
-        """ProjectSummaryResponse - a model defined in OpenAPI
+    def _from_openapi_data(cls, project, total_samples, total_samples_in_query, total_participants, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, *args, **kwargs):  # noqa: E501
+        """ProjectSummary - a model defined in OpenAPI
 
         Args:
             project (WebProject):
-            total_participants (int):
             total_samples (int):
             total_samples_in_query (int):
+            total_participants (int):
             total_sequencing_groups (int):
             total_assays (int):
             cram_seqr_stats ({str: ({str: (str,)},)}):
             batch_sequencing_group_stats ({str: ({str: (str,)},)}):
             participants ([NestedParticipant]):
-            participant_keys ([[str]]):
-            sample_keys ([[str]]):
-            sequencing_group_keys ([[str]]):
-            assay_keys ([[str]]):
+            participant_keys ([list]):
+            sample_keys ([list]):
+            sequencing_group_keys ([list]):
+            assay_keys ([list]):
             seqr_links ({str: (str,)}):
             seqr_sync_types ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -216,17 +216,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.project = project
-        self.total_participants = total_participants
         self.total_samples = total_samples
         self.total_samples_in_query = total_samples_in_query
+        self.total_participants = total_participants
         self.total_sequencing_groups = total_sequencing_groups
         self.total_assays = total_assays
         self.cram_seqr_stats = cram_seqr_stats
         self.batch_sequencing_group_stats = batch_sequencing_group_stats
         self.participants = participants
         self.participant_keys = participant_keys
         self.sample_keys = sample_keys
@@ -250,31 +250,31 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, project, total_participants, total_samples, total_samples_in_query, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, *args, **kwargs):  # noqa: E501
-        """ProjectSummaryResponse - a model defined in OpenAPI
+    def __init__(self, project, total_samples, total_samples_in_query, total_participants, total_sequencing_groups, total_assays, cram_seqr_stats, batch_sequencing_group_stats, participants, participant_keys, sample_keys, sequencing_group_keys, assay_keys, seqr_links, seqr_sync_types, *args, **kwargs):  # noqa: E501
+        """ProjectSummary - a model defined in OpenAPI
 
         Args:
             project (WebProject):
-            total_participants (int):
             total_samples (int):
             total_samples_in_query (int):
+            total_participants (int):
             total_sequencing_groups (int):
             total_assays (int):
             cram_seqr_stats ({str: ({str: (str,)},)}):
             batch_sequencing_group_stats ({str: ({str: (str,)},)}):
             participants ([NestedParticipant]):
-            participant_keys ([[str]]):
-            sample_keys ([[str]]):
-            sequencing_group_keys ([[str]]):
-            assay_keys ([[str]]):
+            participant_keys ([list]):
+            sample_keys ([list]):
+            sequencing_group_keys ([list]):
+            assay_keys ([list]):
             seqr_links ({str: (str,)}):
             seqr_sync_types ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
@@ -328,17 +328,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.project = project
-        self.total_participants = total_participants
         self.total_samples = total_samples
         self.total_samples_in_query = total_samples_in_query
+        self.total_participants = total_participants
         self.total_sequencing_groups = total_sequencing_groups
         self.total_assays = total_assays
         self.cram_seqr_stats = cram_seqr_stats
         self.batch_sequencing_group_stats = batch_sequencing_group_stats
         self.participants = participants
         self.participant_keys = participant_keys
         self.sample_keys = sample_keys
```

### Comparing `metamist-6.0.2/metamist/model/sample_search_response_data.py` & `metamist-6.0.3/metamist/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/sample_upsert.py` & `metamist-6.0.3/metamist/model/assay_upsert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,22 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.assay_upsert import AssayUpsert
-    from metamist.model.sequencing_group_upsert import SequencingGroupUpsert
-    globals()['AssayUpsert'] = AssayUpsert
-    globals()['SequencingGroupUpsert'] = SequencingGroupUpsert
 
-
-class SampleUpsert(ModelNormal):
+class AssayUpsert(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -68,68 +62,58 @@
 
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
-            'id': (str,),  # noqa: E501
-            'external_id': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'project': (int,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'participant_id': (int,),  # noqa: E501
-            'active': (bool,),  # noqa: E501
-            'sequencing_groups': ([SequencingGroupUpsert],),  # noqa: E501
-            'non_sequencing_assays': ([AssayUpsert],),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sample_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'external_id': 'external_id',  # noqa: E501
-        'meta': 'meta',  # noqa: E501
-        'project': 'project',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'participant_id': 'participant_id',  # noqa: E501
-        'active': 'active',  # noqa: E501
-        'sequencing_groups': 'sequencing_groups',  # noqa: E501
-        'non_sequencing_assays': 'non_sequencing_assays',  # noqa: E501
+        'external_ids': 'external_ids',  # noqa: E501
+        'sample_id': 'sample_id',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """SampleUpsert - a model defined in OpenAPI
+        """AssayUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -154,23 +138,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            external_id (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            project (int): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            participant_id (int): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
-            sequencing_groups ([SequencingGroupUpsert]): [optional]  # noqa: E501
-            non_sequencing_assays ([AssayUpsert]): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -211,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """SampleUpsert - a model defined in OpenAPI
+        """AssayUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -244,23 +224,19 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): [optional]  # noqa: E501
-            external_id (str): [optional]  # noqa: E501
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            project (int): [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
-            participant_id (int): [optional]  # noqa: E501
-            active (bool): [optional]  # noqa: E501
-            sequencing_groups ([SequencingGroupUpsert]): [optional]  # noqa: E501
-            non_sequencing_assays ([AssayUpsert]): [optional]  # noqa: E501
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `metamist-6.0.2/metamist/model/search_item.py` & `metamist-6.0.3/metamist/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/search_response.py` & `metamist-6.0.3/metamist/model/search_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/search_response_model.py` & `metamist-6.0.3/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/search_response_type.py` & `metamist-6.0.3/metamist/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.2/metamist/model/sequencing_group_upsert.py` & `metamist-6.0.3/metamist/model/web_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from metamist.model.assay_upsert import AssayUpsert
-    globals()['AssayUpsert'] = AssayUpsert
 
-
-class SequencingGroupUpsert(ModelNormal):
+class WebProject(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,71 +62,62 @@
 
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
-            'type': (str,),  # noqa: E501
-            'technology': (str,),  # noqa: E501
-            'platform': (str,),  # noqa: E501
-            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
-            'meta': ({str: (str,)},),  # noqa: E501
-            'sample_id': (str,),  # noqa: E501
-            'external_ids': ({str: (str,)},),  # noqa: E501
-            'assays': ([AssayUpsert],),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'name': (str,),  # noqa: E501
+            'dataset': (str,),  # noqa: E501
+            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'type': 'type',  # noqa: E501
-        'technology': 'technology',  # noqa: E501
-        'platform': 'platform',  # noqa: E501
         'id': 'id',  # noqa: E501
+        'name': 'name',  # noqa: E501
+        'dataset': 'dataset',  # noqa: E501
         'meta': 'meta',  # noqa: E501
-        'sample_id': 'sample_id',  # noqa: E501
-        'external_ids': 'external_ids',  # noqa: E501
-        'assays': 'assays',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, type, technology, platform, *args, **kwargs):  # noqa: E501
-        """SequencingGroupUpsert - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
+        """WebProject - a model defined in OpenAPI
 
         Args:
-            type (str):
-            technology (str):
-            platform (str):
+            id (int):
+            name (str):
+            dataset (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -155,19 +142,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            meta ({str: (str,)}): [optional]  # noqa: E501
-            sample_id (str): [optional]  # noqa: E501
-            external_ids ({str: (str,)}): [optional]  # noqa: E501
-            assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,17 +169,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.technology = technology
-        self.platform = platform
+        self.id = id
+        self.name = name
+        self.dataset = dataset
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -210,21 +193,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, type, technology, platform, *args, **kwargs):  # noqa: E501
-        """SequencingGroupUpsert - a model defined in OpenAPI
+    def __init__(self, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
+        """WebProject - a model defined in OpenAPI
 
         Args:
-            type (str):
-            technology (str):
-            platform (str):
+            id (int):
+            name (str):
+            dataset (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -249,19 +233,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
-            meta ({str: (str,)}): [optional]  # noqa: E501
-            sample_id (str): [optional]  # noqa: E501
-            external_ids ({str: (str,)}): [optional]  # noqa: E501
-            assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -279,17 +258,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.type = type
-        self.technology = technology
-        self.platform = platform
+        self.id = id
+        self.name = name
+        self.dataset = dataset
+        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.0.2/metamist/model/validation_error.py` & `metamist-6.0.3/metamist/model/assay.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
 
-class ValidationError(ModelNormal):
+class Assay(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,43 +77,49 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'loc': ([bool, date, datetime, dict, float, int, list, str, none_type],),  # noqa: E501
-            'msg': (str,),  # noqa: E501
+            'id': (int,),  # noqa: E501
+            'external_ids': ({str: (str,)},),  # noqa: E501
+            'sample_id': (str,),  # noqa: E501
+            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
             'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'loc': 'loc',  # noqa: E501
-        'msg': 'msg',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'external_ids': 'external_ids',  # noqa: E501
+        'sample_id': 'sample_id',  # noqa: E501
+        'meta': 'meta',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, loc, msg, type, *args, **kwargs):  # noqa: E501
-        """ValidationError - a model defined in OpenAPI
+    def _from_openapi_data(cls, id, external_ids, sample_id, meta, type, *args, **kwargs):  # noqa: E501
+        """Assay - a model defined in OpenAPI
 
         Args:
-            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
-            msg (str):
+            id (int):
+            external_ids ({str: (str,)}):
+            sample_id (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -166,16 +172,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.loc = loc
-        self.msg = msg
+        self.id = id
+        self.external_ids = external_ids
+        self.sample_id = sample_id
+        self.meta = meta
         self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -189,20 +197,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, loc, msg, type, *args, **kwargs):  # noqa: E501
-        """ValidationError - a model defined in OpenAPI
+    def __init__(self, id, external_ids, sample_id, meta, type, *args, **kwargs):  # noqa: E501
+        """Assay - a model defined in OpenAPI
 
         Args:
-            loc ([bool, date, datetime, dict, float, int, list, str, none_type]):
-            msg (str):
+            id (int):
+            external_ids ({str: (str,)}):
+            sample_id (str):
+            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
             type (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -253,16 +263,18 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.loc = loc
-        self.msg = msg
+        self.id = id
+        self.external_ids = external_ids
+        self.sample_id = sample_id
+        self.meta = meta
         self.type = type
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `metamist-6.0.2/metamist/model/web_project.py` & `metamist-6.0.3/metamist/model/sequencing_group_upsert.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
 )
 from ..model_utils import OpenApiModel
 from metamist.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from metamist.model.assay_upsert import AssayUpsert
+    globals()['AssayUpsert'] = AssayUpsert
 
-class WebProject(ModelNormal):
+
+class SequencingGroupUpsert(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,62 +66,66 @@
 
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
-            'name': (str,),  # noqa: E501
-            'dataset': (str,),  # noqa: E501
-            'meta': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
+            'id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'type': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'technology': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'platform': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'meta': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'sample_id': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'external_ids': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
+            'assays': ([AssayUpsert],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'name': 'name',  # noqa: E501
-        'dataset': 'dataset',  # noqa: E501
+        'type': 'type',  # noqa: E501
+        'technology': 'technology',  # noqa: E501
+        'platform': 'platform',  # noqa: E501
         'meta': 'meta',  # noqa: E501
+        'sample_id': 'sample_id',  # noqa: E501
+        'external_ids': 'external_ids',  # noqa: E501
+        'assays': 'assays',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
-        """WebProject - a model defined in OpenAPI
-
-        Args:
-            id (int):
-            name (str):
-            dataset (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """SequencingGroupUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -142,14 +150,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            technology (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            platform (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -169,18 +185,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
-        self.dataset = dataset
-        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,22 +205,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, name, dataset, meta, *args, **kwargs):  # noqa: E501
-        """WebProject - a model defined in OpenAPI
-
-        Args:
-            id (int):
-            name (str):
-            dataset (str):
-            meta ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """SequencingGroupUpsert - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -233,14 +239,22 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            technology (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            platform (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            meta (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            sample_id (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            external_ids (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
+            assays ([AssayUpsert]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -258,18 +272,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.id = id
-        self.name = name
-        self.dataset = dataset
-        self.meta = meta
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `metamist-6.0.2/metamist/model_utils.py` & `metamist-6.0.3/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-6.0.2/metamist/models/__init__.py` & `metamist-6.0.3/metamist/models/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 # import sys
 # sys.setrecursionlimit(n)
 
 from metamist.model.analysis import Analysis
 from metamist.model.analysis_query_model import AnalysisQueryModel
 from metamist.model.analysis_status import AnalysisStatus
 from metamist.model.analysis_update_model import AnalysisUpdateModel
+from metamist.model.assay import Assay
 from metamist.model.assay_upsert import AssayUpsert
 from metamist.model.body_get_assays_by_criteria import BodyGetAssaysByCriteria
 from metamist.model.body_get_latest_complete_analysis_for_type_post import BodyGetLatestCompleteAnalysisForTypePost
 from metamist.model.body_get_participants import BodyGetParticipants
 from metamist.model.body_get_samples import BodyGetSamples
 from metamist.model.error_response import ErrorResponse
 from metamist.model.export_type import ExportType
 from metamist.model.extra_participant_importer_handler import ExtraParticipantImporterHandler
 from metamist.model.family_search_response_data import FamilySearchResponseData
+from metamist.model.family_simple import FamilySimple
 from metamist.model.family_update_model import FamilyUpdateModel
 from metamist.model.http_validation_error import HTTPValidationError
 from metamist.model.meta_search_entity_prefix import MetaSearchEntityPrefix
-from metamist.model.nested_assay import NestedAssay
-from metamist.model.nested_family import NestedFamily
 from metamist.model.nested_participant import NestedParticipant
 from metamist.model.nested_sample import NestedSample
 from metamist.model.nested_sequencing_group import NestedSequencingGroup
 from metamist.model.paging_links import PagingLinks
 from metamist.model.participant_search_response_data import ParticipantSearchResponseData
 from metamist.model.participant_upsert import ParticipantUpsert
 from metamist.model.project import Project
-from metamist.model.project_summary_response import ProjectSummaryResponse
+from metamist.model.project_summary import ProjectSummary
 from metamist.model.sample_search_response_data import SampleSearchResponseData
 from metamist.model.sample_upsert import SampleUpsert
 from metamist.model.search_item import SearchItem
 from metamist.model.search_response import SearchResponse
 from metamist.model.search_response_model import SearchResponseModel
 from metamist.model.search_response_type import SearchResponseType
 from metamist.model.sequencing_group_upsert import SequencingGroupUpsert
```

### Comparing `metamist-6.0.2/metamist/parser/cloudhelper.py` & `metamist-6.0.3/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/metamist/parser/generic_metadata_parser.py` & `metamist-6.0.3/metamist/parser/generic_metadata_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             for r in grp if isinstance(grp, list) else [grp]:
                 filename_promises.append(
                     self.get_all_files_from_row(self.get_sample_id(r), r)
                 )
 
         files_from_rows: List[str] = sum(await asyncio.gather(*filename_promises), [])
         filenames_from_rows = set(f.strip() for f in files_from_rows if f and f.strip())
-        relevant_extensions = ('.cram', '.fastq.gz', '.bam')
+        relevant_extensions = ('.cram', '.fastq.gz', '.fastq', 'fq.gz', '.fq', '.bam')
 
         # we need to explicitly filter filenames from rows not to include absolute
         # paths, otherwise the below check will flag it as missing
         absolute_path_starts = ('/', 'gs://', 'https://')
         filenames_from_rows = set(
             f
             for f in filenames_from_rows
```

### Comparing `metamist-6.0.2/metamist/parser/generic_parser.py` & `metamist-6.0.3/metamist/parser/generic_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,23 @@
         self.karyotype = karyotype
         self.meta = meta
 
         self.samples: list[ParsedSample] = []
 
     def to_sm(self) -> ParticipantUpsert:
         """Convert to SM upsert model"""
-        return ParticipantUpsert(samples=[s.to_sm() for s in self.samples])
+        samples = [s.to_sm() for s in self.samples]
+        return ParticipantUpsert(
+            external_id=self.external_pid,
+            reported_sex=self.reported_sex,
+            reported_gender=self.reported_gender,
+            karyotype=self.karyotype,
+            meta=self.meta,
+            samples=samples,
+        )
 
 
 class ParsedSample:
     """Class for holding sample metadata grouped by id"""
 
     def __init__(
         self,
@@ -307,14 +315,15 @@
         self.external_ids = external_seq_ids
         self.assay_type = assay_type
         self.meta = meta
 
     def to_sm(self) -> AssayUpsert:
         """Convert to SM upsert model"""
         return AssayUpsert(
+            type=self.assay_type,
             id=self.internal_id,
             external_ids=self.external_ids,
             # sample_id=self.s,
             meta=self.meta,
         )
```

### Comparing `metamist-6.0.2/metamist/parser/sample_file_map_parser.py` & `metamist-6.0.3/metamist/parser/sample_file_map_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/metamist/rest.py` & `metamist-6.0.3/metamist/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.2
+    The version of the OpenAPI document: 6.0.3
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-6.0.2/metamist.egg-info/PKG-INFO` & `metamist-6.0.3/metamist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.2
+Version: 6.0.3
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.2/metamist.egg-info/SOURCES.txt` & `metamist-6.0.3/metamist.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 metamist.egg-info/dependency_links.txt
 metamist.egg-info/not-zip-safe
 metamist.egg-info/requires.txt
 metamist.egg-info/top_level.txt
 metamist/api/__init__.py
 metamist/api/analysis_api.py
 metamist/api/assay_api.py
-metamist/api/default_api.py
 metamist/api/enums_api.py
 metamist/api/family_api.py
 metamist/api/import_api.py
 metamist/api/participant_api.py
 metamist/api/project_api.py
 metamist/api/sample_api.py
 metamist/api/seqr_api.py
@@ -32,36 +31,36 @@
 metamist/graphql/__init__.py
 metamist/graphql/schema.graphql
 metamist/model/__init__.py
 metamist/model/analysis.py
 metamist/model/analysis_query_model.py
 metamist/model/analysis_status.py
 metamist/model/analysis_update_model.py
+metamist/model/assay.py
 metamist/model/assay_upsert.py
 metamist/model/body_get_assays_by_criteria.py
 metamist/model/body_get_latest_complete_analysis_for_type_post.py
 metamist/model/body_get_participants.py
 metamist/model/body_get_samples.py
 metamist/model/error_response.py
 metamist/model/export_type.py
 metamist/model/extra_participant_importer_handler.py
 metamist/model/family_search_response_data.py
+metamist/model/family_simple.py
 metamist/model/family_update_model.py
 metamist/model/http_validation_error.py
 metamist/model/meta_search_entity_prefix.py
-metamist/model/nested_assay.py
-metamist/model/nested_family.py
 metamist/model/nested_participant.py
 metamist/model/nested_sample.py
 metamist/model/nested_sequencing_group.py
 metamist/model/paging_links.py
 metamist/model/participant_search_response_data.py
 metamist/model/participant_upsert.py
 metamist/model/project.py
-metamist/model/project_summary_response.py
+metamist/model/project_summary.py
 metamist/model/sample_search_response_data.py
 metamist/model/sample_upsert.py
 metamist/model/search_item.py
 metamist/model/search_response.py
 metamist/model/search_response_model.py
 metamist/model/search_response_type.py
 metamist/model/sequencing_group_upsert.py
@@ -72,17 +71,20 @@
 metamist/parser/cloudhelper.py
 metamist/parser/generic_metadata_parser.py
 metamist/parser/generic_parser.py
 metamist/parser/sample_file_map_parser.py
 test/test_analysis.py
 test/test_assay.py
 test/test_generate_data.py
+test/test_generic_filters.py
 test/test_get_participants.py
 test/test_graphql.py
 test/test_import_individual_metadata.py
+test/test_metamist.py
+test/test_models.py
 test/test_parse_existing_cohort.py
 test/test_parse_file_map.py
 test/test_parse_generic_metadata.py
 test/test_parse_ont_processor.py
 test/test_parse_ont_sheet.py
 test/test_pedigree.py
 test/test_sample.py
```

### Comparing `metamist-6.0.2/setup.py` & `metamist-6.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.0.2',
+    version='6.0.3',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-6.0.2/test/test_analysis.py` & `metamist-6.0.3/test/test_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # pylint: disable=invalid-overridden-method
 from datetime import timedelta, datetime
 
 from test.testbase import DbIsolatedTest, run_as_sync
 
+from db.python.tables.analysis import AnalysisFilter
+from db.python.utils import GenericFilter
 from db.python.layers.assay import AssayLayer
 from db.python.layers.analysis import AnalysisLayer
 from db.python.layers.sample import SampleLayer
 from db.python.layers.sequencing_group import SequencingGroupLayer
 from models.models import (
     AnalysisInternal,
     AssayUpsertInternal,
     SequencingGroupUpsertInternal,
     SampleUpsertInternal,
 )
-
 from models.enums import AnalysisStatus
 
 
 class TestAnalysis(DbIsolatedTest):
     """Test sample class"""
 
     @run_as_sync
@@ -71,15 +72,15 @@
                         ],
                     ),
                 ],
             )
         )
         self.sample_id = sample.id
         self.genome_sequencing_group_id = sample.sequencing_groups[0].id
-        self.exome_sequencing_group_id = sample.sequencing_groups[1].id
+        self.exome_sequencing_group_id = sample.sequencing_groups[self.project_id].id
 
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.genome_sequencing_group_id],
                 meta={'sequence_type': 'genome', 'size': 1024},
@@ -89,23 +90,22 @@
     @run_as_sync
     async def test_add_cram(self):
         """
         Test adding an analysis of type CRAM
         """
 
         analyses = await self.connection.connection.fetch_all('SELECT * FROM analysis')
-        analysis_samples = await self.connection.connection.fetch_all(
+        analysis_sgs = await self.connection.connection.fetch_all(
             'SELECT * FROM analysis_sequencing_group'
         )
-        # print(analyses, analysis_samples)
 
         self.assertEqual(1, len(analyses))
 
-        self.assertEqual(1, analysis_samples[0]['sequencing_group_id'])
-        self.assertEqual(analyses[0]['id'], analysis_samples[0]['analysis_id'])
+        self.assertEqual(1, analysis_sgs[0]['sequencing_group_id'])
+        self.assertEqual(analyses[0]['id'], analysis_sgs[0]['analysis_id'])
 
     @run_as_sync
     async def test_get_analysis(self):
         """
         Test adding an analysis of type ANALYSIS_RUNNER
         """
 
@@ -114,16 +114,19 @@
                 type='analysis-runner',
                 status=AnalysisStatus.UNKNOWN,
                 sequence_group_ids=[],
                 meta={},
             )
         )
 
-        analyses = await self.al.query_analysis(
-            project_ids=[1], analysis_type='analysis-runner'
+        analyses = await self.al.query(
+            AnalysisFilter(
+                project=GenericFilter(eq=self.project_id),
+                type=GenericFilter(eq='analysis-runner'),
+            )
         )
         expected = [
             AnalysisInternal(
                 id=a_id,
                 type='analysis-runner',
                 status=AnalysisStatus.UNKNOWN,
                 sequence_group_ids=[],
@@ -142,15 +145,15 @@
     async def test_get_sequencing_group_file_sizes_single(self):
         """
         Test retrieval of sample file sizes over time
         """
 
         today = datetime.utcnow().date()
 
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[1])
+        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
         expected = {
             'project': self.project_id,
             'sequencing_groups': {
                 self.genome_sequencing_group_id: [
                     {
                         'start': today,
                         'end': None,
@@ -198,29 +201,29 @@
                         'size': 3141,
                     }
                 ],
             },
         }
 
         # Assert that the exome size was added correctly
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[1])
+        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
         self.assertDictEqual(expected, result[0])
 
     @run_as_sync
     async def test_get_sequencing_group_file_sizes_exclusive_date_range(self):
         """
         Exclusive date range returning no data
         """
         today = datetime.utcnow().date()
 
         # Assert that if we select a date range outside of sample creation date
         # that is doesn't show up in the map
         yesterday = today - timedelta(days=3)
         result = await self.al.get_sequencing_group_file_sizes(
-            project_ids=[1], end_date=yesterday
+            project_ids=[self.project_id], end_date=yesterday
         )
 
         self.assertEqual([], result)
 
     @run_as_sync
     async def test_get_sequencing_group_file_sizes_newer_sample(self):
         """
@@ -246,15 +249,15 @@
                         'end': None,
                         'size': 11111,
                     }
                 ]
             },
         }
 
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[1])
+        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
         self.assertDictEqual(expected, result[0])
 
     @run_as_sync
     async def test_get_sequencing_group_file_sizes_two_samples(self):
         """Test that it works for two samples"""
         today = datetime.utcnow().date()
 
@@ -312,9 +315,9 @@
                         'end': None,
                         'size': 987654321,
                     }
                 ],
             },
         }
 
-        result = await self.al.get_sequencing_group_file_sizes(project_ids=[1])
+        result = await self.al.get_sequencing_group_file_sizes(project_ids=[self.project_id])
         self.assertDictEqual(expected, result[0])
```

### Comparing `metamist-6.0.2/test/test_assay.py` & `metamist-6.0.3/test/test_assay.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from test.testbase import DbIsolatedTest, run_as_sync
 from pymysql.err import IntegrityError
 
 from db.python.connect import NotFoundError
 from db.python.layers.sample import SampleLayer
 from db.python.layers.assay import AssayLayer
 from db.python.enum_tables import AssayTypeTable
+from db.python.tables.assay import AssayFilter
+from db.python.utils import GenericFilter
 from models.models.assay import AssayUpsertInternal
 from models.models.sample import SampleUpsertInternal
 
 default_sequencing_meta = {
     'sequencing_type': 'genome',
     'sequencing_platform': 'short-read',
     'sequencing_technology': 'illumina',
@@ -47,15 +49,15 @@
     async def test_not_found_assay(self):
         """
         Test the NotFoundError when getting an invalid assay ID
         """
 
         @run_as_sync
         async def get():
-            return await self.assaylayer.get_assay_by_id(9999, check_project_id=False)
+            return await self.assaylayer.get_assay_by_id(-1, check_project_id=False)
 
         self.assertRaises(NotFoundError, get)
 
     @run_as_sync
     async def test_upsert_assay(self):
         """
         Test inserting a assay, and check all values are inserted correctly
@@ -194,23 +196,20 @@
                 sample_id=self.sample_id_raw,
                 type='sequencing',
                 meta={**default_sequencing_meta},
                 external_ids={'default': 'SEQ02'},
             )
         )
 
-        self.assertEqual(
-            seq1.id, (await self.assaylayer.get_assay_by_external_id('SEQ01')).id
-        )
-        self.assertEqual(
-            seq1.id, (await self.assaylayer.get_assay_by_external_id('EXT_SEQ1')).id
-        )
-        self.assertEqual(
-            seq2.id, (await self.assaylayer.get_assay_by_external_id('SEQ02')).id
-        )
+        fquery_1 = AssayFilter(external_id='SEQ01', project=self.project_id)
+        self.assertEqual(seq1.id, (await self.assaylayer.query(fquery_1))[0].id)
+        fquery_2 = AssayFilter(external_id='EXT_SEQ1', project=self.project_id)
+        self.assertEqual(seq1.id, (await self.assaylayer.query(fquery_2))[0].id)
+        fquery_3 = AssayFilter(external_id='SEQ02', project=self.project_id)
+        self.assertEqual(seq2.id, (await self.assaylayer.query(fquery_3))[0].id)
 
     @run_as_sync
     async def test_get_assays_by_sample_id(self):
         """Get many assays by sample ID"""
         seq1 = await self.assaylayer.upsert_assay(
             AssayUpsertInternal(
                 sample_id=self.sample_id_raw,
@@ -266,77 +265,103 @@
                     type='sequencing',
                     meta={'unique': 'b', 'common': 'common', **default_sequencing_meta},
                     external_ids={'default': 'SEQ02'},
                 ),
             ]
         )
 
-        async def search_result_to_ids(**query):
-            seqs = await self.assaylayer.get_assays_by(
-                **query, project_ids=[self.project_id]
-            )
+        async def search_result_to_ids(filter_: AssayFilter):
+            filter_.project = GenericFilter(eq=self.project_id)
+            seqs = await self.assaylayer.query(filter_)
             return {s.id for s in seqs}
 
         seq1_id = seqs[0].id
         seq2_id = seqs[1].id
 
         # sample_ids
         self.assertSetEqual(
             {seq1_id, seq2_id},
-            await search_result_to_ids(sample_ids=[sample_id_for_test]),
+            await search_result_to_ids(
+                AssayFilter(sample_id=GenericFilter(in_=[sample_id_for_test]))
+            ),
+        )
+        self.assertSetEqual(
+            set(),
+            await search_result_to_ids(
+                AssayFilter(sample_id=GenericFilter(in_=[9_999_999]))
+            ),
         )
-        self.assertSetEqual(set(), await search_result_to_ids(sample_ids=[9_999_999]))
 
         # external assay IDs
         self.assertSetEqual(
-            {seq1_id}, await search_result_to_ids(external_assay_ids=['SEQ01'])
+            {seq1_id},
+            await search_result_to_ids(
+                AssayFilter(external_id=GenericFilter(eq='SEQ01'))
+            ),
         )
         self.assertSetEqual(
             {seq1_id, seq2_id},
-            await search_result_to_ids(external_assay_ids=['SEQ01', 'SEQ02']),
+            await search_result_to_ids(
+                AssayFilter(
+                    external_id=GenericFilter(in_=['SEQ01', 'SEQ02']),
+                )
+            ),
         )
 
         # seq_meta
         self.assertSetEqual(
-            {seq2_id}, await search_result_to_ids(assay_meta={'unique': 'b'})
+            {seq2_id},
+            await search_result_to_ids(
+                AssayFilter(meta={'unique': GenericFilter(eq='b')})
+            ),
         )
         self.assertSetEqual(
             {seq1_id, seq2_id},
-            await search_result_to_ids(assay_meta={'common': 'common'}),
+            await search_result_to_ids(AssayFilter(meta={'common': 'common'})),
         )
 
         # sample meta
         self.assertSetEqual(
             {seq1_id, seq2_id},
-            await search_result_to_ids(sample_meta={'collection-year': '2022'}),
+            await search_result_to_ids(
+                AssayFilter(sample_meta={'collection-year': '2022'})
+            ),
         )
         self.assertSetEqual(
-            set(), await search_result_to_ids(sample_meta={'unknown_key': '2022'})
+            set(),
+            await search_result_to_ids(
+                AssayFilter(sample_meta={'unknown_key': '2022'})
+            ),
         )
 
         # assay types
         self.assertSetEqual(
-            {seq1_id, seq2_id}, await search_result_to_ids(assay_types=['sequencing'])
+            {seq1_id, seq2_id},
+            await search_result_to_ids(
+                AssayFilter(type=GenericFilter(in_=['sequencing']))
+            ),
         )
-        # self.assertSetEqual(
-        #     {seq1_id, seq2_id},
-        #     await search_result_to_ids(types=[SequenceType.GENOME, SequenceType.EXOME]),
-        # )
 
         # combination
         self.assertSetEqual(
             {seq2_id},
             await search_result_to_ids(
-                sample_meta={'collection-year': '2022'}, external_assay_ids=['SEQ02']
+                AssayFilter(
+                    sample_meta={'collection-year': '2022'},
+                    external_id=GenericFilter(in_=['SEQ02']),
+                )
             ),
         )
         self.assertSetEqual(
             {seq1_id},
             await search_result_to_ids(
-                external_assay_ids=['SEQ01'], assay_types=['sequencing']
+                AssayFilter(
+                    external_id=GenericFilter(in_=['SEQ01']),
+                    type=GenericFilter(eq='sequencing'),
+                )
             ),
         )
         # self.assertSetEqual(
         #     set(),
         #     await search_result_to_ids(
         #         external_assay_ids=['SEQ01'], types=[SequenceType.EXOME]
         #     ),
```

### Comparing `metamist-6.0.2/test/test_generate_data.py` & `metamist-6.0.3/test/test_generate_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 from test.data.generate_data import QUERY_ENUMS, QUERY_SG_ID
 from metamist.graphql import validate, configure_sync_client
-from api.graphql.schema import schema   # type: ignore
+from api.graphql.schema import schema  # type: ignore
 
 
 class ValidateGenerateDataQueries(unittest.TestCase):
     """Validate generate data queries"""
+
     def test_validate_queries(self):
         """Validate queries"""
         client = configure_sync_client(schema=schema.as_str(), auth_token='FAKE')
         validate(QUERY_ENUMS, client=client)
         validate(QUERY_SG_ID, client=client)
```

### Comparing `metamist-6.0.2/test/test_get_participants.py` & `metamist-6.0.3/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_graphql.py` & `metamist-6.0.3/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_import_individual_metadata.py` & `metamist-6.0.3/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_parse_existing_cohort.py` & `metamist-6.0.3/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_parse_file_map.py` & `metamist-6.0.3/test/test_parse_file_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from io import StringIO
 from unittest.mock import patch
 from test.testbase import DbIsolatedTest, run_as_sync
 
+from metamist.parser.generic_parser import ParsedParticipant
 from metamist.parser.sample_file_map_parser import SampleFileMapParser
 
 
 class TestSampleMapParser(DbIsolatedTest):
     """Test the TestSampleMapParser"""
 
     @run_as_sync
@@ -72,14 +73,44 @@
             'sequencing_platform': 'illumina',
         }
         self.maxDiff = None
         self.assertDictEqual(expected_sequence_dict, assay.meta)
 
     @run_as_sync
     @patch('metamist.parser.generic_parser.query_async')
+    async def test_to_external(self, mock_graphql_query):
+        """
+        Test importing a single row, forms objects and checks response
+        - MOCKS: query_async
+        """
+        mock_graphql_query.side_effect = self.run_graphql_query_async
+
+        rows = [
+            'Individual ID\tFilenames',
+            '<sample-id>\t<sample-id>.filename-R1.fastq.gz,<sample-id>.filename-R2.fastq.gz',
+        ]
+        parser = SampleFileMapParser(
+            search_locations=[],
+            project=self.project_name,
+            default_sequencing_technology='short-read',
+        )
+        fs = ['<sample-id>.filename-R1.fastq.gz', '<sample-id>.filename-R2.fastq.gz']
+        parser.filename_map = {k: 'gs://BUCKET/FAKE/' + k for k in fs}
+        parser.skip_checking_gcs_objects = True
+
+        file_contents = '\n'.join(rows)
+        participants: list[ParsedParticipant]
+        _, participants = await parser.parse_manifest(
+            StringIO(file_contents), delimiter='\t', dry_run=True
+        )
+        for p in participants:
+            p.to_sm()
+
+    @run_as_sync
+    @patch('metamist.parser.generic_parser.query_async')
     async def test_two_rows_with_provided_checksums(self, mock_graphql_query):
         """
         Test importing a single row, forms objects and checks response
         - MOCKS: get_sample_id_map_by_external, get_sequence_ids_for_sample_ids_by_type
         """
         mock_graphql_query.side_effect = self.run_graphql_query_async
```

### Comparing `metamist-6.0.2/test/test_parse_generic_metadata.py` & `metamist-6.0.3/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_parse_ont_processor.py` & `metamist-6.0.3/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_parse_ont_sheet.py` & `metamist-6.0.3/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_pedigree.py` & `metamist-6.0.3/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_sample.py` & `metamist-6.0.3/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_search.py` & `metamist-6.0.3/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_upsert.py` & `metamist-6.0.3/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.2/test/test_web.py` & `metamist-6.0.3/test/test_web.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from test.testbase import DbIsolatedTest, run_as_sync
 
+from models.enums import MetaSearchEntityPrefix
 from models.models import (
     ParticipantUpsertInternal,
     SampleUpsertInternal,
     SequencingGroupUpsertInternal,
     AssayUpsertInternal,
+    ProjectSummaryInternal,
+    AssayInternal,
+    Assay,
 )
-from db.python.layers.assay import AssayLayer
-from db.python.layers.sample import SampleLayer
-from db.python.layers.participant import ParticipantLayer
-from db.python.layers.web import (
+from models.models import WebProject, SearchItem
+from models.utils.sample_id_format import sample_id_transform_to_raw
+from models.utils.sequencing_group_id_format import sequencing_group_id_transform_to_raw
+
+from db.python.layers import (
+    AssayLayer,
+    SequencingGroupLayer,
+    SampleLayer,
+    ParticipantLayer,
     WebLayer,
-    ProjectSummary,
-    WebProject,
-    SearchItem,
-    MetaSearchEntityPrefix,
 )
 
 default_assay_meta = {
     'sequencing_type': 'genome',
     'sequencing_technology': 'short-read',
     'sequencing_platform': 'illumina',
 }
@@ -141,15 +146,15 @@
                     ),
                 ],
             )
         ],
     )
 
 
-SINGLE_PARTICIPANT_RESULT = ProjectSummary(
+SINGLE_PARTICIPANT_RESULT = ProjectSummaryInternal(
     project=WebProject(id=1, name='test', meta={}, dataset='test'),
     total_samples=1,
     total_samples_in_query=1,
     total_participants=1,
     total_sequencing_groups=1,
     total_assays=1,
     cram_seqr_stats={
@@ -195,15 +200,15 @@
 
     @run_as_sync
     async def test_project_summary_empty(self):
         """Test getting the summary for a project"""
         result = await self.webl.get_project_summary(token=0, grid_filter=[])
 
         # Expect an empty project
-        expected = ProjectSummary(
+        expected = ProjectSummaryInternal(
             project=WebProject(
                 **{'id': 1, 'name': 'test', 'meta': {}, 'dataset': 'test'}
             ),
             total_samples=0,
             total_samples_in_query=0,
             total_participants=0,
             total_sequencing_groups=0,
@@ -229,14 +234,52 @@
 
         result = await self.webl.get_project_summary(token=0, grid_filter=[])
 
         result.participants = []
         self.assertEqual(SINGLE_PARTICIPANT_RESULT, result)
 
     @run_as_sync
+    async def test_project_summary_to_external(self):
+        """Test project summary to_external function"""
+        # Now add a participant with a sample and sequence
+        await self.partl.upsert_participants(participants=[get_test_participant()])
+
+        result = await self.webl.get_project_summary(token=0, grid_filter=[])
+
+        ex_result = result.to_external(links=None)
+
+        self.assertIsInstance(result.participants[0].samples[0].id, int)
+        self.assertIsInstance(ex_result.participants[0].samples[0].id, str)
+        self.assertEqual(
+            result.participants[0].samples[0].id,
+            sample_id_transform_to_raw(ex_result.participants[0].samples[0].id),
+        )
+
+        self.assertIsInstance(
+            result.participants[0].samples[0].sequencing_groups[0].id, int
+        )
+        self.assertIsInstance(
+            ex_result.participants[0].samples[0].sequencing_groups[0].id, str
+        )
+        self.assertEqual(
+            result.participants[0].samples[0].sequencing_groups[0].id,
+            sequencing_group_id_transform_to_raw(
+                ex_result.participants[0].samples[0].sequencing_groups[0].id
+            ),
+        )
+
+        self.assertIsInstance(
+            result.participants[0].samples[0].sequencing_groups[0].assays[0],
+            AssayInternal,
+        )
+        self.assertIsInstance(
+            ex_result.participants[0].samples[0].sequencing_groups[0].assays[0], Assay
+        )
+
+    @run_as_sync
     async def project_summary_with_filter_with_results(self):
         """Project grid but with test filter, that shows results"""
         await self.partl.upsert_participants(participants=[get_test_participant()])
 
         filtered_result_success = await self.webl.get_project_summary(
             token=0,
             grid_filter=[
@@ -261,15 +304,15 @@
                     model_type=MetaSearchEntityPrefix.ASSAY,
                     query='M002',
                     field='batch',
                     is_meta=True,
                 )
             ],
         )
-        empty_result = ProjectSummary(
+        empty_result = ProjectSummaryInternal(
             project=WebProject(
                 **{'id': 1, 'name': 'test', 'meta': {}, 'dataset': 'test'}
             ),
             total_samples=0,
             total_samples_in_query=0,
             total_participants=0,
             total_sequencing_groups=0,
@@ -290,15 +333,15 @@
     @run_as_sync
     async def test_project_summary_multiple_participants(self):
         """Try with multiple participants as some extra security"""
         await self.partl.upsert_participants(
             participants=[get_test_participant(), get_test_participant_2()]
         )
 
-        expected_data_two_samples = ProjectSummary(
+        expected_data_two_samples = ProjectSummaryInternal(
             project=WebProject(id=1, name='test', meta={}, dataset='test'),
             total_samples=2,
             total_samples_in_query=2,
             total_participants=2,
             total_sequencing_groups=2,
             total_assays=2,
             cram_seqr_stats={
@@ -342,15 +385,15 @@
     @run_as_sync
     async def test_project_summary_multiple_participants_and_filter(self):
         """Try with multiple participants as some extra security"""
         await self.partl.upsert_participants(
             participants=[get_test_participant(), get_test_participant_2()]
         )
 
-        expected_data_two_samples_filtered = ProjectSummary(
+        expected_data_two_samples_filtered = ProjectSummaryInternal(
             project=WebProject(id=1, name='test', meta={}, dataset='test'),
             total_samples=2,
             total_samples_in_query=1,
             total_participants=2,
             total_sequencing_groups=2,
             total_assays=2,
             cram_seqr_stats={
@@ -419,15 +462,15 @@
                     }
                 )
             ],
         )
         self.assertEqual(1, len(test_field_with_space.participants))
         test_field_with_space.participants = []
 
-        expected_data_two_samples_filtered = ProjectSummary(
+        expected_data_two_samples_filtered = ProjectSummaryInternal(
             project=WebProject(id=1, name='test', meta={}, dataset='test'),
             total_samples=2,
             total_samples_in_query=1,
             total_participants=2,
             total_sequencing_groups=2,
             total_assays=2,
             cram_seqr_stats={
@@ -457,7 +500,31 @@
                 ('meta.reads_type', 'reads_type'),
             ],
             seqr_links={},
             seqr_sync_types=[],
         )
 
         self.assertEqual(expected_data_two_samples_filtered, test_field_with_space)
+
+    @run_as_sync
+    async def test_project_summary_inactive_sequencing_group(self):
+        """
+        Insert a sequencing-group, archive it, then check that the summary
+        doesn't return that sequencing group
+        """
+        participants = await self.partl.upsert_participants(
+            participants=[get_test_participant()]
+        )
+        sg = participants[0].samples[0].sequencing_groups[0]
+        assay_ids = [a.id for a in sg.assays]
+        sglayer = SequencingGroupLayer(self.connection)
+        new_sg_id = await sglayer.recreate_sequencing_group_with_new_assays(
+            sequencing_group_id=sg.id,
+            assays=assay_ids,
+            meta={'new-meta': 'value'},
+        )
+
+        psummary = await self.webl.get_project_summary(grid_filter=[])
+
+        summary_sgs = psummary.participants[0].samples[0].sequencing_groups
+        self.assertEqual(1, len(summary_sgs))
+        self.assertEqual(new_sg_id, summary_sgs[0].id)
```

### Comparing `metamist-6.0.2/test/testbase.py` & `metamist-6.0.3/test/testbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,18 @@
                 raise ValueError(
                     f'Invalid test query (type: {type(query)}): {query}'
                 ) from exc
 
         value = await schema.execute(
             query,
             variable_values=variables,
-            context_value=await get_context(connection=self.connection),
+            context_value=await get_context(
+                connection=self.connection,
+                request=None,   # pylint: disable
+            ),
         )
         if value.errors:
             raise value.errors[0]
         return value.data
 
 
 class DbIsolatedTest(DbTest):
```

