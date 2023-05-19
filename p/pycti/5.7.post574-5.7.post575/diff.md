# Comparing `tmp/pycti-5.7.post574.tar.gz` & `tmp/pycti-5.7.post575.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.7.post574.tar", last modified: Mon May  8 08:28:53 2023, max compression
+gzip compressed data, was "pycti-5.7.post575.tar", last modified: Fri May 19 16:30:34 2023, max compression
```

## Comparing `pycti-5.7.post574.tar` & `pycti-5.7.post575.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.747594 pycti-5.7.post574/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-08 08:28:40.000000 pycti-5.7.post574/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-08 08:28:53.747594 pycti-5.7.post574/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3141 2023-05-08 08:28:40.000000 pycti-5.7.post574/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28104 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42485 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.747594 pycti-5.7.post574/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24396 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23837 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23845 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24602 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12155 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22661 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20977 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32054 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    63935 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.747594 pycti-5.7.post574/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3308 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   101676 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2250 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-08 08:28:40.000000 pycti-5.7.post574/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-05-08 08:28:53.751594 pycti-5.7.post574/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.303959 pycti-5.7.post575/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-19 16:30:20.000000 pycti-5.7.post575/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4093 2023-05-19 16:30:34.303959 pycti-5.7.post575/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-05-19 16:30:20.000000 pycti-5.7.post575/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.295959 pycti-5.7.post575/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-19 16:30:20.000000 pycti-5.7.post575/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.295959 pycti-5.7.post575/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-19 16:30:20.000000 pycti-5.7.post575/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28212 2023-05-19 16:30:20.000000 pycti-5.7.post575/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-05-19 16:30:20.000000 pycti-5.7.post575/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-05-19 16:30:20.000000 pycti-5.7.post575/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.295959 pycti-5.7.post575/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42775 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.303959 pycti-5.7.post575/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24396 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23837 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23845 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24602 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12155 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22661 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20977 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32054 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64475 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.303959 pycti-5.7.post575/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3308 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   101676 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-05-19 16:30:21.000000 pycti-5.7.post575/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-19 16:30:34.295959 pycti-5.7.post575/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4093 2023-05-19 16:30:34.000000 pycti-5.7.post575/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2250 2023-05-19 16:30:34.000000 pycti-5.7.post575/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-19 16:30:34.000000 pycti-5.7.post575/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-05-19 16:30:34.000000 pycti-5.7.post575/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-19 16:30:34.000000 pycti-5.7.post575/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-19 16:30:21.000000 pycti-5.7.post575/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-05-19 16:30:34.303959 pycti-5.7.post575/setup.cfg
```

### Comparing `pycti-5.7.post574/LICENSE` & `pycti-5.7.post575/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/PKG-INFO` & `pycti-5.7.post575/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.7.post574
+Version: 5.7.post575
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,15 +97,15 @@
 [pytest](https://docs.pytest.org/en/7.2.x/) is used to launch the tests.
 
 ### Launch tests
 
 #### Prerequisite
 
 Your OpenCTI API should be running.
-Your conftest.py should be configured with your API url and your token.
+Your conftest.py should be configured with your API url, your token, and if applicable, your mTLS cert/key.
 
 #### Launching
 
 Unit tests
 ```bash
 $ pytest ./tests/01-unit/
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.7.post574 Summary: Python API
+Metadata-Version: 2.1 Name: pycti Version: 5.7.post575 Summary: Python API
 client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
 python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
 License: Apache Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Natural Language :: French Classifier:
@@ -41,12 +41,13 @@
 latest/client_usage/getting_started.html). ### API reference To learn about the
 methods available for executing queries and retrieving their answers, refer to
 [the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
 latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
 install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
 7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
 OpenCTI API should be running. Your conftest.py should be configured with your
-API url and your token. #### Launching Unit tests ```bash $ pytest ./tests/01-
-unit/ ``` Integration testing ```bash $ pytest ./tests/02-integration/ ``` ##
-About OpenCTI is a product designed and developed by the company [Filigran]
-(https://www.filigran.io). [https://www.filigran.io/wp-content/uploads/2022/08/
+API url, your token, and if applicable, your mTLS cert/key. #### Launching Unit
+tests ```bash $ pytest ./tests/01-unit/ ``` Integration testing ```bash $
+pytest ./tests/02-integration/ ``` ## About OpenCTI is a product designed and
+developed by the company [Filigran](https://www.filigran.io). [https://
+www.filigran.io/wp-content/uploads/2022/08/
 filigran_text_horizontal_dense_margin.png]
```

### Comparing `pycti-5.7.post574/README.md` & `pycti-5.7.post575/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 [pytest](https://docs.pytest.org/en/7.2.x/) is used to launch the tests.
 
 ### Launch tests
 
 #### Prerequisite
 
 Your OpenCTI API should be running.
-Your conftest.py should be configured with your API url and your token.
+Your conftest.py should be configured with your API url, your token, and if applicable, your mTLS cert/key.
 
 #### Launching
 
 Unit tests
 ```bash
 $ pytest ./tests/01-unit/
 ```
```

#### html2text {}

```diff
@@ -29,12 +29,13 @@
 latest/client_usage/getting_started.html). ### API reference To learn about the
 methods available for executing queries and retrieving their answers, refer to
 [the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
 latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
 install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
 7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
 OpenCTI API should be running. Your conftest.py should be configured with your
-API url and your token. #### Launching Unit tests ```bash $ pytest ./tests/01-
-unit/ ``` Integration testing ```bash $ pytest ./tests/02-integration/ ``` ##
-About OpenCTI is a product designed and developed by the company [Filigran]
-(https://www.filigran.io). [https://www.filigran.io/wp-content/uploads/2022/08/
+API url, your token, and if applicable, your mTLS cert/key. #### Launching Unit
+tests ```bash $ pytest ./tests/01-unit/ ``` Integration testing ```bash $
+pytest ./tests/02-integration/ ``` ## About OpenCTI is a product designed and
+developed by the company [Filigran](https://www.filigran.io). [https://
+www.filigran.io/wp-content/uploads/2022/08/
 filigran_text_horizontal_dense_margin.png]
```

### Comparing `pycti-5.7.post574/pycti/__init__.py` & `pycti-5.7.post575/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.7.post574"
+__version__ = "5.7.post575"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.7.post574/pycti/api/opencti_api_client.py` & `pycti-5.7.post575/pycti/api/opencti_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,19 +113,21 @@
         self,
         url,
         token,
         log_level="info",
         ssl_verify=False,
         proxies=None,
         json_logging=False,
+        cert=None,
     ):
         """Constructor method"""
 
         # Check configuration
         self.ssl_verify = ssl_verify
