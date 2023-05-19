# Comparing `tmp/azure-mgmt-eventgrid-8.0.0b1.zip` & `tmp/azure-mgmt-eventgrid-9.0.0.zip`

## zipinfo {}

```diff
@@ -1,63 +1,80 @@
-Zip file size: 123334 bytes, number of entries: 61
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/
--rw-r--r--  2.0 unx    20423 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/PKG-INFO
--rw-r--r--  2.0 unx      107 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/MANIFEST.in
--rw-r--r--  2.0 unx    15248 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/CHANGELOG.md
--rw-r--r--  2.0 unx     3033 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/setup.py
--rw-r--r--  2.0 unx     1180 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/README.md
--rw-r--r--  2.0 unx       67 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/setup.cfg
--rw-r--r--  2.0 unx        1 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx    20423 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      104 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/requires.txt
--rw-r--r--  2.0 unx     2347 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/not-zip-safe
--rw-r--r--  2.0 unx        6 b- defN 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/top_level.txt
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/tests/recordings/
--rw-r--r--  2.0 unx     8047 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/test_azure_mgmt_eventgrid.py
--rw-r--r--  2.0 unx     1655 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/test_domain.py
--rw-r--r--  2.0 unx    15208 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_user_topics.yaml
--rw-r--r--  2.0 unx    14286 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_domain.test_domain.yaml
--rw-r--r--  2.0 unx    16752 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_input_mappings_and_queue_destination.yaml
--rw-r--r--  2.0 unx     7899 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_topic_types.yaml
--rw-r--r--  2.0 unx    15612 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_domains_and_advanced_filter.yaml
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/
--rw-r--r--  2.0 unx       64 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/
--rw-r--r--  2.0 unx       64 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/
--rw-r--r--  2.0 unx      731 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/__init__.py
--rw-r--r--  2.0 unx     5119 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_event_grid_management_client.py
--rw-r--r--  2.0 unx     3389 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_configuration.py
--rw-r--r--  2.0 unx      488 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_version.py
--rw-r--r--  2.0 unx    10712 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/__init__.py
--rw-r--r--  2.0 unx    92770 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_models_py3.py
--rw-r--r--  2.0 unx     6526 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_event_grid_management_client_enums.py
--rw-r--r--  2.0 unx    86817 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_models.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-18 06:45 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/
--rw-r--r--  2.0 unx      577 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/__init__.py
--rw-r--r--  2.0 unx     5096 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/_event_grid_management_client.py
--rw-r--r--  2.0 unx     3333 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/_configuration.py
--rw-r--r--  2.0 unx    10657 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_private_link_resources_operations.py
--rw-r--r--  2.0 unx     1226 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/__init__.py
--rw-r--r--  2.0 unx    10112 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_topic_types_operations.py
--rw-r--r--  2.0 unx     4692 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_operations.py
--rw-r--r--  2.0 unx    36472 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_domains_operations.py
--rw-r--r--  2.0 unx    24406 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_private_endpoint_connections_operations.py
--rw-r--r--  2.0 unx    20541 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_domain_topics_operations.py
--rw-r--r--  2.0 unx    77616 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_event_subscriptions_operations.py
--rw-r--r--  2.0 unx    40477 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_topics_operations.py
--rw-r--r--  2.0 unx    10813 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_private_link_resources_operations.py
--rw-r--r--  2.0 unx     1226 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/__init__.py
--rw-r--r--  2.0 unx    10207 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_topic_types_operations.py
--rw-r--r--  2.0 unx     4757 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_operations.py
--rw-r--r--  2.0 unx    36790 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_domains_operations.py
--rw-r--r--  2.0 unx    24682 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_private_endpoint_connections_operations.py
--rw-r--r--  2.0 unx    20753 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_domain_topics_operations.py
--rw-r--r--  2.0 unx    78055 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_event_subscriptions_operations.py
--rw-r--r--  2.0 unx    40818 b- defN 20-Nov-18 06:44 azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_topics_operations.py
-61 files, 812385 bytes uncompressed, 110100 bytes compressed:  86.4%
+Zip file size: 207206 bytes, number of entries: 78
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/
+-rw-rw-r--  2.0 unx     1180 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/README.md
+-rw-rw-r--  2.0 unx      578 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/_meta.json
+-rw-rw-r--  2.0 unx       67 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/setup.cfg
+-rw-rw-r--  2.0 unx      126 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/MANIFEST.in
+-rw-rw-r--  2.0 unx    23654 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/PKG-INFO
+-rw-rw-r--  2.0 unx     3034 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/setup.py
+-rw-rw-r--  2.0 unx    18057 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx      105 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        1 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx     3480 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        6 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    23654 b- defN 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/PKG-INFO
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/tests/recordings/
+-rw-rw-r--  2.0 unx     1655 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/test_domain.py
+-rw-rw-r--  2.0 unx     8047 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/test_azure_mgmt_eventgrid.py
+-rw-rw-r--  2.0 unx    15073 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/recordings/test_domain.test_domain.yaml
+-rw-rw-r--  2.0 unx    16752 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_input_mappings_and_queue_destination.yaml
+-rw-rw-r--  2.0 unx    15208 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_user_topics.yaml
+-rw-rw-r--  2.0 unx     7899 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_topic_types.yaml
+-rw-rw-r--  2.0 unx    15612 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_domains_and_advanced_filter.yaml
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/mgmt/
+-rw-rw-r--  2.0 unx       64 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/
+-rw-rw-r--  2.0 unx       64 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/
+-rw-rw-r--  2.0 unx     9154 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_event_grid_management_client.py
+-rw-rw-r--  2.0 unx      486 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_version.py
+-rw-rw-r--  2.0 unx     3397 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_configuration.py
+-rw-rw-r--  2.0 unx      731 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/__init__.py
+-rw-rw-r--  2.0 unx   171818 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_models_py3.py
+-rw-rw-r--  2.0 unx   160325 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_models.py
+-rw-rw-r--  2.0 unx    18102 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/__init__.py
+-rw-rw-r--  2.0 unx    11110 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_event_grid_management_client_enums.py
+-rw-rw-r--  2.0 unx    20000 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_event_channels_operations.py
+-rw-rw-r--  2.0 unx     4779 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_operations.py
+-rw-rw-r--  2.0 unx    40073 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_namespaces_operations.py
+-rw-rw-r--  2.0 unx    27310 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_registrations_operations.py
+-rw-rw-r--  2.0 unx    28793 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_topics_operations.py
+-rw-rw-r--  2.0 unx    10249 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_topic_types_operations.py
+-rw-rw-r--  2.0 unx     2125 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/__init__.py
+-rw-rw-r--  2.0 unx    82819 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_event_subscriptions_operations.py
+-rw-rw-r--  2.0 unx    38782 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_topic_event_subscriptions_operations.py
+-rw-rw-r--  2.0 unx    21972 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_domain_topics_operations.py
+-rw-rw-r--  2.0 unx    38616 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_system_topic_event_subscriptions_operations.py
+-rw-rw-r--  2.0 unx    26156 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx    10845 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    38372 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_domains_operations.py
+-rw-rw-r--  2.0 unx     4771 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_extension_topics_operations.py
+-rw-rw-r--  2.0 unx    32934 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_system_topics_operations.py
+-rw-rw-r--  2.0 unx    45610 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_topics_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-May-24 08:39 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/
+-rw-rw-r--  2.0 unx     9169 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/_event_grid_management_client.py
+-rw-rw-r--  2.0 unx     3341 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/_configuration.py
+-rw-rw-r--  2.0 unx      577 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/__init__.py
+-rw-rw-r--  2.0 unx    19812 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_event_channels_operations.py
+-rw-rw-r--  2.0 unx     4719 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    39825 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_namespaces_operations.py
+-rw-rw-r--  2.0 unx    27094 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_registrations_operations.py
+-rw-rw-r--  2.0 unx    28579 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_topics_operations.py
+-rw-rw-r--  2.0 unx    10169 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_topic_types_operations.py
+-rw-rw-r--  2.0 unx     2125 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    82451 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_event_subscriptions_operations.py
+-rw-rw-r--  2.0 unx    38460 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_topic_event_subscriptions_operations.py
+-rw-rw-r--  2.0 unx    21800 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_domain_topics_operations.py
+-rw-rw-r--  2.0 unx    38294 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_system_topic_event_subscriptions_operations.py
+-rw-rw-r--  2.0 unx    25920 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx    10699 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    38124 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_domains_operations.py
+-rw-rw-r--  2.0 unx     4644 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_extension_topics_operations.py
+-rw-rw-r--  2.0 unx    32762 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_system_topics_operations.py
+-rw-rw-r--  2.0 unx    45352 b- defN 21-May-24 08:37 azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_topics_operations.py
+78 files, 1487562 bytes uncompressed, 189774 bytes compressed:  87.2%
```

## zipnote {}

