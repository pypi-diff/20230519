# Comparing `tmp/adestis-netbox-plugin-account-management-1.6.1.tar.gz` & `tmp/adestis-netbox-plugin-account-management-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adestis-netbox-plugin-account-management-1.6.1.tar", last modified: Fri May 19 12:29:41 2023, max compression
+gzip compressed data, was "adestis-netbox-plugin-account-management-1.6.2.tar", last modified: Fri May 19 12:57:43 2023, max compression
```

## Comparing `adestis-netbox-plugin-account-management-1.6.1.tar` & `adestis-netbox-plugin-account-management-1.6.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:41.025651 adestis-netbox-plugin-account-management-1.6.1/
--rw-rw-rw-   0        0        0     1088 2023-03-13 12:38:04.000000 adestis-netbox-plugin-account-management-1.6.1/LICENSE
--rw-rw-rw-   0        0        0      175 2023-03-14 14:02:58.000000 adestis-netbox-plugin-account-management-1.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0      326 2023-05-19 12:29:41.016638 adestis-netbox-plugin-account-management-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-03-14 14:02:58.000000 adestis-netbox-plugin-account-management-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.379140 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      494 2023-05-19 12:29:27.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.513832 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/
--rw-rw-rw-   0        0        0        0 2023-03-14 14:02:58.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/__init__.py
--rw-rw-rw-   0        0        0      516 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/nested_serializer.py
--rw-rw-rw-   0        0        0     2693 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/serializers.py
--rw-rw-rw-   0        0        0      301 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/urls.py
--rw-rw-rw-   0        0        0      659 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/views.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.558410 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/filtersets/
--rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/filtersets/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
--rw-rw-rw-   0        0        0     2610 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/filtersets/system.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.608220 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/forms/
--rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/forms/__init__.py
--rw-rw-rw-   0        0        0     4725 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/forms/login_credentials.py
--rw-rw-rw-   0        0        0     8074 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/forms/system.py
--rw-rw-rw-   0        0        0      878 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/graphql.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.778531 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/
--rw-rw-rw-   0        0        0     4634 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      426 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
--rw-rw-rw-   0        0        0      735 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
--rw-rw-rw-   0        0        0     4448 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
--rw-rw-rw-   0        0        0     1470 2023-05-19 12:29:12.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
--rw-rw-rw-   0        0        0      761 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
--rw-rw-rw-   0        0        0      401 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
--rw-rw-rw-   0        0        0      662 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
--rw-rw-rw-   0        0        0        0 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.846366 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/
--rw-rw-rw-   0        0        0       80 2023-05-15 13:22:31.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/__init__.py
--rw-rw-rw-   0        0        0     3303 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/login_credentials.py
--rw-rw-rw-   0        0        0     2805 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/person.py
--rw-rw-rw-   0        0        0     3347 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/system.py
--rw-rw-rw-   0        0        0     1331 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/navigation.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.902517 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/tables/
--rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/tables/__init__.py
--rw-rw-rw-   0        0        0      939 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/tables/login_credentials.py
--rw-rw-rw-   0        0        0     1180 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/tables/system.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.255379 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.951515 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
--rw-rw-rw-   0        0        0      371 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
--rw-rw-rw-   0        0        0     1685 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
--rw-rw-rw-   0        0        0     2865 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
--rw-rw-rw-   0        0        0     2110 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/urls.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:41.002818 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/views/
--rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/views/__init__.py
--rw-rw-rw-   0        0        0     2544 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/views/login_credentials.py
--rw-rw-rw-   0        0        0     1734 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/views/system.py
-drwxrwxrwx   0        0        0        0 2023-05-19 12:29:40.443130 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management.egg-info/
--rw-rw-rw-   0        0        0      326 2023-05-19 12:29:39.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2988 2023-05-19 12:29:40.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 12:29:39.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-19 12:29:39.000000 adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 12:29:41.026639 adestis-netbox-plugin-account-management-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-05-19 12:29:27.000000 adestis-netbox-plugin-account-management-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:43.046892 adestis-netbox-plugin-account-management-1.6.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-13 12:38:04.000000 adestis-netbox-plugin-account-management-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0      175 2023-03-14 14:02:58.000000 adestis-netbox-plugin-account-management-1.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      326 2023-05-19 12:57:43.021891 adestis-netbox-plugin-account-management-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1374 2023-03-14 14:02:58.000000 adestis-netbox-plugin-account-management-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.403863 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      494 2023-05-19 12:56:13.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.530746 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/
+-rw-rw-rw-   0        0        0        0 2023-03-14 14:02:58.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/nested_serializer.py
+-rw-rw-rw-   0        0        0     2693 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/serializers.py
+-rw-rw-rw-   0        0        0      301 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/urls.py
+-rw-rw-rw-   0        0        0      659 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/views.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.568726 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/filtersets/
+-rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/filtersets/__init__.py
+-rw-rw-rw-   0        0        0     1899 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/filtersets/login_credentials.py
+-rw-rw-rw-   0        0        0     2610 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/filtersets/system.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.608724 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/forms/
+-rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/forms/__init__.py
+-rw-rw-rw-   0        0        0     4725 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/forms/login_credentials.py
+-rw-rw-rw-   0        0        0     8074 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/forms/system.py
+-rw-rw-rw-   0        0        0      878 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/graphql.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.739730 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/
+-rw-rw-rw-   0        0        0     4634 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      426 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0002_alter_system_system_url.py
+-rw-rw-rw-   0        0        0      735 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py
+-rw-rw-rw-   0        0        0     4163 2023-05-19 12:54:59.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py
+-rw-rw-rw-   0        0        0     1470 2023-05-19 12:29:12.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py
+-rw-rw-rw-   0        0        0      761 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py
+-rw-rw-rw-   0        0        0      286 2023-05-19 12:55:48.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0007_remove_logincredentials_person.py
+-rw-rw-rw-   0        0        0      662 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py
+-rw-rw-rw-   0        0        0        0 2023-03-24 15:43:52.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.804731 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/
+-rw-rw-rw-   0        0        0       80 2023-05-15 13:22:31.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/__init__.py
+-rw-rw-rw-   0        0        0     3303 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/login_credentials.py
+-rw-rw-rw-   0        0        0     2805 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/person.py
+-rw-rw-rw-   0        0        0     3347 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/system.py
+-rw-rw-rw-   0        0        0     1331 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/navigation.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.857889 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/tables/
+-rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/tables/__init__.py
+-rw-rw-rw-   0        0        0      939 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/tables/login_credentials.py
+-rw-rw-rw-   0        0        0     1180 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/tables/system.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.300665 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.906888 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/
+-rw-rw-rw-   0        0        0      371 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/device_login_credentials_table.html
+-rw-rw-rw-   0        0        0     1685 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html
+-rw-rw-rw-   0        0        0     2865 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html
+-rw-rw-rw-   0        0        0     2110 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/urls.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.951892 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/views/
+-rw-rw-rw-   0        0        0       57 2023-05-15 15:58:01.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/views/__init__.py
+-rw-rw-rw-   0        0        0     2544 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/views/login_credentials.py
+-rw-rw-rw-   0        0        0     1734 2023-05-19 12:27:54.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/views/system.py
+drwxrwxrwx   0        0        0        0 2023-05-19 12:57:42.460725 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-05-19 12:57:41.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2988 2023-05-19 12:57:41.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 12:57:41.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-19 12:57:41.000000 adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 12:57:43.047891 adestis-netbox-plugin-account-management-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-05-19 12:56:13.000000 adestis-netbox-plugin-account-management-1.6.2/setup.py
```

### Comparing `adestis-netbox-plugin-account-management-1.6.1/LICENSE` & `adestis-netbox-plugin-account-management-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/README.md` & `adestis-netbox-plugin-account-management-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/nested_serializer.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/nested_serializer.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/serializers.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/serializers.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/api/views.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/api/views.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/filtersets/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/filtersets/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/filtersets/system.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/filtersets/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/forms/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/forms/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/forms/system.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/forms/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/graphql.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/graphql.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0001_initial.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0003_remove_logincredentials_adestis_netbox_plugin_account_management_logincredentials_unique_login_crede.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0004_alter_logincredentials_options_alter_person_options_and_more.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,13 +77,8 @@
             field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='system_tenant', to='tenancy.tenant'),
         ),
         migrations.AddField(
             model_name='system',
             name='virtual_machine',
             field=models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.SET_NULL, related_name='system_virtual_machine', to='virtualization.virtualmachine'),
         ),