+        self.cert = cert
         self.proxies = proxies
         if url is None or len(url) == 0:
             raise ValueError("An URL must be set")
         if token is None or len(token) == 0 or token == "ChangeMe":
             raise ValueError("A TOKEN must be set")
 
         # Configure logger
@@ -311,23 +313,25 @@
             # Send the multipart request
             r = self.session.post(
                 self.api_url,
                 data=multipart_data,
                 files=multipart_files,
                 headers=self.request_headers,
                 verify=self.ssl_verify,
+                cert=self.cert,
                 proxies=self.proxies,
             )
         # If no
         else:
             r = self.session.post(
                 self.api_url,
                 json={"query": query, "variables": variables},
                 headers=self.request_headers,
                 verify=self.ssl_verify,
+                cert=self.cert,
                 proxies=self.proxies,
             )
         # Build response
         if r.status_code == 200:
             result = r.json()
             if "errors" in result:
                 main_error = result["errors"][0]
```

### Comparing `pycti-5.7.post574/pycti/api/opencti_api_connector.py` & `pycti-5.7.post575/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/api/opencti_api_work.py` & `pycti-5.7.post575/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/connector/opencti_connector.py` & `pycti-5.7.post575/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/connector/opencti_connector_helper.py` & `pycti-5.7.post575/pycti/connector/opencti_connector_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,22 +636,29 @@
         #     self.listen_stream.stop()
         self.ping.stop()
         self.api.connector.unregister(self.connector_id)
 
     def get_name(self) -> Optional[Union[bool, int, str]]:
         return self.connect_name
 
-    def get_stream_name(self):
+    def get_stream_collection(self):
         if self.connect_live_stream_id is not None:
             if self.connect_live_stream_id in ["live", "raw"]:
-                return self.connect_live_stream_id
+                return {
+                    "id": self.connect_live_stream_id,
+                    "name": self.connect_live_stream_id,
+                    "description": self.connect_live_stream_id,
+                    "stream_live": True,
+                    "stream_public": False,
+                }
             else:
                 query = """
                     query StreamCollection($id: String!) {
                         streamCollection(id: $id)  {
+                            id
                             name
                             description
                             stream_live
                             stream_public
                         }
                     }
                 """