```diff
@@ -1,184 +1,235 @@
-Filename: azure-mgmt-eventgrid-8.0.0b1/
+Filename: azure-mgmt-eventgrid-9.0.0/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/
+Filename: azure-mgmt-eventgrid-9.0.0/tests/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/
+Filename: azure-mgmt-eventgrid-9.0.0/azure/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/PKG-INFO
+Filename: azure-mgmt-eventgrid-9.0.0/README.md
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/MANIFEST.in
+Filename: azure-mgmt-eventgrid-9.0.0/_meta.json
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/CHANGELOG.md
+Filename: azure-mgmt-eventgrid-9.0.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/setup.py
+Filename: azure-mgmt-eventgrid-9.0.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/README.md
+Filename: azure-mgmt-eventgrid-9.0.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/setup.cfg
+Filename: azure-mgmt-eventgrid-9.0.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/dependency_links.txt
+Filename: azure-mgmt-eventgrid-9.0.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/PKG-INFO
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/requires.txt
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/SOURCES.txt
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/not-zip-safe
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/top_level.txt
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/recordings/
+Filename: azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/test_azure_mgmt_eventgrid.py
+Filename: azure-mgmt-eventgrid-9.0.0/tests/recordings/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/test_domain.py
+Filename: azure-mgmt-eventgrid-9.0.0/tests/test_domain.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_user_topics.yaml
+Filename: azure-mgmt-eventgrid-9.0.0/tests/test_azure_mgmt_eventgrid.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_domain.test_domain.yaml
+Filename: azure-mgmt-eventgrid-9.0.0/tests/recordings/test_domain.test_domain.yaml
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_input_mappings_and_queue_destination.yaml
+Filename: azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_input_mappings_and_queue_destination.yaml
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_topic_types.yaml
+Filename: azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_user_topics.yaml
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_domains_and_advanced_filter.yaml
+Filename: azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_topic_types.yaml
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/
+Filename: azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_domains_and_advanced_filter.yaml
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/
+Filename: azure-mgmt-eventgrid-9.0.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_event_grid_management_client.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_event_grid_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_configuration.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_version.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_version.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_models_py3.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_event_grid_management_client_enums.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_models.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_event_grid_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_event_channels_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/_event_grid_management_client.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/_configuration.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_registrations_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_topics_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_topic_types_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_topic_types_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_domains_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_event_subscriptions_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_partner_topic_event_subscriptions_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_domain_topics_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_domain_topics_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_event_subscriptions_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_system_topic_event_subscriptions_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_topics_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/__init__.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_domains_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_topic_types_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_extension_topics_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_system_topics_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_domains_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_topics_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_domain_topics_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/_event_grid_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_event_subscriptions_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_topics_operations.py
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_event_channels_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_namespaces_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_registrations_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_topics_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_topic_types_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_event_subscriptions_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_partner_topic_event_subscriptions_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_domain_topics_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_system_topic_event_subscriptions_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_private_endpoint_connections_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_private_link_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_domains_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_extension_topics_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_system_topics_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_topics_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/PKG-INFO` & `azure-mgmt-eventgrid-9.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-eventgrid
-Version: 8.0.0b1
+Version: 9.0.0
 Summary: Microsoft Azure EventGrid Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -32,14 +32,67 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-eventgrid%2FREADME.png)
         
         
         # Release History
         
+        ## 9.0.0 (2021-05-24)
+        
+        **Features**
+        
+          - Model EventHubEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model StorageQueueEventSubscriptionDestination has a new parameter queue_message_time_to_live_in_seconds
+          - Model TopicTypeInfo has a new parameter supported_scopes_for_source
+          - Model Topic has a new parameter extended_location
+          - Model Topic has a new parameter kind
+          - Model Topic has a new parameter system_data
+          - Model Topic has a new parameter identity
+          - Model Topic has a new parameter sku
+          - Model EventSubscriptionFilter has a new parameter enable_advanced_filtering_on_arrays
+          - Model AzureFunctionEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model EventSubscriptionUpdateParameters has a new parameter dead_letter_with_resource_identity
+          - Model EventSubscriptionUpdateParameters has a new parameter delivery_with_resource_identity
+          - Model ServiceBusQueueEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model DomainTopic has a new parameter system_data
+          - Model DomainUpdateParameters has a new parameter sku
+          - Model DomainUpdateParameters has a new parameter identity
+          - Model HybridConnectionEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model TopicUpdateParameters has a new parameter sku
+          - Model TopicUpdateParameters has a new parameter identity
+          - Model ServiceBusTopicEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model Domain has a new parameter sku
+          - Model Domain has a new parameter system_data
+          - Model Domain has a new parameter identity
+          - Model EventSubscription has a new parameter dead_letter_with_resource_identity
+          - Model EventSubscription has a new parameter system_data
+          - Model EventSubscription has a new parameter delivery_with_resource_identity
+          - Model WebHookEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Added operation TopicsOperations.begin_regenerate_key
+          - Added operation EventSubscriptionsOperations.get_delivery_attributes
+          - Added operation group PartnerRegistrationsOperations
+          - Added operation group SystemTopicsOperations
+          - Added operation group EventChannelsOperations
+          - Added operation group PartnerNamespacesOperations
+          - Added operation group ExtensionTopicsOperations
+          - Added operation group PartnerTopicsOperations
+          - Added operation group PartnerTopicEventSubscriptionsOperations
+          - Added operation group SystemTopicEventSubscriptionsOperations
+        
+        **Breaking changes**
+        
+          - Removed operation TopicsOperations.regenerate_key
+        
+        ## 8.0.0 (2020-12-21)
+        
+        **Breaking changes**
+        
+          - Operation TopicsOperations.regenerate_key has a new signature
+          - Operation DomainsOperations.regenerate_key has a new signature
+        
         ## 8.0.0b1 (2020-10-31)
         
         This is beta preview version.
         For detailed changelog please refer to equivalent stable version 3.0.0rc8(https://pypi.org/project/azure-mgmt-eventgrid/3.0.0rc8/)
         
         This version uses a next-generation code generator that introduces important breaking changes, but also important new features (like unified authentication and async programming).
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/CHANGELOG.md` & `azure-mgmt-eventgrid-9.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,62 @@
 # Release History
 
+## 9.0.0 (2021-05-24)
+
+**Features**
+
+  - Model EventHubEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+  - Model StorageQueueEventSubscriptionDestination has a new parameter queue_message_time_to_live_in_seconds
+  - Model TopicTypeInfo has a new parameter supported_scopes_for_source
+  - Model Topic has a new parameter extended_location
+  - Model Topic has a new parameter kind
+  - Model Topic has a new parameter system_data
+  - Model Topic has a new parameter identity
+  - Model Topic has a new parameter sku
+  - Model EventSubscriptionFilter has a new parameter enable_advanced_filtering_on_arrays
+  - Model AzureFunctionEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+  - Model EventSubscriptionUpdateParameters has a new parameter dead_letter_with_resource_identity
+  - Model EventSubscriptionUpdateParameters has a new parameter delivery_with_resource_identity
+  - Model ServiceBusQueueEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+  - Model DomainTopic has a new parameter system_data
+  - Model DomainUpdateParameters has a new parameter sku
+  - Model DomainUpdateParameters has a new parameter identity
+  - Model HybridConnectionEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+  - Model TopicUpdateParameters has a new parameter sku
+  - Model TopicUpdateParameters has a new parameter identity
+  - Model ServiceBusTopicEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+  - Model Domain has a new parameter sku
+  - Model Domain has a new parameter system_data
+  - Model Domain has a new parameter identity
+  - Model EventSubscription has a new parameter dead_letter_with_resource_identity
+  - Model EventSubscription has a new parameter system_data
+  - Model EventSubscription has a new parameter delivery_with_resource_identity
+  - Model WebHookEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+  - Added operation TopicsOperations.begin_regenerate_key
+  - Added operation EventSubscriptionsOperations.get_delivery_attributes
+  - Added operation group PartnerRegistrationsOperations
+  - Added operation group SystemTopicsOperations
+  - Added operation group EventChannelsOperations
+  - Added operation group PartnerNamespacesOperations
+  - Added operation group ExtensionTopicsOperations
+  - Added operation group PartnerTopicsOperations
+  - Added operation group PartnerTopicEventSubscriptionsOperations
+  - Added operation group SystemTopicEventSubscriptionsOperations
+
+**Breaking changes**
+
+  - Removed operation TopicsOperations.regenerate_key
+
+## 8.0.0 (2020-12-21)
+
+**Breaking changes**
+
+  - Operation TopicsOperations.regenerate_key has a new signature
+  - Operation DomainsOperations.regenerate_key has a new signature
+
 ## 8.0.0b1 (2020-10-31)
 
 This is beta preview version.
 For detailed changelog please refer to equivalent stable version 3.0.0rc8(https://pypi.org/project/azure-mgmt-eventgrid/3.0.0rc8/)
 
 This version uses a next-generation code generator that introduces important breaking changes, but also important new features (like unified authentication and async programming).
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/setup.py` & `azure-mgmt-eventgrid-9.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     packages=find_packages(exclude=[
         'tests',
         # Exclude packages that will be covered by PEP420 or nspkg
         'azure',
         'azure.mgmt',
     ]),
     install_requires=[
-        'msrest>=0.5.0',
+        'msrest>=0.6.21',
         'azure-common~=1.1',
         'azure-mgmt-core>=1.2.0,<2.0.0'
     ],
     extras_require={
         ":python_version<'3.0'": ['azure-mgmt-nspkg'],
     }
 )
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/README.md` & `azure-mgmt-eventgrid-9.0.0/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure_mgmt_eventgrid.egg-info/PKG-INFO` & `azure-mgmt-eventgrid-9.0.0/azure_mgmt_eventgrid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-eventgrid
-Version: 8.0.0b1
+Version: 9.0.0
 Summary: Microsoft Azure EventGrid Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -32,14 +32,67 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-eventgrid%2FREADME.png)
         
         
         # Release History
         
+        ## 9.0.0 (2021-05-24)
+        
+        **Features**
+        
+          - Model EventHubEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model StorageQueueEventSubscriptionDestination has a new parameter queue_message_time_to_live_in_seconds
+          - Model TopicTypeInfo has a new parameter supported_scopes_for_source
+          - Model Topic has a new parameter extended_location
+          - Model Topic has a new parameter kind
+          - Model Topic has a new parameter system_data
+          - Model Topic has a new parameter identity
+          - Model Topic has a new parameter sku
+          - Model EventSubscriptionFilter has a new parameter enable_advanced_filtering_on_arrays
+          - Model AzureFunctionEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model EventSubscriptionUpdateParameters has a new parameter dead_letter_with_resource_identity
+          - Model EventSubscriptionUpdateParameters has a new parameter delivery_with_resource_identity
+          - Model ServiceBusQueueEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model DomainTopic has a new parameter system_data
+          - Model DomainUpdateParameters has a new parameter sku
+          - Model DomainUpdateParameters has a new parameter identity
+          - Model HybridConnectionEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model TopicUpdateParameters has a new parameter sku
+          - Model TopicUpdateParameters has a new parameter identity
+          - Model ServiceBusTopicEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Model Domain has a new parameter sku
+          - Model Domain has a new parameter system_data
+          - Model Domain has a new parameter identity
+          - Model EventSubscription has a new parameter dead_letter_with_resource_identity
+          - Model EventSubscription has a new parameter system_data
+          - Model EventSubscription has a new parameter delivery_with_resource_identity
+          - Model WebHookEventSubscriptionDestination has a new parameter delivery_attribute_mappings
+          - Added operation TopicsOperations.begin_regenerate_key
+          - Added operation EventSubscriptionsOperations.get_delivery_attributes
+          - Added operation group PartnerRegistrationsOperations
+          - Added operation group SystemTopicsOperations
+          - Added operation group EventChannelsOperations
+          - Added operation group PartnerNamespacesOperations
+          - Added operation group ExtensionTopicsOperations
+          - Added operation group PartnerTopicsOperations
+          - Added operation group PartnerTopicEventSubscriptionsOperations
+          - Added operation group SystemTopicEventSubscriptionsOperations
+        
+        **Breaking changes**
+        
+          - Removed operation TopicsOperations.regenerate_key
+        
+        ## 8.0.0 (2020-12-21)
+        
+        **Breaking changes**
+        
+          - Operation TopicsOperations.regenerate_key has a new signature
+          - Operation DomainsOperations.regenerate_key has a new signature
+        
         ## 8.0.0b1 (2020-10-31)
         
         This is beta preview version.
         For detailed changelog please refer to equivalent stable version 3.0.0rc8(https://pypi.org/project/azure-mgmt-eventgrid/3.0.0rc8/)
         
         This version uses a next-generation code generator that introduces important breaking changes, but also important new features (like unified authentication and async programming).
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/test_azure_mgmt_eventgrid.py` & `azure-mgmt-eventgrid-9.0.0/tests/test_azure_mgmt_eventgrid.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/test_domain.py` & `azure-mgmt-eventgrid-9.0.0/tests/test_domain.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_user_topics.yaml` & `azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_user_topics.yaml`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_domain.test_domain.yaml` & `azure-mgmt-eventgrid-9.0.0/tests/recordings/test_domain.test_domain.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -9,71 +9,73 @@
       Connection:
       - keep-alive
       Content-Length:
       - '22'
       Content-Type:
       - application/json
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: PUT
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"properties":{"provisioningState":"Creating","endpoint":null},"location":"westus","tags":null,"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
+      string: '{"properties":{"provisioningState":"Creating","endpoint":null},"systemData":null,"location":"westus","tags":null,"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
     headers:
       azure-asyncoperation:
-      - https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/D703D5E6-7C9C-4312-BBAF-1F33B063F75F?api-version=2020-06-01
+      - https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/24594E47-8207-4964-8122-2D7A9332BE45?api-version=2020-10-15-preview
       cache-control:
       - no-cache
       content-length:
-      - '315'
+      - '338'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:15 GMT
+      - Mon, 24 May 2021 06:40:40 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1198'
+      - '1199'
     status:
       code: 201
       message: Created
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/D703D5E6-7C9C-4312-BBAF-1F33B063F75F?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/24594E47-8207-4964-8122-2D7A9332BE45?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"id":"https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/D703D5E6-7C9C-4312-BBAF-1F33B063F75F?api-version=2020-06-01","name":"d703d5e6-7c9c-4312-bbaf-1f33b063f75f","status":"Succeeded"}'
+      string: '{"id":"https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/24594E47-8207-4964-8122-2D7A9332BE45?api-version=2020-10-15-preview","name":"24594e47-8207-4964-8122-2d7a9332be45","status":"Succeeded"}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '279'
+      - '287'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:26 GMT
+      - Mon, 24 May 2021 06:40:51 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -93,29 +95,30 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"properties":{"provisioningState":"Succeeded","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"e81b8a8f-987e-47c5-b59f-34d73872a8ed","publicNetworkAccess":"Enabled"},"location":"westus","tags":null,"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
+      string: '{"properties":{"provisioningState":"Succeeded","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"f9a9f07a-0f80-4980-8b8b-fac9e67ca89a","publicNetworkAccess":"Enabled"},"sku":{"name":"Basic"},"systemData":null,"location":"westus","tags":null,"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '498'
+      - '544'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:26 GMT
+      - Mon, 24 May 2021 06:40:51 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -139,71 +142,73 @@
       Connection:
       - keep-alive
       Content-Length:
       - '46'
       Content-Type:
       - application/json
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: PATCH
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"properties":{"provisioningState":"Updating","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"e81b8a8f-987e-47c5-b59f-34d73872a8ed","publicNetworkAccess":"Enabled"},"location":"westus","tags":{"tag1":"value1","tag2":"value2"},"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
+      string: '{"properties":{"provisioningState":"Updating","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"f9a9f07a-0f80-4980-8b8b-fac9e67ca89a","publicNetworkAccess":"Enabled"},"sku":{"name":"Basic"},"systemData":null,"location":"westus","tags":{"tag1":"value1","tag2":"value2"},"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
     headers:
       azure-asyncoperation:
-      - https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/E671AD99-24A2-4CD0-A891-1E688BBA525D?api-version=2020-06-01
+      - https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/874FEC44-25EB-4C80-B37F-6E986B8B8221?api-version=2020-10-15-preview
       cache-control:
       - no-cache
       content-length:
-      - '526'
+      - '572'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:29 GMT
+      - Mon, 24 May 2021 06:40:53 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-writes:
-      - '1197'
+      - '1198'
     status:
       code: 201
       message: Created
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/E671AD99-24A2-4CD0-A891-1E688BBA525D?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/874FEC44-25EB-4C80-B37F-6E986B8B8221?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"id":"https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/E671AD99-24A2-4CD0-A891-1E688BBA525D?api-version=2020-06-01","name":"e671ad99-24a2-4cd0-a891-1e688bba525d","status":"Succeeded"}'
+      string: '{"id":"https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/874FEC44-25EB-4C80-B37F-6E986B8B8221?api-version=2020-10-15-preview","name":"874fec44-25eb-4c80-b37f-6e986b8b8221","status":"Succeeded"}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '279'
+      - '287'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:39 GMT
+      - Mon, 24 May 2021 06:41:03 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -223,29 +228,30 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"properties":{"provisioningState":"Succeeded","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"e81b8a8f-987e-47c5-b59f-34d73872a8ed","publicNetworkAccess":"Enabled"},"location":"westus","tags":{"tag1":"value1","tag2":"value2"},"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
+      string: '{"properties":{"provisioningState":"Succeeded","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"f9a9f07a-0f80-4980-8b8b-fac9e67ca89a","publicNetworkAccess":"Enabled"},"sku":{"name":"Basic"},"systemData":null,"location":"westus","tags":{"tag1":"value1","tag2":"value2"},"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '527'
+      - '573'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:39 GMT
+      - Mon, 24 May 2021 06:41:03 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -265,29 +271,30 @@
       Accept:
       - application/json
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"properties":{"provisioningState":"Succeeded","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"e81b8a8f-987e-47c5-b59f-34d73872a8ed","publicNetworkAccess":"Enabled"},"location":"westus","tags":{"tag1":"value1","tag2":"value2"},"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
+      string: '{"properties":{"provisioningState":"Succeeded","endpoint":"https://domain70eb095d.westus-1.eventgrid.azure.net/api/events","inputSchema":"EventGridSchema","metricResourceId":"f9a9f07a-0f80-4980-8b8b-fac9e67ca89a","publicNetworkAccess":"Enabled"},"sku":{"name":"Basic"},"systemData":null,"location":"westus","tags":{"tag1":"value1","tag2":"value2"},"id":"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d","name":"domain70eb095d","type":"Microsoft.EventGrid/domains"}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '527'
+      - '573'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:39 GMT
+      - Mon, 24 May 2021 06:41:03 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
@@ -309,71 +316,73 @@
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
       - '0'
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: DELETE
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/test_domain_test_domain70eb095d/providers/Microsoft.EventGrid/domains/domain70eb095d?api-version=2020-10-15-preview
   response:
     body:
       string: ''
     headers:
       azure-asyncoperation:
-      - https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/752B97CD-3A6A-4E28-A693-8B6601849484?api-version=2020-06-01
+      - https://management.azure.com:443/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/DB0A7498-3E71-4835-9466-54E7CE5AEC4B?api-version=2020-10-15-preview
       cache-control:
       - no-cache
       content-length:
       - '0'
       date:
-      - Tue, 27 Oct 2020 08:49:40 GMT
+      - Mon, 24 May 2021 06:41:03 GMT
       expires:
       - '-1'
       location:
-      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationResults/752B97CD-3A6A-4E28-A693-8B6601849484?api-version=2020-06-01
+      - https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationResults/DB0A7498-3E71-4835-9466-54E7CE5AEC4B?api-version=2020-10-15-preview
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
       - max-age=31536000; includeSubDomains
       x-content-type-options:
       - nosniff
       x-ms-ratelimit-remaining-subscription-deletes:
-      - '14998'
+      - '14999'
     status:
       code: 202
       message: Accepted
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - azsdk-python-mgmt-eventgrid/8.0.0b1 Python/3.6.9 (Linux-4.19.76-linuxkit-x86_64-with-Ubuntu-18.04-bionic)
+      - azsdk-python-mgmt-eventgrid/9.0.0 Python/3.8.10 (Linux-5.4.0-1047-azure-x86_64-with-glibc2.2.5)
+        VSTS_0fb41ef4-5012-48a9-bf39-4ee3de03ee35_build_2384_0
     method: GET
-    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/752B97CD-3A6A-4E28-A693-8B6601849484?api-version=2020-06-01
+    uri: https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/DB0A7498-3E71-4835-9466-54E7CE5AEC4B?api-version=2020-10-15-preview
   response:
     body:
-      string: '{"id":"https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/752B97CD-3A6A-4E28-A693-8B6601849484?api-version=2020-06-01","name":"752b97cd-3a6a-4e28-a693-8b6601849484","status":"Succeeded"}'
+      string: '{"id":"https://management.azure.com/subscriptions/00000000-0000-0000-0000-000000000000/providers/Microsoft.EventGrid/locations/westus/operationsStatus/DB0A7498-3E71-4835-9466-54E7CE5AEC4B?api-version=2020-10-15-preview","name":"db0a7498-3e71-4835-9466-54e7ce5aec4b","status":"Succeeded"}'
     headers:
       cache-control:
       - no-cache
       content-length:
-      - '279'
+      - '287'
       content-type:
       - application/json; charset=utf-8
       date:
-      - Tue, 27 Oct 2020 08:49:50 GMT
+      - Mon, 24 May 2021 06:41:13 GMT
       expires:
       - '-1'
       pragma:
       - no-cache
       server:
       - Microsoft-HTTPAPI/2.0
       strict-transport-security:
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_input_mappings_and_queue_destination.yaml` & `azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_input_mappings_and_queue_destination.yaml`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_topic_types.yaml` & `azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_topic_types.yaml`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/tests/recordings/test_azure_mgmt_eventgrid.test_domains_and_advanced_filter.yaml` & `azure-mgmt-eventgrid-9.0.0/tests/recordings/test_azure_mgmt_eventgrid.test_domains_and_advanced_filter.yaml`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/__init__.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/_configuration.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(EventGridManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2020-06-01"
+        self.api_version = "2020-10-15-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-eventgrid/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs  # type: Any
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/models/_event_grid_management_client_enums.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/models/_event_grid_management_client_enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,21 +38,44 @@
     NUMBER_GREATER_THAN_OR_EQUALS = "NumberGreaterThanOrEquals"
     BOOL_EQUALS = "BoolEquals"
     STRING_IN = "StringIn"
     STRING_NOT_IN = "StringNotIn"
     STRING_BEGINS_WITH = "StringBeginsWith"
     STRING_ENDS_WITH = "StringEndsWith"
     STRING_CONTAINS = "StringContains"
+    NUMBER_IN_RANGE = "NumberInRange"
+    NUMBER_NOT_IN_RANGE = "NumberNotInRange"
+    STRING_NOT_BEGINS_WITH = "StringNotBeginsWith"
+    STRING_NOT_ENDS_WITH = "StringNotEndsWith"
+    STRING_NOT_CONTAINS = "StringNotContains"
+    IS_NULL_OR_UNDEFINED = "IsNullOrUndefined"
+    IS_NOT_NULL = "IsNotNull"
+
+class CreatedByType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """The type of identity that created the resource.
+    """
+
+    USER = "User"
+    APPLICATION = "Application"
+    MANAGED_IDENTITY = "ManagedIdentity"
+    KEY = "Key"
 
 class DeadLetterEndPointType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Type of the endpoint for the dead letter destination
     """
 
     STORAGE_BLOB = "StorageBlob"
 
+class DeliveryAttributeMappingType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Type of the delivery attribute or header name.
+    """
+
+    STATIC = "Static"
+    DYNAMIC = "Dynamic"
+
 class DomainProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Provisioning state of the domain.
     """
 
     CREATING = "Creating"
     UPDATING = "Updating"
     DELETING = "Deleting"
@@ -79,54 +102,85 @@
     EVENT_HUB = "EventHub"
     STORAGE_QUEUE = "StorageQueue"
     HYBRID_CONNECTION = "HybridConnection"
     SERVICE_BUS_QUEUE = "ServiceBusQueue"
     SERVICE_BUS_TOPIC = "ServiceBusTopic"
     AZURE_FUNCTION = "AzureFunction"
 
-class Enum14(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class Enum25(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
 
     TOPICS = "topics"
     DOMAINS = "domains"
 
-class Enum15(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class Enum26(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
 
     TOPICS = "topics"
     DOMAINS = "domains"
 
-class Enum16(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class Enum27(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
 
     TOPICS = "topics"
     DOMAINS = "domains"
 
-class Enum17(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+class Enum28(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
 
     TOPICS = "topics"
     DOMAINS = "domains"
 
+class EventChannelProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Provisioning state of the event channel.
+    """
+
+    CREATING = "Creating"
+    UPDATING = "Updating"
+    DELETING = "Deleting"
+    SUCCEEDED = "Succeeded"
+    CANCELED = "Canceled"
+    FAILED = "Failed"
+
 class EventDeliverySchema(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """The event delivery schema for the event subscription.
     """
 
     EVENT_GRID_SCHEMA = "EventGridSchema"
     CUSTOM_INPUT_SCHEMA = "CustomInputSchema"
     CLOUD_EVENT_SCHEMA_V1_0 = "CloudEventSchemaV1_0"
 
+class EventSubscriptionIdentityType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """The type of managed identity used. The type 'SystemAssigned, UserAssigned' includes both an
+    implicitly created identity and a set of user-assigned identities. The type 'None' will remove
+    any identity.
+    """
+
+    SYSTEM_ASSIGNED = "SystemAssigned"
+    USER_ASSIGNED = "UserAssigned"
+
 class EventSubscriptionProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Provisioning state of the event subscription.
     """
 
     CREATING = "Creating"
     UPDATING = "Updating"
     DELETING = "Deleting"
     SUCCEEDED = "Succeeded"
     CANCELED = "Canceled"
     FAILED = "Failed"
     AWAITING_MANUAL_ACTION = "AwaitingManualAction"
 
+class IdentityType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """The type of managed identity used. The type 'SystemAssigned, UserAssigned' includes both an
+    implicitly created identity and a set of user-assigned identities. The type 'None' will remove
+    any identity.
+    """
+
+    NONE = "None"
+    SYSTEM_ASSIGNED = "SystemAssigned"
+    USER_ASSIGNED = "UserAssigned"
+    SYSTEM_ASSIGNED_USER_ASSIGNED = "SystemAssigned, UserAssigned"
+
 class InputSchema(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """This determines the format that Event Grid should expect for incoming events published to the
     domain.
     """
 
     EVENT_GRID_SCHEMA = "EventGridSchema"
     CUSTOM_EVENT_SCHEMA = "CustomEventSchema"
@@ -140,14 +194,81 @@
 
 class IpActionType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Action to perform based on the match or no match of the IpMask.
     """
 
     ALLOW = "Allow"
 
+class PartnerNamespaceProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Provisioning state of the partner namespace.
+    """
+
+    CREATING = "Creating"
+    UPDATING = "Updating"
+    DELETING = "Deleting"
+    SUCCEEDED = "Succeeded"
+    CANCELED = "Canceled"
+    FAILED = "Failed"
+
+class PartnerRegistrationProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Provisioning state of the partner registration.
+    """
+
+    CREATING = "Creating"
+    UPDATING = "Updating"
+    DELETING = "Deleting"
+    SUCCEEDED = "Succeeded"
+    CANCELED = "Canceled"
+    FAILED = "Failed"
+
+class PartnerRegistrationVisibilityState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Visibility state of the partner registration.
+    """
+
+    HIDDEN = "Hidden"
+    PUBLIC_PREVIEW = "PublicPreview"
+    GENERALLY_AVAILABLE = "GenerallyAvailable"
+
+class PartnerTopicActivationState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Activation state of the partner topic.
+    """
+
+    NEVER_ACTIVATED = "NeverActivated"
+    ACTIVATED = "Activated"
+    DEACTIVATED = "Deactivated"
+
+class PartnerTopicProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Provisioning state of the partner topic.
+    """
+
+    CREATING = "Creating"
+    UPDATING = "Updating"
+    DELETING = "Deleting"
+    SUCCEEDED = "Succeeded"
+    CANCELED = "Canceled"
+    FAILED = "Failed"
+
+class PartnerTopicReadinessState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """The readiness state of the corresponding partner topic.
+    """
+
+    NOT_ACTIVATED_BY_USER_YET = "NotActivatedByUserYet"
+    ACTIVATED_BY_USER = "ActivatedByUser"
+    DEACTIVATED_BY_USER = "DeactivatedByUser"
+    DELETED_BY_USER = "DeletedByUser"
+
+class PartnerTopicTypeAuthorizationState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Status of whether the customer has authorized a partner to create partner topics
+    in the customer's subscription.
+    """
+
+    NOT_APPLICABLE = "NotApplicable"
+    NOT_AUTHORIZED = "NotAuthorized"
+    AUTHORIZED = "Authorized"
+
 class PersistedConnectionStatus(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Status of the connection.
     """
 
     PENDING = "Pending"
     APPROVED = "Approved"
     REJECTED = "Rejected"
@@ -159,14 +280,21 @@
     cref="P:Microsoft.Azure.Events.ResourceProvider.Common.Contracts.DomainProperties.InboundIpRules"
     />`
     """
 
     ENABLED = "Enabled"
     DISABLED = "Disabled"
 
+class ResourceKind(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """Kind of the resource.
+    """
+
+    AZURE = "Azure"
+    AZURE_ARC = "AzureArc"
+
 class ResourceProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Provisioning state of the Private Endpoint Connection.
     """
 
     CREATING = "Creating"
     UPDATING = "Updating"
     DELETING = "Deleting"
@@ -177,25 +305,38 @@
 class ResourceRegionType(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Region type of the resource.
     """
 
     REGIONAL_RESOURCE = "RegionalResource"
     GLOBAL_RESOURCE = "GlobalResource"
 
+class Sku(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+    """The Sku name of the resource. The possible values are: Basic or Premium.
+    """
+
+    BASIC = "Basic"
+    PREMIUM = "Premium"
+
 class TopicProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Provisioning state of the topic.
     """
 
     CREATING = "Creating"
     UPDATING = "Updating"
     DELETING = "Deleting"
     SUCCEEDED = "Succeeded"
     CANCELED = "Canceled"
     FAILED = "Failed"
 
+class TopicTypePropertiesSupportedScopesForSourceItem(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
+
+    RESOURCE = "Resource"
+    RESOURCE_GROUP = "ResourceGroup"
+    AZURE_SUBSCRIPTION = "AzureSubscription"
+
 class TopicTypeProvisioningState(with_metaclass(_CaseInsensitiveEnumMeta, str, Enum)):
     """Provisioning state of the topic type
     """
 
     CREATING = "Creating"
     UPDATING = "Updating"
     DELETING = "Deleting"
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/__init__.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/_configuration.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(EventGridManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2020-06-01"
+        self.api_version = "2020-10-15-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-eventgrid/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs: Any
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_private_link_resources_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class PrivateLinkResourcesOperations:
     """PrivateLinkResourcesOperations async operations.
 
@@ -29,30 +29,30 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     async def get(
         self,
         resource_group_name: str,
         parent_type: str,
         parent_name: str,
         private_link_resource_name: str,
-        **kwargs
-    ) -> "models.PrivateLinkResource":
+        **kwargs: Any
+    ) -> "_models.PrivateLinkResource":
         """Get a private link resource.
 
         Get properties of a private link resource.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
@@ -64,20 +64,20 @@
         :param private_link_resource_name: The name of private link resource.
         :type private_link_resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResource, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.PrivateLinkResource
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateLinkResource"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateLinkResource"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -114,16 +114,16 @@
     def list_by_resource(
         self,
         resource_group_name: str,
         parent_type: str,
         parent_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.PrivateLinkResourcesListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.PrivateLinkResourcesListResult"]:
         """List private link resources under specific topic or domain.
 
         List all the private link resources under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
@@ -144,20 +144,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResourcesListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.PrivateLinkResourcesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateLinkResourcesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateLinkResourcesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_topic_types_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_topic_types_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class TopicTypesOperations:
     """TopicTypesOperations async operations.
 
@@ -29,41 +29,41 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def list(
         self,
-        **kwargs
-    ) -> AsyncIterable["models.TopicTypesListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.TopicTypesListResult"]:
         """List topic types.
 
         List all registered topic types.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either TopicTypesListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.TopicTypesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicTypesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicTypesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -104,33 +104,33 @@
             get_next, extract_data
         )
     list.metadata = {'url': '/providers/Microsoft.EventGrid/topicTypes'}  # type: ignore
 
     async def get(
         self,
         topic_type_name: str,
-        **kwargs
-    ) -> "models.TopicTypeInfo":
+        **kwargs: Any
+    ) -> "_models.TopicTypeInfo":
         """Get a topic type.
 
         Get information about a topic type.
 
         :param topic_type_name: Name of the topic type.
         :type topic_type_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TopicTypeInfo, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.TopicTypeInfo
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicTypeInfo"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicTypeInfo"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'topicTypeName': self._serialize.url("topic_type_name", topic_type_name, 'str'),
         }
@@ -159,33 +159,33 @@
 
         return deserialized
     get.metadata = {'url': '/providers/Microsoft.EventGrid/topicTypes/{topicTypeName}'}  # type: ignore
 
     def list_event_types(
         self,
         topic_type_name: str,
-        **kwargs
-    ) -> AsyncIterable["models.EventTypesListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventTypesListResult"]:
         """List event types.
 
         List event types for a topic type.
 
         :param topic_type_name: Name of the topic type.
         :type topic_type_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventTypesListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventTypesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventTypesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventTypesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
+from typing import TYPE_CHECKING
 import warnings
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
+from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models
+from .. import models as _models
 
-T = TypeVar('T')
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
 
-class Operations:
-    """Operations async operations.
+    T = TypeVar('T')
+    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+
+class Operations(object):
+    """Operations operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
     :ivar models: Alias to model classes used in this operation group.
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
-    def __init__(self, client, config, serializer, deserializer) -> None:
+    def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def list(
         self,
-        **kwargs
-    ) -> AsyncIterable["models.OperationsListResult"]:
+        **kwargs  # type: Any
+    ):
+        # type: (...) -> Iterable["_models.OperationsListResult"]
         """List available operations.
 
         List the available operations supported by the Microsoft.EventGrid resource provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationsListResult or the result of cls(response)
-        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.OperationsListResult]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.OperationsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.OperationsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -77,30 +82,30 @@
                 request = self._client.get(url, query_parameters, header_parameters)
             else:
                 url = next_link
                 query_parameters = {}  # type: Dict[str, Any]
                 request = self._client.get(url, query_parameters, header_parameters)
             return request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize('OperationsListResult', pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
-            return None, AsyncList(list_of_elem)
+            return None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
+        def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(
+        return ItemPaged(
             get_next, extract_data
         )
     list.metadata = {'url': '/providers/Microsoft.EventGrid/operations'}  # type: ignore
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_domains_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_domains_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class DomainsOperations:
     """DomainsOperations async operations.
 
@@ -31,47 +31,47 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     async def get(
         self,
         resource_group_name: str,
         domain_name: str,
-        **kwargs
-    ) -> "models.Domain":
+        **kwargs: Any
+    ) -> "_models.Domain":
         """Get a domain.
 
         Get properties of a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Domain, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.Domain
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -103,23 +103,23 @@
         return deserialized
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         domain_name: str,
-        domain_info: "models.Domain",
-        **kwargs
-    ) -> "models.Domain":
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        domain_info: "_models.Domain",
+        **kwargs: Any
+    ) -> "_models.Domain":
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -156,39 +156,39 @@
         return deserialized
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         domain_name: str,
-        domain_info: "models.Domain",
-        **kwargs
-    ) -> AsyncLROPoller["models.Domain"]:
+        domain_info: "_models.Domain",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.Domain"]:
         """Create or update a domain.
 
         Asynchronously creates or updates a new domain with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_info: Domain information.
         :type domain_info: ~azure.mgmt.eventgrid.models.Domain
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Domain or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.Domain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -205,15 +205,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Domain', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -223,22 +229,22 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     async def _delete_initial(
         self,
         resource_group_name: str,
         domain_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'domainName': self._serialize.url("domain_name", domain_name, 'str'),
@@ -252,41 +258,41 @@
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
 
         request = self._client.delete(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
-        if response.status_code not in [202, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     async def begin_delete(
         self,
         resource_group_name: str,
         domain_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a domain.
 
         Delete existing domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
@@ -307,15 +313,21 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -325,23 +337,23 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     async def _update_initial(
         self,
         resource_group_name: str,
         domain_name: str,
-        domain_update_parameters: "models.DomainUpdateParameters",
-        **kwargs
-    ) -> Optional["models.Domain"]:
-        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["models.Domain"]]
+        domain_update_parameters: "_models.DomainUpdateParameters",
+        **kwargs: Any
+    ) -> Optional["_models.Domain"]:
+        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Domain"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -380,39 +392,39 @@
         return deserialized
     _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     async def begin_update(
         self,
         resource_group_name: str,
         domain_name: str,
-        domain_update_parameters: "models.DomainUpdateParameters",
-        **kwargs
-    ) -> AsyncLROPoller["models.Domain"]:
+        domain_update_parameters: "_models.DomainUpdateParameters",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.Domain"]:
         """Update a domain.
 
         Asynchronously updates a domain with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_update_parameters: Domain update information.
         :type domain_update_parameters: ~azure.mgmt.eventgrid.models.DomainUpdateParameters
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -429,15 +441,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Domain', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -447,16 +465,16 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     def list_by_subscription(
         self,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.DomainsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.DomainsListResult"]:
         """List domains under an Azure subscription.
 
         List all the domains under an Azure subscription.
 
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
@@ -469,20 +487,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DomainsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.DomainsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -533,16 +551,16 @@
     list_by_subscription.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.EventGrid/domains'}  # type: ignore
 
     def list_by_resource_group(
         self,
         resource_group_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.DomainsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.DomainsListResult"]:
         """List domains under a resource group.
 
         List all the domains under a resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -557,20 +575,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DomainsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.DomainsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -621,35 +639,35 @@
         )
     list_by_resource_group.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains'}  # type: ignore
 
     async def list_shared_access_keys(
         self,
         resource_group_name: str,
         domain_name: str,
-        **kwargs
-    ) -> "models.DomainSharedAccessKeys":
+        **kwargs: Any
+    ) -> "_models.DomainSharedAccessKeys":
         """List keys for a domain.
 
         List the two keys used to publish to a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DomainSharedAccessKeys, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.DomainSharedAccessKeys
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainSharedAccessKeys"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.list_shared_access_keys.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -681,40 +699,38 @@
         return deserialized
     list_shared_access_keys.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/listKeys'}  # type: ignore
 
     async def regenerate_key(
         self,
         resource_group_name: str,
         domain_name: str,
-        key_name: str,
-        **kwargs
-    ) -> "models.DomainSharedAccessKeys":
+        regenerate_key_request: "_models.DomainRegenerateKeyRequest",
+        **kwargs: Any
+    ) -> "_models.DomainSharedAccessKeys":
         """Regenerate key for a domain.
 
         Regenerate a shared access key for a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
-        :param key_name: Key name to regenerate key1 or key2.
-        :type key_name: str
+        :param regenerate_key_request: Request body to regenerate key.
+        :type regenerate_key_request: ~azure.mgmt.eventgrid.models.DomainRegenerateKeyRequest
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DomainSharedAccessKeys, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.DomainSharedAccessKeys
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainSharedAccessKeys"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-
-        _regenerate_key_request = models.DomainRegenerateKeyRequest(key_name=key_name)
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self.regenerate_key.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -729,15 +745,15 @@
 
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
         header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
         header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
         body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(_regenerate_key_request, 'DomainRegenerateKeyRequest')
+        body_content = self._serialize.body(regenerate_key_request, 'DomainRegenerateKeyRequest')
         body_content_kwargs['content'] = body_content
         request = self._client.post(url, query_parameters, header_parameters, **body_content_kwargs)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_private_endpoint_connections_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class PrivateEndpointConnectionsOperations:
     """PrivateEndpointConnectionsOperations async operations.
 
@@ -31,56 +31,56 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     async def get(
         self,
         resource_group_name: str,
-        parent_type: Union[str, "models.Enum14"],
+        parent_type: Union[str, "_models.Enum25"],
         parent_name: str,
         private_endpoint_connection_name: str,
-        **kwargs
-    ) -> "models.PrivateEndpointConnection":
+        **kwargs: Any
+    ) -> "_models.PrivateEndpointConnection":
         """Get a specific private endpoint connection.
 
         Get a specific private endpoint connection under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum14
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum25
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection
          connection.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.PrivateEndpointConnection
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnection"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -113,26 +113,26 @@
 
         return deserialized
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     async def _update_initial(
         self,
         resource_group_name: str,
-        parent_type: Union[str, "models.Enum15"],
+        parent_type: Union[str, "_models.Enum26"],
         parent_name: str,
         private_endpoint_connection_name: str,
-        private_endpoint_connection: "models.PrivateEndpointConnection",
-        **kwargs
-    ) -> "models.PrivateEndpointConnection":
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnection"]
+        private_endpoint_connection: "_models.PrivateEndpointConnection",
+        **kwargs: Any
+    ) -> "_models.PrivateEndpointConnection":
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -174,49 +174,49 @@
 
         return deserialized
     _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     async def begin_update(
         self,
         resource_group_name: str,
-        parent_type: Union[str, "models.Enum15"],
+        parent_type: Union[str, "_models.Enum26"],
         parent_name: str,
         private_endpoint_connection_name: str,
-        private_endpoint_connection: "models.PrivateEndpointConnection",
-        **kwargs
-    ) -> AsyncLROPoller["models.PrivateEndpointConnection"]:
+        private_endpoint_connection: "_models.PrivateEndpointConnection",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.PrivateEndpointConnection"]:
         """Update a specific private endpoint connection.
 
         Update a specific private endpoint connection under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum15
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum26
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection
          connection.
         :type private_endpoint_connection_name: str
         :param private_endpoint_connection: The private endpoint connection object to update.
         :type private_endpoint_connection: ~azure.mgmt.eventgrid.models.PrivateEndpointConnection
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnection"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -235,15 +235,23 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'parentType': self._serialize.url("parent_type", parent_type, 'str'),
+            'parentName': self._serialize.url("parent_name", parent_name, 'str'),
+            'privateEndpointConnectionName': self._serialize.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -252,25 +260,25 @@
         else:
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     async def _delete_initial(
         self,
         resource_group_name: str,
-        parent_type: Union[str, "models.Enum16"],
+        parent_type: Union[str, "_models.Enum27"],
         parent_name: str,
         private_endpoint_connection_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'parentType': self._serialize.url("parent_type", parent_type, 'str'),
@@ -298,38 +306,38 @@
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     async def begin_delete(
         self,
         resource_group_name: str,
-        parent_type: Union[str, "models.Enum16"],
+        parent_type: Union[str, "_models.Enum27"],
         parent_name: str,
         private_endpoint_connection_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a specific private endpoint connection.
 
         Delete a specific private endpoint connection under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum16
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum27
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection
          connection.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
@@ -352,15 +360,23 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'parentType': self._serialize.url("parent_type", parent_type, 'str'),
+            'parentName': self._serialize.url("parent_name", parent_name, 'str'),
+            'privateEndpointConnectionName': self._serialize.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -369,29 +385,29 @@
         else:
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     def list_by_resource(
         self,
         resource_group_name: str,
-        parent_type: Union[str, "models.Enum17"],
+        parent_type: Union[str, "_models.Enum28"],
         parent_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.PrivateEndpointConnectionListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.PrivateEndpointConnectionListResult"]:
         """Lists all private endpoint connections under a resource.
 
         Get all private endpoint connections under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum17
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum28
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
          or, eq (for equal), and ne (for not equal). No arithmetic operations are supported. The
@@ -403,20 +419,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnectionListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.PrivateEndpointConnectionListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnectionListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnectionListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_domain_topics_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_domain_topics_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class DomainTopicsOperations:
     """DomainTopicsOperations async operations.
 
@@ -31,29 +31,29 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     async def get(
         self,
         resource_group_name: str,
         domain_name: str,
         domain_topic_name: str,
-        **kwargs
-    ) -> "models.DomainTopic":
+        **kwargs: Any
+    ) -> "_models.DomainTopic":
         """Get a domain topic.
 
         Get properties of a domain topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
@@ -61,20 +61,20 @@
         :param domain_topic_name: Name of the topic.
         :type domain_topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DomainTopic, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.DomainTopic
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -108,22 +108,22 @@
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{domainTopicName}'}  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         domain_name: str,
         domain_topic_name: str,
-        **kwargs
-    ) -> "models.DomainTopic":
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopic"]
+        **kwargs: Any
+    ) -> "_models.DomainTopic":
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -157,38 +157,38 @@
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{domainTopicName}'}  # type: ignore
 
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         domain_name: str,
         domain_topic_name: str,