-
-        # migrations.AddConstraint(
-        #     model_name='logincredentials',
-        #     constraint=models.UniqueConstraint(fields=('system', 'contact', 'logon_name'), name='adestis_netbox_plugin_account_management_logincredentials_unique_login_credentials'),
-        # ),
     ]
```

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0005_person_mitigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0006_fix_constraint_logincredentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/migrations/0008_alter_logincredentials_contact.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/person.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/person.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/models/system.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/models/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/navigation.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/navigation.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/tables/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/tables/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/tables/system.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/tables/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/logincredentials.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/templates/adestis_netbox_plugin_account_management/system.html`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/urls.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/urls.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/views/login_credentials.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/views/login_credentials.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management/views/system.py` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management/views/system.py`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt` & `adestis-netbox-plugin-account-management-1.6.2/adestis_netbox_plugin_account_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adestis-netbox-plugin-account-management-1.6.1/setup.py` & `adestis-netbox-plugin-account-management-1.6.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='adestis-netbox-plugin-account-management',
-    version='1.6.1',
+    version='1.6.2',
     description='ADESTIS Account Management',
     url='https://github.com/adestis/netbox-account-management',
     author='ADESTIS GmbH',
     author_email='pypi@adestis.de',
     install_requires=[],
     packages=find_packages(),
     include_package_data=True,
```