```

### Comparing `pycti-5.7.post574/pycti/entities/opencti_attack_pattern.py` & `pycti-5.7.post575/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_campaign.py` & `pycti-5.7.post575/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_case_incident.py` & `pycti-5.7.post575/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_case_rfi.py` & `pycti-5.7.post575/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_case_rft.py` & `pycti-5.7.post575/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_channel.py` & `pycti-5.7.post575/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_course_of_action.py` & `pycti-5.7.post575/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_data_component.py` & `pycti-5.7.post575/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_data_source.py` & `pycti-5.7.post575/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_event.py` & `pycti-5.7.post575/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_external_reference.py` & `pycti-5.7.post575/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_feedback.py` & `pycti-5.7.post575/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_grouping.py` & `pycti-5.7.post575/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_identity.py` & `pycti-5.7.post575/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_incident.py` & `pycti-5.7.post575/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_indicator.py` & `pycti-5.7.post575/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_infrastructure.py` & `pycti-5.7.post575/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_intrusion_set.py` & `pycti-5.7.post575/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.7.post575/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_label.py` & `pycti-5.7.post575/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_language.py` & `pycti-5.7.post575/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_location.py` & `pycti-5.7.post575/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_malware.py` & `pycti-5.7.post575/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_marking_definition.py` & `pycti-5.7.post575/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_narrative.py` & `pycti-5.7.post575/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_note.py` & `pycti-5.7.post575/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_observed_data.py` & `pycti-5.7.post575/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_opinion.py` & `pycti-5.7.post575/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_report.py` & `pycti-5.7.post575/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix.py` & `pycti-5.7.post575/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_core_object.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_domain_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,19 +149,21 @@
                 note_types
                 likelihood
                 objects {
                     edges {
                         node {
                             ... on BasicObject {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                             ... on BasicRelationship {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
             }
@@ -170,19 +172,21 @@
                 last_observed
                 number_observed
                 objects {
                     edges {
                         node {
                             ... on BasicObject {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                             ... on BasicRelationship {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
             }
@@ -191,19 +195,21 @@
                 authors
                 opinion
                 objects {
                     edges {
                         node {
                             ... on BasicObject {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                             ... on BasicRelationship {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
             }
@@ -213,19 +219,21 @@
                 report_types
                 published
                 objects {
                     edges {
                         node {
                             ... on BasicObject {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                             ... on BasicRelationship {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
             }
@@ -234,19 +242,21 @@
                 description
                 context
                 objects {
                     edges {
                         node {
                             ... on BasicObject {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                             ... on BasicRelationship {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
             }
@@ -467,19 +477,21 @@
                 name
                 description
                 objects {
                     edges {
                         node {
                             ... on BasicObject {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                             ... on BasicRelationship {
                                 id
+                                parent_types
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
             }
```

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.7.post575/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_threat_actor.py` & `pycti-5.7.post575/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_tool.py` & `pycti-5.7.post575/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_vocabulary.py` & `pycti-5.7.post575/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/entities/opencti_vulnerability.py` & `pycti-5.7.post575/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/utils/constants.py` & `pycti-5.7.post575/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/utils/opencti_stix2.py` & `pycti-5.7.post575/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.7.post575/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/utils/opencti_stix2_update.py` & `pycti-5.7.post575/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti/utils/opencti_stix2_utils.py` & `pycti-5.7.post575/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti.egg-info/PKG-INFO` & `pycti-5.7.post575/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.7.post574
+Version: 5.7.post575
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -97,15 +97,15 @@
 [pytest](https://docs.pytest.org/en/7.2.x/) is used to launch the tests.
 
 ### Launch tests
 
 #### Prerequisite
 
 Your OpenCTI API should be running.
-Your conftest.py should be configured with your API url and your token.
+Your conftest.py should be configured with your API url, your token, and if applicable, your mTLS cert/key.
 
 #### Launching
 
 Unit tests
 ```bash
 $ pytest ./tests/01-unit/
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.7.post574 Summary: Python API
+Metadata-Version: 2.1 Name: pycti Version: 5.7.post575 Summary: Python API
 client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
 python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
 License: Apache Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Natural Language :: French Classifier:
@@ -41,12 +41,13 @@
 latest/client_usage/getting_started.html). ### API reference To learn about the
 methods available for executing queries and retrieving their answers, refer to
 [the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
 latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
 install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
 7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
 OpenCTI API should be running. Your conftest.py should be configured with your
-API url and your token. #### Launching Unit tests ```bash $ pytest ./tests/01-
-unit/ ``` Integration testing ```bash $ pytest ./tests/02-integration/ ``` ##
-About OpenCTI is a product designed and developed by the company [Filigran]
-(https://www.filigran.io). [https://www.filigran.io/wp-content/uploads/2022/08/
+API url, your token, and if applicable, your mTLS cert/key. #### Launching Unit
+tests ```bash $ pytest ./tests/01-unit/ ``` Integration testing ```bash $
+pytest ./tests/02-integration/ ``` ## About OpenCTI is a product designed and
+developed by the company [Filigran](https://www.filigran.io). [https://
+www.filigran.io/wp-content/uploads/2022/08/
 filigran_text_horizontal_dense_margin.png]
```

### Comparing `pycti-5.7.post574/pycti.egg-info/SOURCES.txt` & `pycti-5.7.post575/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pycti.egg-info/requires.txt` & `pycti-5.7.post575/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/pyproject.toml` & `pycti-5.7.post575/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post574/setup.cfg` & `pycti-5.7.post575/setup.cfg`

 * *Files identical despite different names*