-        **kwargs
-    ) -> AsyncLROPoller["models.DomainTopic"]:
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.DomainTopic"]:
         """Create or update a domain topic.
 
         Asynchronously creates or updates a new domain topic with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_topic_name: Name of the domain topic.
         :type domain_topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either DomainTopic or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.DomainTopic]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopic"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -205,15 +205,22 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('DomainTopic', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+            'domainTopicName': self._serialize.url("domain_topic_name", domain_topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -224,22 +231,22 @@
     begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{domainTopicName}'}  # type: ignore
 
     async def _delete_initial(
         self,
         resource_group_name: str,
         domain_name: str,
         domain_topic_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'domainName': self._serialize.url("domain_name", domain_name, 'str'),
@@ -254,44 +261,44 @@
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
 
         request = self._client.delete(url, query_parameters, header_parameters)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
-        if response.status_code not in [202, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{domainTopicName}'}  # type: ignore
 
     async def begin_delete(
         self,
         resource_group_name: str,
         domain_name: str,
         domain_topic_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a domain topic.
 
         Delete existing domain topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_topic_name: Name of the domain topic.
         :type domain_topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
@@ -313,15 +320,22 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+            'domainTopicName': self._serialize.url("domain_topic_name", domain_topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -333,16 +347,16 @@
 
     def list_by_domain(
         self,
         resource_group_name: str,
         domain_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.DomainTopicsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.DomainTopicsListResult"]:
         """List domain topics.
 
         List all the topics in a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Domain name.
@@ -359,20 +373,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DomainTopicsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.DomainTopicsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopicsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopicsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_event_subscriptions_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_event_subscriptions_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class EventSubscriptionsOperations:
     """EventSubscriptionsOperations async operations.
 
@@ -31,28 +31,28 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     async def get(
         self,
         scope: str,
         event_subscription_name: str,
-        **kwargs
-    ) -> "models.EventSubscription":
+        **kwargs: Any
+    ) -> "_models.EventSubscription":
         """Get an event subscription.
 
         Get properties of an event subscription.
 
         :param scope: The scope of the event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
          EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
@@ -65,20 +65,20 @@
         :param event_subscription_name: Name of the event subscription.
         :type event_subscription_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: EventSubscription, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.EventSubscription
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
             'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
@@ -109,23 +109,23 @@
         return deserialized
     get.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def _create_or_update_initial(
         self,
         scope: str,
         event_subscription_name: str,
-        event_subscription_info: "models.EventSubscription",
-        **kwargs
-    ) -> "models.EventSubscription":
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        event_subscription_info: "_models.EventSubscription",
+        **kwargs: Any
+    ) -> "_models.EventSubscription":
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
@@ -161,17 +161,17 @@
         return deserialized
     _create_or_update_initial.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def begin_create_or_update(
         self,
         scope: str,
         event_subscription_name: str,
-        event_subscription_info: "models.EventSubscription",
-        **kwargs
-    ) -> AsyncLROPoller["models.EventSubscription"]:
+        event_subscription_info: "_models.EventSubscription",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.EventSubscription"]:
         """Create or update an event subscription.
 
         Asynchronously creates a new event subscription or updates an existing event subscription based
         on the specified scope.
 
         :param scope: The identifier of the resource to which the event subscription needs to be
          created or updated. The scope can be a subscription, or a resource group, or a top level
@@ -187,24 +187,24 @@
          be between 3 and 64 characters in length and should use alphanumeric letters only.
         :type event_subscription_name: str
         :param event_subscription_info: Event subscription properties containing the destination and
          filter information.
         :type event_subscription_info: ~azure.mgmt.eventgrid.models.EventSubscription
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either EventSubscription or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.EventSubscription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -221,15 +221,20 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('EventSubscription', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -239,22 +244,22 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_create_or_update.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def _delete_initial(
         self,
         scope: str,
         event_subscription_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
             'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
         }
@@ -280,15 +285,15 @@
 
     _delete_initial.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def begin_delete(
         self,
         scope: str,
         event_subscription_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete an event subscription.
 
         Delete an existing event subscription.
 
         :param scope: The scope of the event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
@@ -299,16 +304,16 @@
          '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'
          for an EventGrid topic.
         :type scope: str
         :param event_subscription_name: Name of the event subscription.
         :type event_subscription_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
@@ -329,15 +334,20 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -347,23 +357,23 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def _update_initial(
         self,
         scope: str,
         event_subscription_name: str,
-        event_subscription_update_parameters: "models.EventSubscriptionUpdateParameters",
-        **kwargs
-    ) -> "models.EventSubscription":
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        event_subscription_update_parameters: "_models.EventSubscriptionUpdateParameters",
+        **kwargs: Any
+    ) -> "_models.EventSubscription":
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
@@ -399,17 +409,17 @@
         return deserialized
     _update_initial.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def begin_update(
         self,
         scope: str,
         event_subscription_name: str,
-        event_subscription_update_parameters: "models.EventSubscriptionUpdateParameters",
-        **kwargs
-    ) -> AsyncLROPoller["models.EventSubscription"]:
+        event_subscription_update_parameters: "_models.EventSubscriptionUpdateParameters",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.EventSubscription"]:
         """Update an event subscription.
 
         Asynchronously updates an existing event subscription.
 
         :param scope: The scope of existing event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
          EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
@@ -421,24 +431,24 @@
         :type scope: str
         :param event_subscription_name: Name of the event subscription to be updated.
         :type event_subscription_name: str
         :param event_subscription_update_parameters: Updated event subscription information.
         :type event_subscription_update_parameters: ~azure.mgmt.eventgrid.models.EventSubscriptionUpdateParameters
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either EventSubscription or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.EventSubscription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -455,15 +465,20 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('EventSubscription', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -473,16 +488,16 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_update.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     async def get_full_url(
         self,
         scope: str,
         event_subscription_name: str,
-        **kwargs
-    ) -> "models.EventSubscriptionFullUrl":
+        **kwargs: Any
+    ) -> "_models.EventSubscriptionFullUrl":
         """Get full URL of an event subscription.
 
         Get the full endpoint URL for an event subscription.
 
         :param scope: The scope of the event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
          EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
@@ -495,20 +510,20 @@
         :param event_subscription_name: Name of the event subscription.
         :type event_subscription_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: EventSubscriptionFullUrl, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.EventSubscriptionFullUrl
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionFullUrl"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionFullUrl"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get_full_url.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
             'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
@@ -539,16 +554,16 @@
         return deserialized
     get_full_url.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}/getFullUrl'}  # type: ignore
 
     def list_global_by_subscription(
         self,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """Get an aggregated list of all global event subscriptions under an Azure subscription.
 
         List all aggregated global event subscriptions under a specific Azure subscription.
 
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
@@ -561,20 +576,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -625,16 +640,16 @@
     list_global_by_subscription.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.EventGrid/eventSubscriptions'}  # type: ignore
 
     def list_global_by_subscription_for_topic_type(
         self,
         topic_type_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all global event subscriptions for a topic type.
 
         List all global event subscriptions under an Azure subscription for a topic type.
 
         :param topic_type_name: Name of the topic type.
         :type topic_type_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -649,20 +664,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -714,16 +729,16 @@
     list_global_by_subscription_for_topic_type.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.EventGrid/topicTypes/{topicTypeName}/eventSubscriptions'}  # type: ignore
 
     def list_global_by_resource_group(
         self,
         resource_group_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all global event subscriptions under an Azure subscription and resource group.
 
         List all global event subscriptions under a specific Azure subscription and resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -738,20 +753,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -804,16 +819,16 @@
 
     def list_global_by_resource_group_for_topic_type(
         self,
         resource_group_name: str,
         topic_type_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all global event subscriptions under a resource group for a topic type.
 
         List all global event subscriptions under a resource group for a specific topic type.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_type_name: Name of the topic type.
@@ -830,20 +845,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -896,16 +911,16 @@
     list_global_by_resource_group_for_topic_type.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topicTypes/{topicTypeName}/eventSubscriptions'}  # type: ignore
 
     def list_regional_by_subscription(
         self,
         location: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all regional event subscriptions under an Azure subscription.
 
         List all event subscriptions from the given location under a specific Azure subscription.
 
         :param location: Name of the location.
         :type location: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -920,20 +935,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -986,16 +1001,16 @@
 
     def list_regional_by_resource_group(
         self,
         resource_group_name: str,
         location: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all regional event subscriptions under an Azure subscription and resource group.
 
         List all event subscriptions from the given location under a specific Azure subscription and
         resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
@@ -1013,20 +1028,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1080,16 +1095,16 @@
 
     def list_regional_by_subscription_for_topic_type(
         self,
         location: str,
         topic_type_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all regional event subscriptions under an Azure subscription for a topic type.
 
         List all event subscriptions from the given location under a specific Azure subscription and
         topic type.
 
         :param location: Name of the location.
         :type location: str
@@ -1107,20 +1122,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1175,16 +1190,16 @@
     def list_regional_by_resource_group_for_topic_type(
         self,
         resource_group_name: str,
         location: str,
         topic_type_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all regional event subscriptions under an Azure subscription and resource group for a topic type.
 
         List all event subscriptions from the given location under a specific Azure subscription and
         resource group and topic type.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
@@ -1204,20 +1219,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1274,16 +1289,16 @@
         self,
         resource_group_name: str,
         provider_namespace: str,
         resource_type_name: str,
         resource_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all event subscriptions for a specific topic.
 
         List all event subscriptions that have been created for a specific topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param provider_namespace: Namespace of the provider of the topic.
@@ -1304,20 +1319,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1374,16 +1389,16 @@
     def list_by_domain_topic(
         self,
         resource_group_name: str,
         domain_name: str,
         topic_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.EventSubscriptionsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventSubscriptionsListResult"]:
         """List all event subscriptions for a specific domain topic.
 
         List all event subscriptions that have been created for a specific domain topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the top level domain.
@@ -1402,20 +1417,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1463,7 +1478,73 @@
 
             return pipeline_response
 
         return AsyncItemPaged(
             get_next, extract_data
         )
     list_by_domain_topic.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{topicName}/providers/Microsoft.EventGrid/eventSubscriptions'}  # type: ignore
+
+    async def get_delivery_attributes(
+        self,
+        scope: str,
+        event_subscription_name: str,
+        **kwargs: Any
+    ) -> "_models.DeliveryAttributeListResult":
+        """Get delivery attributes for an event subscription.
+
+        Get all delivery attributes for an event subscription.
+
+        :param scope: The scope of the event subscription. The scope can be a subscription, or a
+         resource group, or a top level resource belonging to a resource provider namespace, or an
+         EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}' for a resource group, and
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}'
+         for a resource, and
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'
+         for an EventGrid topic.
+        :type scope: str
+        :param event_subscription_name: Name of the event subscription.
+        :type event_subscription_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: DeliveryAttributeListResult, or the result of cls(response)
+        :rtype: ~azure.mgmt.eventgrid.models.DeliveryAttributeListResult
+        :raises: ~azure.core.exceptions.HttpResponseError
+        """
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DeliveryAttributeListResult"]
+        error_map = {
+            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+        }
+        error_map.update(kwargs.pop('error_map', {}))
+        api_version = "2020-10-15-preview"
+        accept = "application/json"
+
+        # Construct URL
+        url = self.get_delivery_attributes.metadata['url']  # type: ignore
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+        url = self._client.format_url(url, **path_format_arguments)
+
+        # Construct parameters
+        query_parameters = {}  # type: Dict[str, Any]
+        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+
+        # Construct headers
+        header_parameters = {}  # type: Dict[str, Any]
+        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+
+        request = self._client.post(url, query_parameters, header_parameters)
+        pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize('DeliveryAttributeListResult', pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+    get_delivery_attributes.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}/getDeliveryAttributes'}  # type: ignore
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/aio/operations/_topics_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_topics_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.core.polling import AsyncLROPoller, AsyncNoPolling, AsyncPollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.async_arm_polling import AsyncARMPolling
 
-from ... import models
+from ... import models as _models
 
 T = TypeVar('T')
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 class TopicsOperations:
     """TopicsOperations async operations.
 
@@ -31,47 +31,47 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     async def get(
         self,
         resource_group_name: str,
         topic_name: str,
-        **kwargs
-    ) -> "models.Topic":
+        **kwargs: Any
+    ) -> "_models.Topic":
         """Get a topic.
 
         Get properties of a topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Topic, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.Topic
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -103,23 +103,23 @@
         return deserialized
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     async def _create_or_update_initial(
         self,
         resource_group_name: str,
         topic_name: str,
-        topic_info: "models.Topic",
-        **kwargs
-    ) -> "models.Topic":
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        topic_info: "_models.Topic",
+        **kwargs: Any
+    ) -> "_models.Topic":
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -156,39 +156,39 @@
         return deserialized
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     async def begin_create_or_update(
         self,
         resource_group_name: str,
         topic_name: str,
-        topic_info: "models.Topic",
-        **kwargs
-    ) -> AsyncLROPoller["models.Topic"]:
+        topic_info: "_models.Topic",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.Topic"]:
         """Create a topic.
 
         Asynchronously creates a new topic with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :param topic_info: Topic information.
         :type topic_info: ~azure.mgmt.eventgrid.models.Topic
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either Topic or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.Topic]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._create_or_update_initial(
@@ -205,15 +205,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Topic', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -223,22 +229,22 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_create_or_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     async def _delete_initial(
         self,
         resource_group_name: str,
         topic_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> None:
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'topicName': self._serialize.url("topic_name", topic_name, 'str'),
@@ -265,28 +271,28 @@
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     async def begin_delete(
         self,
         resource_group_name: str,
         topic_name: str,
-        **kwargs
+        **kwargs: Any
     ) -> AsyncLROPoller[None]:
         """Delete a topic.
 
         Delete existing topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
@@ -307,15 +313,21 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -325,23 +337,23 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     async def _update_initial(
         self,
         resource_group_name: str,
         topic_name: str,
-        topic_update_parameters: "models.TopicUpdateParameters",
-        **kwargs
-    ) -> Optional["models.Topic"]:
-        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["models.Topic"]]
+        topic_update_parameters: "_models.TopicUpdateParameters",
+        **kwargs: Any
+    ) -> Optional["_models.Topic"]:
+        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Topic"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -380,39 +392,39 @@
         return deserialized
     _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     async def begin_update(
         self,
         resource_group_name: str,
         topic_name: str,
-        topic_update_parameters: "models.TopicUpdateParameters",
-        **kwargs
-    ) -> AsyncLROPoller["models.Topic"]:
+        topic_update_parameters: "_models.TopicUpdateParameters",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.Topic"]:
         """Update a topic.
 
         Asynchronously updates a topic with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :param topic_update_parameters: Topic update information.
         :type topic_update_parameters: ~azure.mgmt.eventgrid.models.TopicUpdateParameters
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of AsyncLROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.AsyncLROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = await self._update_initial(
@@ -429,15 +441,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Topic', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = AsyncARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = AsyncNoPolling()
         else: polling_method = polling
         if cont_token:
             return AsyncLROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -447,16 +465,16 @@
             return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     def list_by_subscription(
         self,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.TopicsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.TopicsListResult"]:
         """List topics under an Azure subscription.
 
         List all the topics under an Azure subscription.
 
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
@@ -469,20 +487,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either TopicsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.TopicsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -533,16 +551,16 @@
     list_by_subscription.metadata = {'url': '/subscriptions/{subscriptionId}/providers/Microsoft.EventGrid/topics'}  # type: ignore
 
     def list_by_resource_group(
         self,
         resource_group_name: str,
         filter: Optional[str] = None,
         top: Optional[int] = None,
-        **kwargs
-    ) -> AsyncIterable["models.TopicsListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.TopicsListResult"]:
         """List topics under a resource group.
 
         List all the topics under a resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -557,20 +575,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either TopicsListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.TopicsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -621,35 +639,35 @@
         )
     list_by_resource_group.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics'}  # type: ignore
 
     async def list_shared_access_keys(
         self,
         resource_group_name: str,
         topic_name: str,
-        **kwargs
-    ) -> "models.TopicSharedAccessKeys":
+        **kwargs: Any
+    ) -> "_models.TopicSharedAccessKeys":
         """List keys for a topic.
 
         List the two keys used to publish to a topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TopicSharedAccessKeys, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.TopicSharedAccessKeys
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicSharedAccessKeys"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.list_shared_access_keys.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -677,49 +695,32 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
     list_shared_access_keys.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/listKeys'}  # type: ignore
 
-    async def regenerate_key(
+    async def _regenerate_key_initial(
         self,
         resource_group_name: str,
         topic_name: str,
-        key_name: str,
-        **kwargs
-    ) -> "models.TopicSharedAccessKeys":
-        """Regenerate key for a topic.
-
-        Regenerate a shared access key for a topic.
-
-        :param resource_group_name: The name of the resource group within the user's subscription.
-        :type resource_group_name: str
-        :param topic_name: Name of the topic.
-        :type topic_name: str
-        :param key_name: Key name to regenerate key1 or key2.
-        :type key_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: TopicSharedAccessKeys, or the result of cls(response)
-        :rtype: ~azure.mgmt.eventgrid.models.TopicSharedAccessKeys
-        :raises: ~azure.core.exceptions.HttpResponseError
-        """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicSharedAccessKeys"]
+        regenerate_key_request: "_models.TopicRegenerateKeyRequest",
+        **kwargs: Any
+    ) -> Optional["_models.TopicSharedAccessKeys"]:
+        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.TopicSharedAccessKeys"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-
-        _regenerate_key_request = models.TopicRegenerateKeyRequest(key_name=key_name)
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
-        url = self.regenerate_key.metadata['url']  # type: ignore
+        url = self._regenerate_key_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'topicName': self._serialize.url("topic_name", topic_name, 'str'),
         }
         url = self._client.format_url(url, **path_format_arguments)
 
@@ -729,40 +730,115 @@
 
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
         header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
         header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
         body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(_regenerate_key_request, 'TopicRegenerateKeyRequest')
+        body_content = self._serialize.body(regenerate_key_request, 'TopicRegenerateKeyRequest')
         body_content_kwargs['content'] = body_content
         request = self._client.post(url, query_parameters, header_parameters, **body_content_kwargs)
         pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('TopicSharedAccessKeys', pipeline_response)
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize('TopicSharedAccessKeys', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
-    regenerate_key.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/regenerateKey'}  # type: ignore
+    _regenerate_key_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/regenerateKey'}  # type: ignore
+
+    async def begin_regenerate_key(
+        self,
+        resource_group_name: str,
+        topic_name: str,
+        regenerate_key_request: "_models.TopicRegenerateKeyRequest",
+        **kwargs: Any
+    ) -> AsyncLROPoller["_models.TopicSharedAccessKeys"]:
+        """Regenerate key for a topic.
+
+        Regenerate a shared access key for a topic.
+
+        :param resource_group_name: The name of the resource group within the user's subscription.
+        :type resource_group_name: str
+        :param topic_name: Name of the topic.
+        :type topic_name: str
+        :param regenerate_key_request: Request body to regenerate key.
+        :type regenerate_key_request: ~azure.mgmt.eventgrid.models.TopicRegenerateKeyRequest
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be AsyncARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.AsyncPollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+        :return: An instance of AsyncLROPoller that returns either TopicSharedAccessKeys or the result of cls(response)
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.mgmt.eventgrid.models.TopicSharedAccessKeys]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        polling = kwargs.pop('polling', True)  # type: Union[bool, AsyncPollingMethod]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicSharedAccessKeys"]
+        lro_delay = kwargs.pop(
+            'polling_interval',
+            self._config.polling_interval
+        )
+        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        if cont_token is None:
+            raw_result = await self._regenerate_key_initial(
+                resource_group_name=resource_group_name,
+                topic_name=topic_name,
+                regenerate_key_request=regenerate_key_request,
+                cls=lambda x,y,z: x,
+                **kwargs
+            )
+
+        kwargs.pop('error_map', None)
+        kwargs.pop('content_type', None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize('TopicSharedAccessKeys', pipeline_response)
+
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = AsyncARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        elif polling is False: polling_method = AsyncNoPolling()
+        else: polling_method = polling
+        if cont_token:
+            return AsyncLROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output
+            )
+        else:
+            return AsyncLROPoller(self._client, raw_result, get_long_running_output, polling_method)
+    begin_regenerate_key.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/regenerateKey'}  # type: ignore
 
     def list_event_types(
         self,
         resource_group_name: str,
         provider_namespace: str,
         resource_type_name: str,
         resource_name: str,
-        **kwargs
-    ) -> AsyncIterable["models.EventTypesListResult"]:
+        **kwargs: Any
+    ) -> AsyncIterable["_models.EventTypesListResult"]:
         """List topic event types.
 
         List event types for a topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param provider_namespace: Namespace of the provider of the topic.
@@ -772,20 +848,20 @@
         :param resource_name: Name of the topic.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventTypesListResult or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.EventTypesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventTypesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventTypesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_private_link_resources_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_private_link_resources_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -33,15 +33,15 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
@@ -49,15 +49,15 @@
         self,
         resource_group_name,  # type: str
         parent_type,  # type: str
         parent_name,  # type: str
         private_link_resource_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.PrivateLinkResource"
+        # type: (...) -> "_models.PrivateLinkResource"
         """Get a private link resource.
 
         Get properties of a private link resource.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
@@ -69,20 +69,20 @@
         :param private_link_resource_name: The name of private link resource.
         :type private_link_resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateLinkResource, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.PrivateLinkResource
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateLinkResource"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateLinkResource"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -121,15 +121,15 @@
         resource_group_name,  # type: str
         parent_type,  # type: str
         parent_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.PrivateLinkResourcesListResult"]
+        # type: (...) -> Iterable["_models.PrivateLinkResourcesListResult"]
         """List private link resources under specific topic or domain.
 
         List all the private link resources under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
@@ -150,20 +150,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateLinkResourcesListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.PrivateLinkResourcesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateLinkResourcesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateLinkResourcesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_topic_types_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_topic_types_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -33,42 +33,42 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def list(
         self,
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.TopicTypesListResult"]
+        # type: (...) -> Iterable["_models.TopicTypesListResult"]
         """List topic types.
 
         List all registered topic types.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either TopicTypesListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.TopicTypesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicTypesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicTypesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -111,32 +111,32 @@
     list.metadata = {'url': '/providers/Microsoft.EventGrid/topicTypes'}  # type: ignore
 
     def get(
         self,
         topic_type_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.TopicTypeInfo"
+        # type: (...) -> "_models.TopicTypeInfo"
         """Get a topic type.
 
         Get information about a topic type.
 
         :param topic_type_name: Name of the topic type.
         :type topic_type_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TopicTypeInfo, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.TopicTypeInfo
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicTypeInfo"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicTypeInfo"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'topicTypeName': self._serialize.url("topic_type_name", topic_type_name, 'str'),
         }
@@ -167,32 +167,32 @@
     get.metadata = {'url': '/providers/Microsoft.EventGrid/topicTypes/{topicTypeName}'}  # type: ignore
 
     def list_event_types(
         self,
         topic_type_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventTypesListResult"]
+        # type: (...) -> Iterable["_models.EventTypesListResult"]
         """List event types.
 
         List event types for a topic type.
 
         :param topic_type_name: Name of the topic type.
         :type topic_type_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventTypesListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventTypesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventTypesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventTypesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/aio/operations/_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import TYPE_CHECKING
+from typing import Any, AsyncIterable, Callable, Dict, Generic, Optional, TypeVar
 import warnings
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import ClientAuthenticationError, HttpResponseError, ResourceExistsError, ResourceNotFoundError, map_error
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpRequest, HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models
+from ... import models as _models
 
-if TYPE_CHECKING:
-    # pylint: disable=unused-import,ungrouped-imports
-    from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar
+T = TypeVar('T')
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-    T = TypeVar('T')
-    ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
-
-class Operations(object):
-    """Operations operations.
+class Operations:
+    """Operations async operations.
 
     You should not instantiate this class directly. Instead, you should create a Client instance that
     instantiates it for you and attaches it as an attribute.
 
     :ivar models: Alias to model classes used in this operation group.
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
-    def __init__(self, client, config, serializer, deserializer):
+    def __init__(self, client, config, serializer, deserializer) -> None:
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def list(
         self,
-        **kwargs  # type: Any
-    ):
-        # type: (...) -> Iterable["models.OperationsListResult"]
+        **kwargs: Any
+    ) -> AsyncIterable["_models.OperationsListResult"]:
         """List available operations.
 
         List the available operations supported by the Microsoft.EventGrid resource provider.
 
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either OperationsListResult or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.OperationsListResult]
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.eventgrid.models.OperationsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.OperationsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.OperationsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -82,30 +77,30 @@
                 request = self._client.get(url, query_parameters, header_parameters)
             else:
                 url = next_link
                 query_parameters = {}  # type: Dict[str, Any]
                 request = self._client.get(url, query_parameters, header_parameters)
             return request
 
-        def extract_data(pipeline_response):
+        async def extract_data(pipeline_response):
             deserialized = self._deserialize('OperationsListResult', pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)
-            return None, iter(list_of_elem)
+            return None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
+        async def get_next(next_link=None):
             request = prepare_request(next_link)
 
-            pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+            pipeline_response = await self._client._pipeline.run(request, stream=False, **kwargs)
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(
+        return AsyncItemPaged(
             get_next, extract_data
         )
     list.metadata = {'url': '/providers/Microsoft.EventGrid/operations'}  # type: ignore
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_domains_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_domains_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, Union
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -35,48 +35,48 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def get(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.Domain"
+        # type: (...) -> "_models.Domain"
         """Get a domain.
 
         Get properties of a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Domain, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.Domain
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -108,24 +108,24 @@
         return deserialized
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
-        domain_info,  # type: "models.Domain"
+        domain_info,  # type: "_models.Domain"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.Domain"
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        # type: (...) -> "_models.Domain"
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -162,40 +162,40 @@
         return deserialized
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     def begin_create_or_update(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
-        domain_info,  # type: "models.Domain"
+        domain_info,  # type: "_models.Domain"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.Domain"]
+        # type: (...) -> LROPoller["_models.Domain"]
         """Create or update a domain.
 
         Asynchronously creates or updates a new domain with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_info: Domain information.
         :type domain_info: ~azure.mgmt.eventgrid.models.Domain
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either Domain or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.Domain]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -212,15 +212,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Domain', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -238,15 +244,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'domainName': self._serialize.url("domain_name", domain_name, 'str'),
@@ -260,15 +266,15 @@
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
 
         request = self._client.delete(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
-        if response.status_code not in [202, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
@@ -286,16 +292,16 @@
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
@@ -316,15 +322,21 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -334,24 +346,24 @@
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     def _update_initial(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
-        domain_update_parameters,  # type: "models.DomainUpdateParameters"
+        domain_update_parameters,  # type: "_models.DomainUpdateParameters"
         **kwargs  # type: Any
     ):
-        # type: (...) -> Optional["models.Domain"]
-        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["models.Domain"]]
+        # type: (...) -> Optional["_models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Domain"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -390,40 +402,40 @@
         return deserialized
     _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}'}  # type: ignore
 
     def begin_update(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
-        domain_update_parameters,  # type: "models.DomainUpdateParameters"
+        domain_update_parameters,  # type: "_models.DomainUpdateParameters"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.Domain"]
+        # type: (...) -> LROPoller["_models.Domain"]
         """Update a domain.
 
         Asynchronously updates a domain with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_update_parameters: Domain update information.
         :type domain_update_parameters: ~azure.mgmt.eventgrid.models.DomainUpdateParameters
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Domain"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Domain"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(
@@ -440,15 +452,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Domain', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -460,15 +478,15 @@
 
     def list_by_subscription(
         self,
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.DomainsListResult"]
+        # type: (...) -> Iterable["_models.DomainsListResult"]
         """List domains under an Azure subscription.
 
         List all the domains under an Azure subscription.
 
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
@@ -481,20 +499,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DomainsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.DomainsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -547,15 +565,15 @@
     def list_by_resource_group(
         self,
         resource_group_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.DomainsListResult"]
+        # type: (...) -> Iterable["_models.DomainsListResult"]
         """List domains under a resource group.
 
         List all the domains under a resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -570,20 +588,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DomainsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.DomainsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -636,34 +654,34 @@
 
     def list_shared_access_keys(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.DomainSharedAccessKeys"
+        # type: (...) -> "_models.DomainSharedAccessKeys"
         """List keys for a domain.
 
         List the two keys used to publish to a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DomainSharedAccessKeys, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.DomainSharedAccessKeys
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainSharedAccessKeys"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.list_shared_access_keys.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -695,41 +713,39 @@
         return deserialized
     list_shared_access_keys.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/listKeys'}  # type: ignore
 
     def regenerate_key(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
-        key_name,  # type: str
+        regenerate_key_request,  # type: "_models.DomainRegenerateKeyRequest"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.DomainSharedAccessKeys"
+        # type: (...) -> "_models.DomainSharedAccessKeys"
         """Regenerate key for a domain.
 
         Regenerate a shared access key for a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
-        :param key_name: Key name to regenerate key1 or key2.
-        :type key_name: str
+        :param regenerate_key_request: Request body to regenerate key.
+        :type regenerate_key_request: ~azure.mgmt.eventgrid.models.DomainRegenerateKeyRequest
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DomainSharedAccessKeys, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.DomainSharedAccessKeys
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainSharedAccessKeys"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-
-        _regenerate_key_request = models.DomainRegenerateKeyRequest(key_name=key_name)
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self.regenerate_key.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -744,15 +760,15 @@
 
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
         header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
         header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
         body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(_regenerate_key_request, 'DomainRegenerateKeyRequest')
+        body_content = self._serialize.body(regenerate_key_request, 'DomainRegenerateKeyRequest')
         body_content_kwargs['content'] = body_content
         request = self._client.post(url, query_parameters, header_parameters, **body_content_kwargs)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_private_endpoint_connections_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, Union
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -35,57 +35,57 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def get(
         self,
         resource_group_name,  # type: str
-        parent_type,  # type: Union[str, "models.Enum14"]
+        parent_type,  # type: Union[str, "_models.Enum25"]
         parent_name,  # type: str
         private_endpoint_connection_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.PrivateEndpointConnection"
+        # type: (...) -> "_models.PrivateEndpointConnection"
         """Get a specific private endpoint connection.
 
         Get a specific private endpoint connection under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum14
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum25
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection
          connection.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: PrivateEndpointConnection, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.PrivateEndpointConnection
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnection"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -118,27 +118,27 @@
 
         return deserialized
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     def _update_initial(
         self,
         resource_group_name,  # type: str
-        parent_type,  # type: Union[str, "models.Enum15"]
+        parent_type,  # type: Union[str, "_models.Enum26"]
         parent_name,  # type: str
         private_endpoint_connection_name,  # type: str
-        private_endpoint_connection,  # type: "models.PrivateEndpointConnection"
+        private_endpoint_connection,  # type: "_models.PrivateEndpointConnection"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.PrivateEndpointConnection"
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnection"]
+        # type: (...) -> "_models.PrivateEndpointConnection"
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -180,50 +180,50 @@
 
         return deserialized
     _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     def begin_update(
         self,
         resource_group_name,  # type: str
-        parent_type,  # type: Union[str, "models.Enum15"]
+        parent_type,  # type: Union[str, "_models.Enum26"]
         parent_name,  # type: str
         private_endpoint_connection_name,  # type: str
-        private_endpoint_connection,  # type: "models.PrivateEndpointConnection"
+        private_endpoint_connection,  # type: "_models.PrivateEndpointConnection"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.PrivateEndpointConnection"]
+        # type: (...) -> LROPoller["_models.PrivateEndpointConnection"]
         """Update a specific private endpoint connection.
 
         Update a specific private endpoint connection under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum15
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum26
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection
          connection.
         :type private_endpoint_connection_name: str
         :param private_endpoint_connection: The private endpoint connection object to update.
         :type private_endpoint_connection: ~azure.mgmt.eventgrid.models.PrivateEndpointConnection
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either PrivateEndpointConnection or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.PrivateEndpointConnection]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnection"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnection"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(
@@ -242,15 +242,23 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('PrivateEndpointConnection', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'parentType': self._serialize.url("parent_type", parent_type, 'str'),
+            'parentName': self._serialize.url("parent_name", parent_name, 'str'),
+            'privateEndpointConnectionName': self._serialize.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -259,26 +267,26 @@
         else:
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_update.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     def _delete_initial(
         self,
         resource_group_name,  # type: str
-        parent_type,  # type: Union[str, "models.Enum16"]
+        parent_type,  # type: Union[str, "_models.Enum27"]
         parent_name,  # type: str
         private_endpoint_connection_name,  # type: str
         **kwargs  # type: Any
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'parentType': self._serialize.url("parent_type", parent_type, 'str'),
@@ -306,39 +314,39 @@
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     def begin_delete(
         self,
         resource_group_name,  # type: str
-        parent_type,  # type: Union[str, "models.Enum16"]
+        parent_type,  # type: Union[str, "_models.Enum27"]
         parent_name,  # type: str
         private_endpoint_connection_name,  # type: str
         **kwargs  # type: Any
     ):
         # type: (...) -> LROPoller[None]
         """Delete a specific private endpoint connection.
 
         Delete a specific private endpoint connection under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum16
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum27
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param private_endpoint_connection_name: The name of the private endpoint connection
          connection.
         :type private_endpoint_connection_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
@@ -361,15 +369,23 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'parentType': self._serialize.url("parent_type", parent_type, 'str'),
+            'parentName': self._serialize.url("parent_name", parent_name, 'str'),
+            'privateEndpointConnectionName': self._serialize.url("private_endpoint_connection_name", private_endpoint_connection_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -378,30 +394,30 @@
         else:
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/{parentType}/{parentName}/privateEndpointConnections/{privateEndpointConnectionName}'}  # type: ignore
 
     def list_by_resource(
         self,
         resource_group_name,  # type: str
-        parent_type,  # type: Union[str, "models.Enum17"]
+        parent_type,  # type: Union[str, "_models.Enum28"]
         parent_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.PrivateEndpointConnectionListResult"]
+        # type: (...) -> Iterable["_models.PrivateEndpointConnectionListResult"]
         """Lists all private endpoint connections under a resource.
 
         Get all private endpoint connections under a topic or domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param parent_type: The type of the parent resource. This can be either \'topics\' or
          \'domains\'.
-        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum17
+        :type parent_type: str or ~azure.mgmt.eventgrid.models.Enum28
         :param parent_name: The name of the parent resource (namely, either, the topic name or domain
          name).
         :type parent_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
          or, eq (for equal), and ne (for not equal). No arithmetic operations are supported. The
@@ -413,20 +429,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either PrivateEndpointConnectionListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.PrivateEndpointConnectionListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.PrivateEndpointConnectionListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.PrivateEndpointConnectionListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_domain_topics_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_domain_topics_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, Union
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -35,30 +35,30 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def get(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
         domain_topic_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.DomainTopic"
+        # type: (...) -> "_models.DomainTopic"
         """Get a domain topic.
 
         Get properties of a domain topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
@@ -66,20 +66,20 @@
         :param domain_topic_name: Name of the topic.
         :type domain_topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: DomainTopic, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.DomainTopic
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -115,21 +115,21 @@
     def _create_or_update_initial(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
         domain_topic_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.DomainTopic"
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopic"]
+        # type: (...) -> "_models.DomainTopic"
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -165,37 +165,37 @@
     def begin_create_or_update(
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
         domain_topic_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.DomainTopic"]
+        # type: (...) -> LROPoller["_models.DomainTopic"]
         """Create or update a domain topic.
 
         Asynchronously creates or updates a new domain topic with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_topic_name: Name of the domain topic.
         :type domain_topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either DomainTopic or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.DomainTopic]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopic"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -212,15 +212,22 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('DomainTopic', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+            'domainTopicName': self._serialize.url("domain_topic_name", domain_topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -239,15 +246,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'domainName': self._serialize.url("domain_name", domain_name, 'str'),
@@ -262,15 +269,15 @@
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
 
         request = self._client.delete(url, query_parameters, header_parameters)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
-        if response.status_code not in [202, 204]:
+        if response.status_code not in [200, 202, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     _delete_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{domainTopicName}'}  # type: ignore
@@ -291,16 +298,16 @@
         :type resource_group_name: str
         :param domain_name: Name of the domain.
         :type domain_name: str
         :param domain_topic_name: Name of the domain topic.
         :type domain_topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
@@ -322,15 +329,22 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'domainName': self._serialize.url("domain_name", domain_name, 'str'),
+            'domainTopicName': self._serialize.url("domain_topic_name", domain_topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -344,15 +358,15 @@
         self,
         resource_group_name,  # type: str
         domain_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.DomainTopicsListResult"]
+        # type: (...) -> Iterable["_models.DomainTopicsListResult"]
         """List domain topics.
 
         List all the topics in a domain.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Domain name.
@@ -369,20 +383,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either DomainTopicsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.DomainTopicsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.DomainTopicsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DomainTopicsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_event_subscriptions_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_event_subscriptions_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, Union
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -35,29 +35,29 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def get(
         self,
         scope,  # type: str
         event_subscription_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.EventSubscription"
+        # type: (...) -> "_models.EventSubscription"
         """Get an event subscription.
 
         Get properties of an event subscription.
 
         :param scope: The scope of the event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
          EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
@@ -70,20 +70,20 @@
         :param event_subscription_name: Name of the event subscription.
         :type event_subscription_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: EventSubscription, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.EventSubscription
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
             'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
@@ -114,24 +114,24 @@
         return deserialized
     get.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     def _create_or_update_initial(
         self,
         scope,  # type: str
         event_subscription_name,  # type: str
-        event_subscription_info,  # type: "models.EventSubscription"
+        event_subscription_info,  # type: "_models.EventSubscription"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.EventSubscription"
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        # type: (...) -> "_models.EventSubscription"
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
@@ -167,18 +167,18 @@
         return deserialized
     _create_or_update_initial.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     def begin_create_or_update(
         self,
         scope,  # type: str
         event_subscription_name,  # type: str
-        event_subscription_info,  # type: "models.EventSubscription"
+        event_subscription_info,  # type: "_models.EventSubscription"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.EventSubscription"]
+        # type: (...) -> LROPoller["_models.EventSubscription"]
         """Create or update an event subscription.
 
         Asynchronously creates a new event subscription or updates an existing event subscription based
         on the specified scope.
 
         :param scope: The identifier of the resource to which the event subscription needs to be
          created or updated. The scope can be a subscription, or a resource group, or a top level
@@ -194,24 +194,24 @@
          be between 3 and 64 characters in length and should use alphanumeric letters only.
         :type event_subscription_name: str
         :param event_subscription_info: Event subscription properties containing the destination and
          filter information.
         :type event_subscription_info: ~azure.mgmt.eventgrid.models.EventSubscription
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either EventSubscription or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.EventSubscription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -228,15 +228,20 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('EventSubscription', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -254,15 +259,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
             'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
         }
@@ -308,16 +313,16 @@
          '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'
          for an EventGrid topic.
         :type scope: str
         :param event_subscription_name: Name of the event subscription.
         :type event_subscription_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
@@ -338,15 +343,20 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -356,24 +366,24 @@
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     def _update_initial(
         self,
         scope,  # type: str
         event_subscription_name,  # type: str
-        event_subscription_update_parameters,  # type: "models.EventSubscriptionUpdateParameters"
+        event_subscription_update_parameters,  # type: "_models.EventSubscriptionUpdateParameters"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.EventSubscription"
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        # type: (...) -> "_models.EventSubscription"
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
@@ -409,18 +419,18 @@
         return deserialized
     _update_initial.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}'}  # type: ignore
 
     def begin_update(
         self,
         scope,  # type: str
         event_subscription_name,  # type: str
-        event_subscription_update_parameters,  # type: "models.EventSubscriptionUpdateParameters"
+        event_subscription_update_parameters,  # type: "_models.EventSubscriptionUpdateParameters"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.EventSubscription"]
+        # type: (...) -> LROPoller["_models.EventSubscription"]
         """Update an event subscription.
 
         Asynchronously updates an existing event subscription.
 
         :param scope: The scope of existing event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
          EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
@@ -432,24 +442,24 @@
         :type scope: str
         :param event_subscription_name: Name of the event subscription to be updated.
         :type event_subscription_name: str
         :param event_subscription_update_parameters: Updated event subscription information.
         :type event_subscription_update_parameters: ~azure.mgmt.eventgrid.models.EventSubscriptionUpdateParameters
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either EventSubscription or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.EventSubscription]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscription"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscription"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(
@@ -466,15 +476,20 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('EventSubscription', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -486,15 +501,15 @@
 
     def get_full_url(
         self,
         scope,  # type: str
         event_subscription_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.EventSubscriptionFullUrl"
+        # type: (...) -> "_models.EventSubscriptionFullUrl"
         """Get full URL of an event subscription.
 
         Get the full endpoint URL for an event subscription.
 
         :param scope: The scope of the event subscription. The scope can be a subscription, or a
          resource group, or a top level resource belonging to a resource provider namespace, or an
          EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
@@ -507,20 +522,20 @@
         :param event_subscription_name: Name of the event subscription.
         :type event_subscription_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: EventSubscriptionFullUrl, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.EventSubscriptionFullUrl
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionFullUrl"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionFullUrl"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get_full_url.metadata['url']  # type: ignore
         path_format_arguments = {
             'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
             'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
@@ -553,15 +568,15 @@
 
     def list_global_by_subscription(
         self,
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """Get an aggregated list of all global event subscriptions under an Azure subscription.
 
         List all aggregated global event subscriptions under a specific Azure subscription.
 
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
@@ -574,20 +589,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -640,15 +655,15 @@
     def list_global_by_subscription_for_topic_type(
         self,
         topic_type_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all global event subscriptions for a topic type.
 
         List all global event subscriptions under an Azure subscription for a topic type.
 
         :param topic_type_name: Name of the topic type.
         :type topic_type_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -663,20 +678,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -730,15 +745,15 @@
     def list_global_by_resource_group(
         self,
         resource_group_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all global event subscriptions under an Azure subscription and resource group.
 
         List all global event subscriptions under a specific Azure subscription and resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -753,20 +768,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -821,15 +836,15 @@
         self,
         resource_group_name,  # type: str
         topic_type_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all global event subscriptions under a resource group for a topic type.
 
         List all global event subscriptions under a resource group for a specific topic type.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_type_name: Name of the topic type.
@@ -846,20 +861,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -914,15 +929,15 @@
     def list_regional_by_subscription(
         self,
         location,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all regional event subscriptions under an Azure subscription.
 
         List all event subscriptions from the given location under a specific Azure subscription.
 
         :param location: Name of the location.
         :type location: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -937,20 +952,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1005,15 +1020,15 @@
         self,
         resource_group_name,  # type: str
         location,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all regional event subscriptions under an Azure subscription and resource group.
 
         List all event subscriptions from the given location under a specific Azure subscription and
         resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
@@ -1031,20 +1046,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1100,15 +1115,15 @@
         self,
         location,  # type: str
         topic_type_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all regional event subscriptions under an Azure subscription for a topic type.
 
         List all event subscriptions from the given location under a specific Azure subscription and
         topic type.
 
         :param location: Name of the location.
         :type location: str
@@ -1126,20 +1141,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1196,15 +1211,15 @@
         resource_group_name,  # type: str
         location,  # type: str
         topic_type_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all regional event subscriptions under an Azure subscription and resource group for a topic type.
 
         List all event subscriptions from the given location under a specific Azure subscription and
         resource group and topic type.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
@@ -1224,20 +1239,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1296,15 +1311,15 @@
         provider_namespace,  # type: str
         resource_type_name,  # type: str
         resource_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all event subscriptions for a specific topic.
 
         List all event subscriptions that have been created for a specific topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param provider_namespace: Namespace of the provider of the topic.
@@ -1325,20 +1340,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1397,15 +1412,15 @@
         resource_group_name,  # type: str
         domain_name,  # type: str
         topic_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventSubscriptionsListResult"]
+        # type: (...) -> Iterable["_models.EventSubscriptionsListResult"]
         """List all event subscriptions for a specific domain topic.
 
         List all event subscriptions that have been created for a specific domain topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param domain_name: Name of the top level domain.
@@ -1424,20 +1439,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventSubscriptionsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventSubscriptionsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventSubscriptionsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventSubscriptionsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -1485,7 +1500,74 @@
 
             return pipeline_response
 
         return ItemPaged(
             get_next, extract_data
         )
     list_by_domain_topic.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/domains/{domainName}/topics/{topicName}/providers/Microsoft.EventGrid/eventSubscriptions'}  # type: ignore
+
+    def get_delivery_attributes(
+        self,
+        scope,  # type: str
+        event_subscription_name,  # type: str
+        **kwargs  # type: Any
+    ):
+        # type: (...) -> "_models.DeliveryAttributeListResult"
+        """Get delivery attributes for an event subscription.
+
+        Get all delivery attributes for an event subscription.
+
+        :param scope: The scope of the event subscription. The scope can be a subscription, or a
+         resource group, or a top level resource belonging to a resource provider namespace, or an
+         EventGrid topic. For example, use '/subscriptions/{subscriptionId}/' for a subscription,
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}' for a resource group, and
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/{resourceType}/{resourceName}'
+         for a resource, and
+         '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'
+         for an EventGrid topic.
+        :type scope: str
+        :param event_subscription_name: Name of the event subscription.
+        :type event_subscription_name: str
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :return: DeliveryAttributeListResult, or the result of cls(response)
+        :rtype: ~azure.mgmt.eventgrid.models.DeliveryAttributeListResult
+        :raises: ~azure.core.exceptions.HttpResponseError
+        """
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.DeliveryAttributeListResult"]
+        error_map = {
+            401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
+        }
+        error_map.update(kwargs.pop('error_map', {}))
+        api_version = "2020-10-15-preview"
+        accept = "application/json"
+
+        # Construct URL
+        url = self.get_delivery_attributes.metadata['url']  # type: ignore
+        path_format_arguments = {
+            'scope': self._serialize.url("scope", scope, 'str', skip_quote=True),
+            'eventSubscriptionName': self._serialize.url("event_subscription_name", event_subscription_name, 'str'),
+        }
+        url = self._client.format_url(url, **path_format_arguments)
+
+        # Construct parameters
+        query_parameters = {}  # type: Dict[str, Any]
+        query_parameters['api-version'] = self._serialize.query("api_version", api_version, 'str')
+
+        # Construct headers
+        header_parameters = {}  # type: Dict[str, Any]
+        header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
+
+        request = self._client.post(url, query_parameters, header_parameters)
+        pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response, error_format=ARMErrorFormat)
+
+        deserialized = self._deserialize('DeliveryAttributeListResult', pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+    get_delivery_attributes.metadata = {'url': '/{scope}/providers/Microsoft.EventGrid/eventSubscriptions/{eventSubscriptionName}/getDeliveryAttributes'}  # type: ignore
```

## Comparing `azure-mgmt-eventgrid-8.0.0b1/azure/mgmt/eventgrid/operations/_topics_operations.py` & `azure-mgmt-eventgrid-9.0.0/azure/mgmt/eventgrid/operations/_topics_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
 from azure.core.polling import LROPoller, NoPolling, PollingMethod
 from azure.mgmt.core.exceptions import ARMErrorFormat
 from azure.mgmt.core.polling.arm_polling import ARMPolling
 
-from .. import models
+from .. import models as _models
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any, Callable, Dict, Generic, Iterable, Optional, TypeVar, Union
 
     T = TypeVar('T')
     ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
@@ -35,48 +35,48 @@
     :type models: ~azure.mgmt.eventgrid.models
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
     """
 
-    models = models
+    models = _models
 
     def __init__(self, client, config, serializer, deserializer):
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
         self._config = config
 
     def get(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.Topic"
+        # type: (...) -> "_models.Topic"
         """Get a topic.
 
         Get properties of a topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: Topic, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.Topic
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.get.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -108,24 +108,24 @@
         return deserialized
     get.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     def _create_or_update_initial(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
-        topic_info,  # type: "models.Topic"
+        topic_info,  # type: "_models.Topic"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.Topic"
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        # type: (...) -> "_models.Topic"
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._create_or_update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -162,40 +162,40 @@
         return deserialized
     _create_or_update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     def begin_create_or_update(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
-        topic_info,  # type: "models.Topic"
+        topic_info,  # type: "_models.Topic"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.Topic"]
+        # type: (...) -> LROPoller["_models.Topic"]
         """Create a topic.
 
         Asynchronously creates a new topic with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :param topic_info: Topic information.
         :type topic_info: ~azure.mgmt.eventgrid.models.Topic
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either Topic or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.Topic]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._create_or_update_initial(
@@ -212,15 +212,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Topic', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -238,15 +244,15 @@
     ):
         # type: (...) -> None
         cls = kwargs.pop('cls', None)  # type: ClsType[None]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
 
         # Construct URL
         url = self._delete_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'topicName': self._serialize.url("topic_name", topic_name, 'str'),
@@ -286,16 +292,16 @@
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
@@ -316,15 +322,21 @@
         kwargs.pop('error_map', None)
         kwargs.pop('content_type', None)
 
         def get_long_running_output(pipeline_response):
             if cls:
                 return cls(pipeline_response, None, {})
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -334,24 +346,24 @@
             return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
     begin_delete.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     def _update_initial(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
-        topic_update_parameters,  # type: "models.TopicUpdateParameters"
+        topic_update_parameters,  # type: "_models.TopicUpdateParameters"
         **kwargs  # type: Any
     ):
-        # type: (...) -> Optional["models.Topic"]
-        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["models.Topic"]]
+        # type: (...) -> Optional["_models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.Topic"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
         url = self._update_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
@@ -390,40 +402,40 @@
         return deserialized
     _update_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}'}  # type: ignore
 
     def begin_update(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
-        topic_update_parameters,  # type: "models.TopicUpdateParameters"
+        topic_update_parameters,  # type: "_models.TopicUpdateParameters"
         **kwargs  # type: Any
     ):
-        # type: (...) -> LROPoller["models.Topic"]
+        # type: (...) -> LROPoller["_models.Topic"]
         """Update a topic.
 
         Asynchronously updates a topic with the specified parameters.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :param topic_update_parameters: Topic update information.
         :type topic_update_parameters: ~azure.mgmt.eventgrid.models.TopicUpdateParameters
         :keyword callable cls: A custom type or function that will be passed the direct response
         :keyword str continuation_token: A continuation token to restart a poller from a saved state.
-        :keyword polling: True for ARMPolling, False for no polling, or a
-         polling object for personal polling strategy
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
         :paramtype polling: bool or ~azure.core.polling.PollingMethod
         :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
         :return: An instance of LROPoller that returns either None or the result of cls(response)
         :rtype: ~azure.core.polling.LROPoller[None]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.Topic"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.Topic"]
         lro_delay = kwargs.pop(
             'polling_interval',
             self._config.polling_interval
         )
         cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
         if cont_token is None:
             raw_result = self._update_initial(
@@ -440,15 +452,21 @@
         def get_long_running_output(pipeline_response):
             deserialized = self._deserialize('Topic', pipeline_response)
 
             if cls:
                 return cls(pipeline_response, deserialized, {})
             return deserialized
 
-        if polling is True: polling_method = ARMPolling(lro_delay,  **kwargs)
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
         elif polling is False: polling_method = NoPolling()
         else: polling_method = polling
         if cont_token:
             return LROPoller.from_continuation_token(
                 polling_method=polling_method,
                 continuation_token=cont_token,
                 client=self._client,
@@ -460,15 +478,15 @@
 
     def list_by_subscription(
         self,
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.TopicsListResult"]
+        # type: (...) -> Iterable["_models.TopicsListResult"]
         """List topics under an Azure subscription.
 
         List all the topics under an Azure subscription.
 
         :param filter: The query used to filter the search results using OData syntax. Filtering is
          permitted on the 'name' property only and with limited number of OData operations. These
          operations are: the 'contains' function as well as the following logical operations: not, and,
@@ -481,20 +499,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either TopicsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.TopicsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -547,15 +565,15 @@
     def list_by_resource_group(
         self,
         resource_group_name,  # type: str
         filter=None,  # type: Optional[str]
         top=None,  # type: Optional[int]
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.TopicsListResult"]
+        # type: (...) -> Iterable["_models.TopicsListResult"]
         """List topics under a resource group.
 
         List all the topics under a resource group.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param filter: The query used to filter the search results using OData syntax. Filtering is
@@ -570,20 +588,20 @@
          items per page.
         :type top: int
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either TopicsListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.TopicsListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicsListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicsListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
@@ -636,34 +654,34 @@
 
     def list_shared_access_keys(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.TopicSharedAccessKeys"
+        # type: (...) -> "_models.TopicSharedAccessKeys"
         """List keys for a topic.
 
         List the two keys used to publish to a topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param topic_name: Name of the topic.
         :type topic_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: TopicSharedAccessKeys, or the result of cls(response)
         :rtype: ~azure.mgmt.eventgrid.models.TopicSharedAccessKeys
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicSharedAccessKeys"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         # Construct URL
         url = self.list_shared_access_keys.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
@@ -691,50 +709,33 @@
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
     list_shared_access_keys.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/listKeys'}  # type: ignore
 
-    def regenerate_key(
+    def _regenerate_key_initial(
         self,
         resource_group_name,  # type: str
         topic_name,  # type: str
-        key_name,  # type: str
+        regenerate_key_request,  # type: "_models.TopicRegenerateKeyRequest"
         **kwargs  # type: Any
     ):
-        # type: (...) -> "models.TopicSharedAccessKeys"
-        """Regenerate key for a topic.
-
-        Regenerate a shared access key for a topic.
-
-        :param resource_group_name: The name of the resource group within the user's subscription.
-        :type resource_group_name: str
-        :param topic_name: Name of the topic.
-        :type topic_name: str
-        :param key_name: Key name to regenerate key1 or key2.
-        :type key_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: TopicSharedAccessKeys, or the result of cls(response)
-        :rtype: ~azure.mgmt.eventgrid.models.TopicSharedAccessKeys
-        :raises: ~azure.core.exceptions.HttpResponseError
-        """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.TopicSharedAccessKeys"]
+        # type: (...) -> Optional["_models.TopicSharedAccessKeys"]
+        cls = kwargs.pop('cls', None)  # type: ClsType[Optional["_models.TopicSharedAccessKeys"]]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-
-        _regenerate_key_request = models.TopicRegenerateKeyRequest(key_name=key_name)
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         content_type = kwargs.pop("content_type", "application/json")
         accept = "application/json"
 
         # Construct URL
-        url = self.regenerate_key.metadata['url']  # type: ignore
+        url = self._regenerate_key_initial.metadata['url']  # type: ignore
         path_format_arguments = {
             'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
             'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
             'topicName': self._serialize.url("topic_name", topic_name, 'str'),
         }
         url = self._client.format_url(url, **path_format_arguments)
 
@@ -744,41 +745,117 @@
 
         # Construct headers
         header_parameters = {}  # type: Dict[str, Any]
         header_parameters['Content-Type'] = self._serialize.header("content_type", content_type, 'str')
         header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
 
         body_content_kwargs = {}  # type: Dict[str, Any]
-        body_content = self._serialize.body(_regenerate_key_request, 'TopicRegenerateKeyRequest')
+        body_content = self._serialize.body(regenerate_key_request, 'TopicRegenerateKeyRequest')
         body_content_kwargs['content'] = body_content
         request = self._client.post(url, query_parameters, header_parameters, **body_content_kwargs)
         pipeline_response = self._client._pipeline.run(request, stream=False, **kwargs)
         response = pipeline_response.http_response
 
-        if response.status_code not in [200]:
+        if response.status_code not in [200, 202]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             raise HttpResponseError(response=response, error_format=ARMErrorFormat)
 
-        deserialized = self._deserialize('TopicSharedAccessKeys', pipeline_response)
+        deserialized = None
+        if response.status_code == 200:
+            deserialized = self._deserialize('TopicSharedAccessKeys', pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
-    regenerate_key.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/regenerateKey'}  # type: ignore
+    _regenerate_key_initial.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/regenerateKey'}  # type: ignore
+
+    def begin_regenerate_key(
+        self,
+        resource_group_name,  # type: str
+        topic_name,  # type: str
+        regenerate_key_request,  # type: "_models.TopicRegenerateKeyRequest"
+        **kwargs  # type: Any
+    ):
+        # type: (...) -> LROPoller["_models.TopicSharedAccessKeys"]
+        """Regenerate key for a topic.
+
+        Regenerate a shared access key for a topic.
+
+        :param resource_group_name: The name of the resource group within the user's subscription.
+        :type resource_group_name: str
+        :param topic_name: Name of the topic.
+        :type topic_name: str
+        :param regenerate_key_request: Request body to regenerate key.
+        :type regenerate_key_request: ~azure.mgmt.eventgrid.models.TopicRegenerateKeyRequest
+        :keyword callable cls: A custom type or function that will be passed the direct response
+        :keyword str continuation_token: A continuation token to restart a poller from a saved state.
+        :keyword polling: By default, your polling method will be ARMPolling.
+         Pass in False for this operation to not poll, or pass in your own initialized polling object for a personal polling strategy.
+        :paramtype polling: bool or ~azure.core.polling.PollingMethod
+        :keyword int polling_interval: Default waiting time between two polls for LRO operations if no Retry-After header is present.
+        :return: An instance of LROPoller that returns either TopicSharedAccessKeys or the result of cls(response)
+        :rtype: ~azure.core.polling.LROPoller[~azure.mgmt.eventgrid.models.TopicSharedAccessKeys]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        polling = kwargs.pop('polling', True)  # type: Union[bool, PollingMethod]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.TopicSharedAccessKeys"]
+        lro_delay = kwargs.pop(
+            'polling_interval',
+            self._config.polling_interval
+        )
+        cont_token = kwargs.pop('continuation_token', None)  # type: Optional[str]
+        if cont_token is None:
+            raw_result = self._regenerate_key_initial(
+                resource_group_name=resource_group_name,
+                topic_name=topic_name,
+                regenerate_key_request=regenerate_key_request,
+                cls=lambda x,y,z: x,
+                **kwargs
+            )
+
+        kwargs.pop('error_map', None)
+        kwargs.pop('content_type', None)
+
+        def get_long_running_output(pipeline_response):
+            deserialized = self._deserialize('TopicSharedAccessKeys', pipeline_response)
+
+            if cls:
+                return cls(pipeline_response, deserialized, {})
+            return deserialized
+
+        path_format_arguments = {
+            'subscriptionId': self._serialize.url("self._config.subscription_id", self._config.subscription_id, 'str'),
+            'resourceGroupName': self._serialize.url("resource_group_name", resource_group_name, 'str'),
+            'topicName': self._serialize.url("topic_name", topic_name, 'str'),
+        }
+
+        if polling is True: polling_method = ARMPolling(lro_delay, path_format_arguments=path_format_arguments,  **kwargs)
+        elif polling is False: polling_method = NoPolling()
+        else: polling_method = polling
+        if cont_token:
+            return LROPoller.from_continuation_token(
+                polling_method=polling_method,
+                continuation_token=cont_token,
+                client=self._client,
+                deserialization_callback=get_long_running_output
+            )
+        else:
+            return LROPoller(self._client, raw_result, get_long_running_output, polling_method)
+    begin_regenerate_key.metadata = {'url': '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.EventGrid/topics/{topicName}/regenerateKey'}  # type: ignore
 
     def list_event_types(
         self,
         resource_group_name,  # type: str
         provider_namespace,  # type: str
         resource_type_name,  # type: str
         resource_name,  # type: str
         **kwargs  # type: Any
     ):
-        # type: (...) -> Iterable["models.EventTypesListResult"]
+        # type: (...) -> Iterable["_models.EventTypesListResult"]
         """List topic event types.
 
         List event types for a topic.
 
         :param resource_group_name: The name of the resource group within the user's subscription.
         :type resource_group_name: str
         :param provider_namespace: Namespace of the provider of the topic.
@@ -788,20 +865,20 @@
         :param resource_name: Name of the topic.
         :type resource_name: str
         :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either EventTypesListResult or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.eventgrid.models.EventTypesListResult]
         :raises: ~azure.core.exceptions.HttpResponseError
         """
-        cls = kwargs.pop('cls', None)  # type: ClsType["models.EventTypesListResult"]
+        cls = kwargs.pop('cls', None)  # type: ClsType["_models.EventTypesListResult"]
         error_map = {
             401: ClientAuthenticationError, 404: ResourceNotFoundError, 409: ResourceExistsError
         }
         error_map.update(kwargs.pop('error_map', {}))
-        api_version = "2020-06-01"
+        api_version = "2020-10-15-preview"
         accept = "application/json"
 
         def prepare_request(next_link=None):
             # Construct headers
             header_parameters = {}  # type: Dict[str, Any]
             header_parameters['Accept'] = self._serialize.header("accept", accept, 'str')
```

