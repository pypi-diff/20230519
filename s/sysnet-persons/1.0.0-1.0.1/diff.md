# Comparing `tmp/sysnet-persons-1.0.0.tar.gz` & `tmp/sysnet-persons-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysnet-persons-1.0.0.tar", last modified: Wed Feb  1 18:28:51 2023, max compression
+gzip compressed data, was "sysnet-persons-1.0.1.tar", last modified: Fri May 19 08:09:12 2023, max compression
```

## Comparing `sysnet-persons-1.0.0.tar` & `sysnet-persons-1.0.1.tar`

### file list

```diff
@@ -1,84 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 18:28:51.551606 sysnet-persons-1.0.0/
--rw-rw-rw-   0        0        0    11558 2022-09-22 12:06:50.000000 sysnet-persons-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    25029 2023-02-01 18:28:51.551606 sysnet-persons-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10988 2023-02-01 18:10:24.000000 sysnet-persons-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-01 18:28:51.441719 sysnet-persons-1.0.0/persons/
--rw-rw-rw-   0        0        0     2144 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-01 18:28:51.441719 sysnet-persons-1.0.0/persons/api/
--rw-rw-rw-   0        0        0      230 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/api/__init__.py
--rw-rw-rw-   0        0        0    25661 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/api/admins_api.py
--rw-rw-rw-   0        0        0     3860 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/api/developers_api.py
--rw-rw-rw-   0        0        0    72247 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/api/public_api.py
--rw-rw-rw-   0        0        0    25005 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/api_client.py
--rw-rw-rw-   0        0        0     8212 2023-02-01 18:10:24.000000 sysnet-persons-1.0.0/persons/configuration.py
-drwxrwxrwx   0        0        0        0 2023-02-01 18:28:51.488989 sysnet-persons-1.0.0/persons/models/
--rw-rw-rw-   0        0        0     1863 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/__init__.py
--rw-rw-rw-   0        0        0     3703 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/code_value_type.py
--rw-rw-rw-   0        0        0     2987 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/config_body.py
--rw-rw-rw-   0        0        0    12477 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/contact_type.py
--rw-rw-rw-   0        0        0     5277 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/context_type.py
--rw-rw-rw-   0        0        0     5903 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/context_type_persons.py
--rw-rw-rw-   0        0        0     3959 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/context_type_roles.py
--rw-rw-rw-   0        0        0     5128 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/department_type.py
--rw-rw-rw-   0        0        0     5839 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/document_entry.py
--rw-rw-rw-   0        0        0     7568 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/document_entry_list.py
--rw-rw-rw-   0        0        0     8241 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/document_metadata_type.py
--rw-rw-rw-   0        0        0     3621 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/geo_point_jtsk_type.py
--rw-rw-rw-   0        0        0     3693 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/geo_point_type.py
--rw-rw-rw-   0        0        0    13667 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/individual_type.py
--rw-rw-rw-   0        0        0     5363 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/issuing_type.py
--rw-rw-rw-   0        0        0     8602 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/models/location_type.py
--rw-rw-rw-   0        0        0     3859 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/mail_address_type.py
--rw-rw-rw-   0        0        0     5498 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/member_type.py
--rw-rw-rw-   0        0        0     5363 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/person_link_type.py
--rw-rw-rw-   0        0        0     6767 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/person_list_item.py
--rw-rw-rw-   0        0        0    17547 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/person_type.py
--rw-rw-rw-   0        0        0     4586 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/phone_number_type.py
--rw-rw-rw-   0        0        0     5231 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/reference_registry.py
--rw-rw-rw-   0        0        0     5405 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/role_category_type.py
--rw-rw-rw-   0        0        0     5206 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/role_list_item.py
--rw-rw-rw-   0        0        0    10766 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/role_type.py
--rw-rw-rw-   0        0        0     3761 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/tag_item_type.py
--rw-rw-rw-   0        0        0     3042 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/persons/models/tag_type.py
--rw-rw-rw-   0        0        0    12985 2023-02-01 18:08:09.000000 sysnet-persons-1.0.0/persons/rest.py
--rw-rw-rw-   0        0        0      673 2023-02-01 18:19:06.000000 sysnet-persons-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-01 18:28:51.551606 sysnet-persons-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-02-01 18:08:11.000000 sysnet-persons-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-01 18:28:51.504622 sysnet-persons-1.0.0/sysnet_persons.egg-info/
--rw-rw-rw-   0        0        0    25029 2023-02-01 18:28:51.000000 sysnet-persons-1.0.0/sysnet_persons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2228 2023-02-01 18:28:51.000000 sysnet-persons-1.0.0/sysnet_persons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 18:28:51.000000 sysnet-persons-1.0.0/sysnet_persons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-02-01 18:28:51.000000 sysnet-persons-1.0.0/sysnet_persons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-01 18:28:51.000000 sysnet-persons-1.0.0/sysnet_persons.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-01 18:28:51.551606 sysnet-persons-1.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_admins_api.py
--rw-rw-rw-   0        0        0      862 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_code_value_type.py
--rw-rw-rw-   0        0        0      836 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_config_body.py
--rw-rw-rw-   0        0        0      844 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_contact_type.py
--rw-rw-rw-   0        0        0      844 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_context_type.py
--rw-rw-rw-   0        0        0      902 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_context_type_persons.py
--rw-rw-rw-   0        0        0      886 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_context_type_roles.py
--rw-rw-rw-   0        0        0      868 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_department_type.py
--rw-rw-rw-   0        0        0      794 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_developers_api.py
--rw-rw-rw-   0        0        0      860 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_document_entry.py
--rw-rw-rw-   0        0        0      894 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_document_entry_list.py
--rw-rw-rw-   0        0        0      918 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_document_metadata_type.py
--rw-rw-rw-   0        0        0      888 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_geo_point_jtsk_type.py
--rw-rw-rw-   0        0        0      854 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_geo_point_type.py
--rw-rw-rw-   0        0        0      868 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_individual_type.py
--rw-rw-rw-   0        0        0      844 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_issuing_type.py
--rw-rw-rw-   0        0        0      852 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_location_type.py
--rw-rw-rw-   0        0        0      878 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_mail_address_type.py
--rw-rw-rw-   0        0        0      836 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_member_type.py
--rw-rw-rw-   0        0        0      870 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_person_link_type.py
--rw-rw-rw-   0        0        0      870 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_person_list_item.py
--rw-rw-rw-   0        0        0      836 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_person_type.py
--rw-rw-rw-   0        0        0      878 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_phone_number_type.py
--rw-rw-rw-   0        0        0     3629 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_public_api.py
--rw-rw-rw-   0        0        0      892 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_reference_registry.py
--rw-rw-rw-   0        0        0      886 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_role_category_type.py
--rw-rw-rw-   0        0        0      854 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_role_list_item.py
--rw-rw-rw-   0        0        0      820 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_role_type.py
--rw-rw-rw-   0        0        0      846 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_tag_item_type.py
--rw-rw-rw-   0        0        0      812 2023-02-01 18:08:10.000000 sysnet-persons-1.0.0/test/test_tag_type.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2022-09-22 12:06:50.000000 sysnet-persons-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    28378 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14312 2023-05-19 08:07:51.000000 sysnet-persons-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.764594 sysnet-persons-1.0.1/persons/
+-rw-rw-rw-   0        0        0     2230 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.780231 sysnet-persons-1.0.1/persons/api/
+-rw-rw-rw-   0        0        0      316 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/persons/api/__init__.py
+-rw-rw-rw-   0        0        0    25661 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api/admins_api.py
+-rw-rw-rw-   0        0        0     6822 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api/developers_api.py
+-rw-rw-rw-   0        0        0    38477 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api/link_api.py
+-rw-rw-rw-   0        0        0    53758 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/persons/api/manage_api.py
+-rw-rw-rw-   0        0        0    72247 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/persons/api/public_api.py
+-rw-rw-rw-   0        0        0    25005 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/api_client.py
+-rw-rw-rw-   0        0        0     8212 2023-05-19 08:05:47.000000 sysnet-persons-1.0.1/persons/configuration.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.836197 sysnet-persons-1.0.1/persons/models/
+-rw-rw-rw-   0        0        0     1863 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/__init__.py
+-rw-rw-rw-   0        0        0     3703 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/code_value_type.py
+-rw-rw-rw-   0        0        0     2987 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/config_body.py
+-rw-rw-rw-   0        0        0    13229 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/contact_type.py
+-rw-rw-rw-   0        0        0     5277 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/context_type.py
+-rw-rw-rw-   0        0        0     5903 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/context_type_persons.py
+-rw-rw-rw-   0        0        0     3959 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/context_type_roles.py
+-rw-rw-rw-   0        0        0     5128 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/department_type.py
+-rw-rw-rw-   0        0        0     5839 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/document_entry.py
+-rw-rw-rw-   0        0        0     7568 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/document_entry_list.py
+-rw-rw-rw-   0        0        0     8241 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/document_metadata_type.py
+-rw-rw-rw-   0        0        0     3621 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/geo_point_jtsk_type.py
+-rw-rw-rw-   0        0        0     3693 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/geo_point_type.py
+-rw-rw-rw-   0        0        0    13655 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/individual_type.py
+-rw-rw-rw-   0        0        0     5363 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/issuing_type.py
+-rw-rw-rw-   0        0        0     9273 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/location_type.py
+-rw-rw-rw-   0        0        0     3859 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/mail_address_type.py
+-rw-rw-rw-   0        0        0     5498 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/member_type.py
+-rw-rw-rw-   0        0        0     5363 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/person_link_type.py
+-rw-rw-rw-   0        0        0     6767 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/person_list_item.py
+-rw-rw-rw-   0        0        0    17547 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/person_type.py
+-rw-rw-rw-   0        0        0     4586 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/phone_number_type.py
+-rw-rw-rw-   0        0        0     5231 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/reference_registry.py
+-rw-rw-rw-   0        0        0     5405 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/role_category_type.py
+-rw-rw-rw-   0        0        0     5206 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/role_list_item.py
+-rw-rw-rw-   0        0        0    10766 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/role_type.py
+-rw-rw-rw-   0        0        0     3761 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/tag_item_type.py
+-rw-rw-rw-   0        0        0     3042 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/models/tag_type.py
+-rw-rw-rw-   0        0        0    12985 2023-05-19 07:57:53.000000 sysnet-persons-1.0.1/persons/rest.py
+-rw-rw-rw-   0        0        0      673 2023-05-19 08:07:51.000000 sysnet-persons-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-05-19 07:57:55.000000 sysnet-persons-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.851858 sysnet-persons-1.0.1/sysnet_persons.egg-info/
+-rw-rw-rw-   0        0        0    28378 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2324 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 08:09:12.000000 sysnet-persons-1.0.1/sysnet_persons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 08:09:12.904259 sysnet-persons-1.0.1/test/
+-rw-rw-rw-   0        0        0       15 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1673 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_admins_api.py
+-rw-rw-rw-   0        0        0      862 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_code_value_type.py
+-rw-rw-rw-   0        0        0      836 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_config_body.py
+-rw-rw-rw-   0        0        0      844 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_contact_type.py
+-rw-rw-rw-   0        0        0      844 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_context_type.py
+-rw-rw-rw-   0        0        0      902 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_context_type_persons.py
+-rw-rw-rw-   0        0        0      886 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_context_type_roles.py
+-rw-rw-rw-   0        0        0      868 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_department_type.py
+-rw-rw-rw-   0        0        0      955 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_developers_api.py
+-rw-rw-rw-   0        0        0      860 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_document_entry.py
+-rw-rw-rw-   0        0        0      894 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_document_entry_list.py
+-rw-rw-rw-   0        0        0      918 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_document_metadata_type.py
+-rw-rw-rw-   0        0        0      888 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_geo_point_jtsk_type.py
+-rw-rw-rw-   0        0        0      854 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_geo_point_type.py
+-rw-rw-rw-   0        0        0      868 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_individual_type.py
+-rw-rw-rw-   0        0        0      844 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_issuing_type.py
+-rw-rw-rw-   0        0        0     2080 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_link_api.py
+-rw-rw-rw-   0        0        0      852 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_location_type.py
+-rw-rw-rw-   0        0        0      878 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_mail_address_type.py
+-rw-rw-rw-   0        0        0     3163 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_manage_api.py
+-rw-rw-rw-   0        0        0      836 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_member_type.py
+-rw-rw-rw-   0        0        0      870 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_person_link_type.py
+-rw-rw-rw-   0        0        0      870 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_person_list_item.py
+-rw-rw-rw-   0        0        0      836 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_person_type.py
+-rw-rw-rw-   0        0        0      878 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_phone_number_type.py
+-rw-rw-rw-   0        0        0     3629 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_public_api.py
+-rw-rw-rw-   0        0        0      892 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_reference_registry.py
+-rw-rw-rw-   0        0        0      886 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_role_category_type.py
+-rw-rw-rw-   0        0        0      854 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_role_list_item.py
+-rw-rw-rw-   0        0        0      820 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_role_type.py
+-rw-rw-rw-   0        0        0      846 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_tag_item_type.py
+-rw-rw-rw-   0        0        0      812 2023-05-19 07:57:54.000000 sysnet-persons-1.0.1/test/test_tag_type.py
```

### Comparing `sysnet-persons-1.0.0/LICENSE` & `sysnet-persons-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysnet-persons-1.0.0/PKG-INFO` & `sysnet-persons-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-persons
-Version: 1.0.0
+Version: 1.0.1
 Summary: SYSNET Persons Registry REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,36 +212,35 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# persons
+# sysnet-persons
 This is a API to Persons Registry
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
-- Package version: 1.0.0
+- API version: 1.0.1
+- Package version: 1.0.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install sysnet-persons
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
 import persons 
 ```
 
 ### Setuptools
@@ -391,26 +390,52 @@
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_tag: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/persons/1.0.0*
+All URIs are relative to *https://service.sysnet.cz/persons/1.0.1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**delete_tag**](docs/AdminsApi.md#delete_tag) | **DELETE** /tag/{name} | odstraní definici tagu  (cruD)
 *AdminsApi* | [**get_config**](docs/AdminsApi.md#get_config) | **GET** /config | získá konfiguraci konektoru
 *AdminsApi* | [**get_tag**](docs/AdminsApi.md#get_tag) | **GET** /tag/{name} | vrací definici tagu (cRud)
 *AdminsApi* | [**get_tag_list**](docs/AdminsApi.md#get_tag_list) | **GET** /tag | vrací seznam tagů v systému (autocomplete)
 *AdminsApi* | [**post_tag**](docs/AdminsApi.md#post_tag) | **POST** /tag | vytvoří nový tag (Crud)
 *AdminsApi* | [**put_config**](docs/AdminsApi.md#put_config) | **PUT** /config | aktualizuje hlavní konfiguraci konektoru
 *AdminsApi* | [**put_tag**](docs/AdminsApi.md#put_tag) | **PUT** /tag/{name} | aktualizuje definici tagu (crUd)
 *DevelopersApi* | [**info_api**](docs/DevelopersApi.md#info_api) | **GET** /info | vrací servisní informace
+*DevelopersApi* | [**info_api_head**](docs/DevelopersApi.md#info_api_head) | **HEAD** /info | vrací informaci o dostupnosti služby
+*LinkApi* | [**delete_individual_role**](docs/LinkApi.md#delete_individual_role) | **DELETE** /individual/role/{individual_id} | Odebere roli uživateli
+*LinkApi* | [**delete_person_member**](docs/LinkApi.md#delete_person_member) | **DELETE** /person/member/{person_id} | Odebere člena osobě
+*LinkApi* | [**delete_person_role**](docs/LinkApi.md#delete_person_role) | **DELETE** /person/role/{person_id} | Odebere roli osobě
+*LinkApi* | [**get_individual_roles**](docs/LinkApi.md#get_individual_roles) | **GET** /individual/role/{individual_id} | Získá všechny role pro uživatele
+*LinkApi* | [**get_person_members**](docs/LinkApi.md#get_person_members) | **GET** /person/member/{person_id} | Získá všechny uživatele pro osobu
+*LinkApi* | [**get_person_roles**](docs/LinkApi.md#get_person_roles) | **GET** /person/role/{person_id} | Získá všechny role pro osobu
+*LinkApi* | [**put_individual_role**](docs/LinkApi.md#put_individual_role) | **PUT** /individual/role/{individual_id} | Přiřadí uživateli roli
+*LinkApi* | [**put_person_member**](docs/LinkApi.md#put_person_member) | **PUT** /person/member/{person_id} | Přiřadí uživatela za člena osoby
+*LinkApi* | [**put_person_role**](docs/LinkApi.md#put_person_role) | **PUT** /person/role/{person_id} | Přiřadí osobě roli
+*ManageApi* | [**check_individuals**](docs/ManageApi.md#check_individuals) | **HEAD** /individual/data | Kontroluje existenci kolekce uživatelů
+*ManageApi* | [**check_persons**](docs/ManageApi.md#check_persons) | **HEAD** /person/data | Kontroluje existenci kolekce subjektů
+*ManageApi* | [**check_roles**](docs/ManageApi.md#check_roles) | **HEAD** /role/data | Kontroluje existenci kolekce rolí
+*ManageApi* | [**check_tags**](docs/ManageApi.md#check_tags) | **HEAD** /tag/data | Kontroluje existenci kolekce tagů
+*ManageApi* | [**export_individuals**](docs/ManageApi.md#export_individuals) | **GET** /individual/data | Exportuje všechny uživatele ve formátu BSON
+*ManageApi* | [**export_persons**](docs/ManageApi.md#export_persons) | **GET** /person/data | Exportuje všechny subjekty ve formátu BSON
+*ManageApi* | [**export_roles**](docs/ManageApi.md#export_roles) | **GET** /role/data | Exportuje všechny role ve formátu BSON
+*ManageApi* | [**export_tags**](docs/ManageApi.md#export_tags) | **GET** /tag/data | Exportuje všechny tagy ve formátu BSON
+*ManageApi* | [**import_individuals**](docs/ManageApi.md#import_individuals) | **PUT** /individual/data | Importuje uživatele
+*ManageApi* | [**import_individuals_replace**](docs/ManageApi.md#import_individuals_replace) | **POST** /individual/data | Nahradí všechny uživatele
+*ManageApi* | [**import_persons**](docs/ManageApi.md#import_persons) | **PUT** /person/data | Importuje subjekty
+*ManageApi* | [**import_persons_replace**](docs/ManageApi.md#import_persons_replace) | **POST** /person/data | Nahradí všechny subjekty
+*ManageApi* | [**import_roles**](docs/ManageApi.md#import_roles) | **PUT** /role/data | Importuje role
+*ManageApi* | [**import_roles_replace**](docs/ManageApi.md#import_roles_replace) | **POST** /role/data | Nahradí všechny role
+*ManageApi* | [**import_tags**](docs/ManageApi.md#import_tags) | **PUT** /tag/data | Importuje tagy
+*ManageApi* | [**import_tags_replace**](docs/ManageApi.md#import_tags_replace) | **POST** /tag/data | Nahradí všechny tagy
 *PublicApi* | [**delete_individual**](docs/PublicApi.md#delete_individual) | **DELETE** /individual/{identifier} | odstraní registrační dokument jednotlivce s daným identifikátorem (cruD)
 *PublicApi* | [**delete_person**](docs/PublicApi.md#delete_person) | **DELETE** /person/{identifier} | odstraní registrační dokument subjektu s daným identifikátorem (cruD)
 *PublicApi* | [**delete_role**](docs/PublicApi.md#delete_role) | **DELETE** /role/{identifier} | odstraní roli s daným identifikátorem (cruD)
 *PublicApi* | [**get_context**](docs/PublicApi.md#get_context) | **GET** /context/{identifier} | vrací kontext jednotlivce
 *PublicApi* | [**get_individual**](docs/PublicApi.md#get_individual) | **GET** /individual/{identifier} | vrací registrační dokument jednotlivce s daným identifikátorem (cRud)
 *PublicApi* | [**get_individual_list**](docs/PublicApi.md#get_individual_list) | **GET** /individual | vrací seznam jednotlivců (autocomplete)
 *PublicApi* | [**get_person**](docs/PublicApi.md#get_person) | **GET** /person/{identifier} | vrací registrační dokument subjektu s daným identifikátorem (cRud)
```

### Comparing `sysnet-persons-1.0.0/README.md` & `sysnet-persons-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# persons
+# sysnet-persons
 This is a API to Persons Registry
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
-- Package version: 1.0.0
+- API version: 1.0.1
+- Package version: 1.0.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install sysnet-persons
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
 import persons 
 ```
 
 ### Setuptools
@@ -173,26 +172,52 @@
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_tag: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/persons/1.0.0*
+All URIs are relative to *https://service.sysnet.cz/persons/1.0.1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**delete_tag**](docs/AdminsApi.md#delete_tag) | **DELETE** /tag/{name} | odstraní definici tagu  (cruD)
 *AdminsApi* | [**get_config**](docs/AdminsApi.md#get_config) | **GET** /config | získá konfiguraci konektoru
 *AdminsApi* | [**get_tag**](docs/AdminsApi.md#get_tag) | **GET** /tag/{name} | vrací definici tagu (cRud)
 *AdminsApi* | [**get_tag_list**](docs/AdminsApi.md#get_tag_list) | **GET** /tag | vrací seznam tagů v systému (autocomplete)
 *AdminsApi* | [**post_tag**](docs/AdminsApi.md#post_tag) | **POST** /tag | vytvoří nový tag (Crud)
 *AdminsApi* | [**put_config**](docs/AdminsApi.md#put_config) | **PUT** /config | aktualizuje hlavní konfiguraci konektoru
 *AdminsApi* | [**put_tag**](docs/AdminsApi.md#put_tag) | **PUT** /tag/{name} | aktualizuje definici tagu (crUd)
 *DevelopersApi* | [**info_api**](docs/DevelopersApi.md#info_api) | **GET** /info | vrací servisní informace
+*DevelopersApi* | [**info_api_head**](docs/DevelopersApi.md#info_api_head) | **HEAD** /info | vrací informaci o dostupnosti služby
+*LinkApi* | [**delete_individual_role**](docs/LinkApi.md#delete_individual_role) | **DELETE** /individual/role/{individual_id} | Odebere roli uživateli
+*LinkApi* | [**delete_person_member**](docs/LinkApi.md#delete_person_member) | **DELETE** /person/member/{person_id} | Odebere člena osobě
+*LinkApi* | [**delete_person_role**](docs/LinkApi.md#delete_person_role) | **DELETE** /person/role/{person_id} | Odebere roli osobě
+*LinkApi* | [**get_individual_roles**](docs/LinkApi.md#get_individual_roles) | **GET** /individual/role/{individual_id} | Získá všechny role pro uživatele
+*LinkApi* | [**get_person_members**](docs/LinkApi.md#get_person_members) | **GET** /person/member/{person_id} | Získá všechny uživatele pro osobu
+*LinkApi* | [**get_person_roles**](docs/LinkApi.md#get_person_roles) | **GET** /person/role/{person_id} | Získá všechny role pro osobu
+*LinkApi* | [**put_individual_role**](docs/LinkApi.md#put_individual_role) | **PUT** /individual/role/{individual_id} | Přiřadí uživateli roli
+*LinkApi* | [**put_person_member**](docs/LinkApi.md#put_person_member) | **PUT** /person/member/{person_id} | Přiřadí uživatela za člena osoby
+*LinkApi* | [**put_person_role**](docs/LinkApi.md#put_person_role) | **PUT** /person/role/{person_id} | Přiřadí osobě roli
+*ManageApi* | [**check_individuals**](docs/ManageApi.md#check_individuals) | **HEAD** /individual/data | Kontroluje existenci kolekce uživatelů
+*ManageApi* | [**check_persons**](docs/ManageApi.md#check_persons) | **HEAD** /person/data | Kontroluje existenci kolekce subjektů
+*ManageApi* | [**check_roles**](docs/ManageApi.md#check_roles) | **HEAD** /role/data | Kontroluje existenci kolekce rolí
+*ManageApi* | [**check_tags**](docs/ManageApi.md#check_tags) | **HEAD** /tag/data | Kontroluje existenci kolekce tagů
+*ManageApi* | [**export_individuals**](docs/ManageApi.md#export_individuals) | **GET** /individual/data | Exportuje všechny uživatele ve formátu BSON
+*ManageApi* | [**export_persons**](docs/ManageApi.md#export_persons) | **GET** /person/data | Exportuje všechny subjekty ve formátu BSON
+*ManageApi* | [**export_roles**](docs/ManageApi.md#export_roles) | **GET** /role/data | Exportuje všechny role ve formátu BSON
+*ManageApi* | [**export_tags**](docs/ManageApi.md#export_tags) | **GET** /tag/data | Exportuje všechny tagy ve formátu BSON
+*ManageApi* | [**import_individuals**](docs/ManageApi.md#import_individuals) | **PUT** /individual/data | Importuje uživatele
+*ManageApi* | [**import_individuals_replace**](docs/ManageApi.md#import_individuals_replace) | **POST** /individual/data | Nahradí všechny uživatele
+*ManageApi* | [**import_persons**](docs/ManageApi.md#import_persons) | **PUT** /person/data | Importuje subjekty
+*ManageApi* | [**import_persons_replace**](docs/ManageApi.md#import_persons_replace) | **POST** /person/data | Nahradí všechny subjekty
+*ManageApi* | [**import_roles**](docs/ManageApi.md#import_roles) | **PUT** /role/data | Importuje role
+*ManageApi* | [**import_roles_replace**](docs/ManageApi.md#import_roles_replace) | **POST** /role/data | Nahradí všechny role
+*ManageApi* | [**import_tags**](docs/ManageApi.md#import_tags) | **PUT** /tag/data | Importuje tagy
+*ManageApi* | [**import_tags_replace**](docs/ManageApi.md#import_tags_replace) | **POST** /tag/data | Nahradí všechny tagy
 *PublicApi* | [**delete_individual**](docs/PublicApi.md#delete_individual) | **DELETE** /individual/{identifier} | odstraní registrační dokument jednotlivce s daným identifikátorem (cruD)
 *PublicApi* | [**delete_person**](docs/PublicApi.md#delete_person) | **DELETE** /person/{identifier} | odstraní registrační dokument subjektu s daným identifikátorem (cruD)
 *PublicApi* | [**delete_role**](docs/PublicApi.md#delete_role) | **DELETE** /role/{identifier} | odstraní roli s daným identifikátorem (cruD)
 *PublicApi* | [**get_context**](docs/PublicApi.md#get_context) | **GET** /context/{identifier} | vrací kontext jednotlivce
 *PublicApi* | [**get_individual**](docs/PublicApi.md#get_individual) | **GET** /individual/{identifier} | vrací registrační dokument jednotlivce s daným identifikátorem (cRud)
 *PublicApi* | [**get_individual_list**](docs/PublicApi.md#get_individual_list) | **GET** /individual | vrací seznam jednotlivců (autocomplete)
 *PublicApi* | [**get_person**](docs/PublicApi.md#get_person) | **GET** /person/{identifier} | vrací registrační dokument subjektu s daným identifikátorem (cRud)
```

### Comparing `sysnet-persons-1.0.0/persons/__init__.py` & `sysnet-persons-1.0.1/persons/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 # flake8: noqa
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from persons.api.admins_api import AdminsApi
 from persons.api.developers_api import DevelopersApi
+from persons.api.link_api import LinkApi
+from persons.api.manage_api import ManageApi
 from persons.api.public_api import PublicApi
 # import ApiClient
 from persons.api_client import ApiClient
 from persons.configuration import Configuration
 # import models into sdk package
 from persons.models.code_value_type import CodeValueType
 from persons.models.config_body import ConfigBody
```

### Comparing `sysnet-persons-1.0.0/persons/api/admins_api.py` & `sysnet-persons-1.0.1/persons/api/admins_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/api/public_api.py` & `sysnet-persons-1.0.1/persons/api/public_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/api_client.py` & `sysnet-persons-1.0.1/persons/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.0/python'
+        self.user_agent = 'Swagger-Codegen/1.0.1/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `sysnet-persons-1.0.0/persons/configuration.py` & `sysnet-persons-1.0.1/persons/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
@@ -42,15 +42,15 @@
     Ref: https://github.com/swagger-api/swagger-codegen
     Do not edit the class manually.
     """
 
     def __init__(self):
         """Constructor"""
         # Default Base url
-        self.host = "https://service.sysnet.cz/persons/1.0.0"
+        self.host = "https://service.sysnet.cz/persons/1.0.1"
         # Temp file folder for downloading files
         self.temp_folder_path = None
 
         # Authentication Settings
         # dict to store API key(s)
         self.api_key = {}
         # dict to store API prefix (e.g. Bearer)
@@ -242,10 +242,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.0".\
+               "Version of the API: 1.0.1\n"\
+               "SDK Package Version: 1.0.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `sysnet-persons-1.0.0/persons/models/__init__.py` & `sysnet-persons-1.0.1/persons/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
```

### Comparing `sysnet-persons-1.0.0/persons/models/code_value_type.py` & `sysnet-persons-1.0.1/persons/models/code_value_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/config_body.py` & `sysnet-persons-1.0.1/persons/models/config_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/contact_type.py` & `sysnet-persons-1.0.1/persons/models/contact_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -30,14 +30,15 @@
     swagger_types = {
         'identifier': 'str',
         'first_name': 'str',
         'last_name': 'str',
         'degree_before': 'list[str]',
         'degree_after': 'list[str]',
         'full_name': 'str',
+        'birthdate': 'date',
         'phone': 'list[PhoneNumberType]',
         'phone_default': 'int',
         'email': 'list[MailAddressType]',
         'email_default': 'int',
         'web': 'str',
         'isds': 'str',
         'reference': 'str'
@@ -46,31 +47,33 @@
     attribute_map = {
         'identifier': 'identifier',
         'first_name': 'firstName',
         'last_name': 'lastName',
         'degree_before': 'degreeBefore',
         'degree_after': 'degreeAfter',
         'full_name': 'fullName',
+        'birthdate': 'birthdate',
         'phone': 'phone',
         'phone_default': 'phoneDefault',
         'email': 'email',
         'email_default': 'emailDefault',
         'web': 'web',
         'isds': 'isds',
         'reference': 'reference'
     }
 
-    def __init__(self, identifier=None, first_name=None, last_name=None, degree_before=None, degree_after=None, full_name=None, phone=None, phone_default=0, email=None, email_default=0, web=None, isds=None, reference=None):  # noqa: E501
+    def __init__(self, identifier=None, first_name=None, last_name=None, degree_before=None, degree_after=None, full_name=None, birthdate=None, phone=None, phone_default=0, email=None, email_default=0, web=None, isds=None, reference=None):  # noqa: E501
         """ContactType - a model defined in Swagger"""  # noqa: E501
         self._identifier = None
         self._first_name = None
         self._last_name = None
         self._degree_before = None
         self._degree_after = None
         self._full_name = None
+        self._birthdate = None
         self._phone = None
         self._phone_default = None
         self._email = None
         self._email_default = None
         self._web = None
         self._isds = None
         self._reference = None
@@ -83,14 +86,16 @@
             self.last_name = last_name
         if degree_before is not None:
             self.degree_before = degree_before
         if degree_after is not None:
             self.degree_after = degree_after
         if full_name is not None:
             self.full_name = full_name
+        if birthdate is not None:
+            self.birthdate = birthdate
         if phone is not None:
             self.phone = phone
         if phone_default is not None:
             self.phone_default = phone_default
         if email is not None:
             self.email = email
         if email_default is not None:
@@ -237,14 +242,37 @@
         :param full_name: The full_name of this ContactType.  # noqa: E501
         :type: str
         """
 
         self._full_name = full_name
 
     @property
+    def birthdate(self):
+        """Gets the birthdate of this ContactType.  # noqa: E501
+
+        Datum narození  # noqa: E501
+
+        :return: The birthdate of this ContactType.  # noqa: E501
+        :rtype: date
+        """
+        return self._birthdate
+
+    @birthdate.setter
+    def birthdate(self, birthdate):
+        """Sets the birthdate of this ContactType.
+
+        Datum narození  # noqa: E501
+
+        :param birthdate: The birthdate of this ContactType.  # noqa: E501
+        :type: date
+        """
+
+        self._birthdate = birthdate
+
+    @property
     def phone(self):
         """Gets the phone of this ContactType.  # noqa: E501
 
         Telefonní číslo  # noqa: E501
 
         :return: The phone of this ContactType.  # noqa: E501
         :rtype: list[PhoneNumberType]
```

### Comparing `sysnet-persons-1.0.0/persons/models/context_type.py` & `sysnet-persons-1.0.1/persons/models/context_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/context_type_persons.py` & `sysnet-persons-1.0.1/persons/models/context_type_persons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/context_type_roles.py` & `sysnet-persons-1.0.1/persons/models/context_type_roles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/department_type.py` & `sysnet-persons-1.0.1/persons/models/department_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/document_entry.py` & `sysnet-persons-1.0.1/persons/models/document_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/document_entry_list.py` & `sysnet-persons-1.0.1/persons/models/document_entry_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/document_metadata_type.py` & `sysnet-persons-1.0.1/persons/models/document_metadata_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/geo_point_jtsk_type.py` & `sysnet-persons-1.0.1/persons/models/geo_point_jtsk_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/geo_point_type.py` & `sysnet-persons-1.0.1/persons/models/geo_point_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/individual_type.py` & `sysnet-persons-1.0.1/persons/models/individual_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -35,15 +35,15 @@
         'username': 'str',
         'password': 'str',
         'contact': 'list[ContactType]',
         'contact_default': 'int',
         'address': 'list[LocationType]',
         'address_default': 'int',
         'address_printable': 'str',
-        'birthdate': 'datetime',
+        'birthdate': 'date',
         'gdpr': 'bool',
         'tags': 'TagType',
         'document': 'DocumentMetadataType'
     }
 
     attribute_map = {
         'identifier': 'identifier',
@@ -362,26 +362,26 @@
     @property
     def birthdate(self):
         """Gets the birthdate of this IndividualType.  # noqa: E501
 
         Datum narození  # noqa: E501
 
         :return: The birthdate of this IndividualType.  # noqa: E501
-        :rtype: datetime
+        :rtype: date
         """
         return self._birthdate
 
     @birthdate.setter
     def birthdate(self, birthdate):
         """Sets the birthdate of this IndividualType.
 
         Datum narození  # noqa: E501
 
         :param birthdate: The birthdate of this IndividualType.  # noqa: E501
-        :type: datetime
+        :type: date
         """
 
         self._birthdate = birthdate
 
     @property
     def gdpr(self):
         """Gets the gdpr of this IndividualType.  # noqa: E501
```

### Comparing `sysnet-persons-1.0.0/persons/models/issuing_type.py` & `sysnet-persons-1.0.1/persons/models/issuing_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/location_type.py` & `sysnet-persons-1.0.1/persons/models/location_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -28,53 +28,58 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'ruian_adm': 'float',
         'street': 'str',
         'city': 'str',
         'zip': 'str',
+        'region': 'str',
         'country': 'CodeValueType',
         'address_list': 'list[str]',
         'note': 'str',
         'wgs': 'GeoPointType',
         'jtsk': 'GeoPointJtskType'
     }
 
     attribute_map = {
         'ruian_adm': 'ruianAdm',
         'street': 'street',
         'city': 'city',
         'zip': 'zip',
+        'region': 'region',
         'country': 'country',
         'address_list': 'addressList',
         'note': 'note',
         'wgs': 'wgs',
         'jtsk': 'jtsk'
     }
 
-    def __init__(self, ruian_adm=None, street=None, city=None, zip=None, country=None, address_list=None, note=None, wgs=None, jtsk=None):  # noqa: E501
+    def __init__(self, ruian_adm=None, street=None, city=None, zip=None, region=None, country=None, address_list=None, note=None, wgs=None, jtsk=None):  # noqa: E501
         """LocationType - a model defined in Swagger"""  # noqa: E501
         self._ruian_adm = None
         self._street = None
         self._city = None
         self._zip = None
+        self._region = None
         self._country = None
         self._address_list = None
         self._note = None
         self._wgs = None
         self._jtsk = None
         self.discriminator = None
         if ruian_adm is not None:
             self.ruian_adm = ruian_adm
         if street is not None:
             self.street = street
         if city is not None:
             self.city = city
         if zip is not None:
             self.zip = zip
+        if region is not None:
+            self.region = region
         if country is not None:
             self.country = country
         if address_list is not None:
             self.address_list = address_list
         if note is not None:
             self.note = note
         if wgs is not None:
@@ -171,14 +176,37 @@
         :param zip: The zip of this LocationType.  # noqa: E501
         :type: str
         """
 
         self._zip = zip
 
     @property
+    def region(self):
+        """Gets the region of this LocationType.  # noqa: E501
+
+        Kraj  # noqa: E501
+
+        :return: The region of this LocationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._region
+
+    @region.setter
+    def region(self, region):
+        """Sets the region of this LocationType.
+
+        Kraj  # noqa: E501
+
+        :param region: The region of this LocationType.  # noqa: E501
+        :type: str
+        """
+
+        self._region = region
+
+    @property
     def country(self):
         """Gets the country of this LocationType.  # noqa: E501
 
 
         :return: The country of this LocationType.  # noqa: E501
         :rtype: CodeValueType
         """
```

### Comparing `sysnet-persons-1.0.0/persons/models/mail_address_type.py` & `sysnet-persons-1.0.1/persons/models/mail_address_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/member_type.py` & `sysnet-persons-1.0.1/persons/models/member_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/person_link_type.py` & `sysnet-persons-1.0.1/persons/models/person_link_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/person_list_item.py` & `sysnet-persons-1.0.1/persons/models/person_list_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/person_type.py` & `sysnet-persons-1.0.1/persons/models/person_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/phone_number_type.py` & `sysnet-persons-1.0.1/persons/models/phone_number_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/reference_registry.py` & `sysnet-persons-1.0.1/persons/models/reference_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/role_category_type.py` & `sysnet-persons-1.0.1/persons/models/role_category_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/role_list_item.py` & `sysnet-persons-1.0.1/persons/models/role_list_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/role_type.py` & `sysnet-persons-1.0.1/persons/models/role_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/tag_item_type.py` & `sysnet-persons-1.0.1/persons/models/tag_item_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/models/tag_type.py` & `sysnet-persons-1.0.1/persons/models/tag_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `sysnet-persons-1.0.0/persons/rest.py` & `sysnet-persons-1.0.1/persons/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `sysnet-persons-1.0.0/pyproject.toml` & `sysnet-persons-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sysnet-persons"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Radim Jaeger", email="rjaeger@sysnet.cz" },
 ]
 description = "SYSNET Persons Registry REST API client"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `sysnet-persons-1.0.0/setup.py` & `sysnet-persons-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "persons"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `sysnet-persons-1.0.0/sysnet_persons.egg-info/PKG-INFO` & `sysnet-persons-1.0.1/sysnet_persons.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysnet-persons
-Version: 1.0.0
+Version: 1.0.1
 Summary: SYSNET Persons Registry REST API client
 Home-page: 
 Author-email: Radim Jaeger <rjaeger@sysnet.cz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,36 +212,35 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# persons
+# sysnet-persons
 This is a API to Persons Registry
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.0.0
-- Package version: 1.0.0
+- API version: 1.0.1
+- Package version: 1.0.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
-Python 2.7 and 3.4+
+Python 3.9+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on Github, you can install directly from Github
 
 ```sh
-pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
+pip install sysnet-persons
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)
 
 Then import the package:
 ```python
 import persons 
 ```
 
 ### Setuptools
@@ -391,26 +390,52 @@
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling AdminsApi->put_tag: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *https://service.sysnet.cz/persons/1.0.0*
+All URIs are relative to *https://service.sysnet.cz/persons/1.0.1*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *AdminsApi* | [**delete_tag**](docs/AdminsApi.md#delete_tag) | **DELETE** /tag/{name} | odstraní definici tagu  (cruD)
 *AdminsApi* | [**get_config**](docs/AdminsApi.md#get_config) | **GET** /config | získá konfiguraci konektoru
 *AdminsApi* | [**get_tag**](docs/AdminsApi.md#get_tag) | **GET** /tag/{name} | vrací definici tagu (cRud)
 *AdminsApi* | [**get_tag_list**](docs/AdminsApi.md#get_tag_list) | **GET** /tag | vrací seznam tagů v systému (autocomplete)
 *AdminsApi* | [**post_tag**](docs/AdminsApi.md#post_tag) | **POST** /tag | vytvoří nový tag (Crud)
 *AdminsApi* | [**put_config**](docs/AdminsApi.md#put_config) | **PUT** /config | aktualizuje hlavní konfiguraci konektoru
 *AdminsApi* | [**put_tag**](docs/AdminsApi.md#put_tag) | **PUT** /tag/{name} | aktualizuje definici tagu (crUd)
 *DevelopersApi* | [**info_api**](docs/DevelopersApi.md#info_api) | **GET** /info | vrací servisní informace
+*DevelopersApi* | [**info_api_head**](docs/DevelopersApi.md#info_api_head) | **HEAD** /info | vrací informaci o dostupnosti služby
+*LinkApi* | [**delete_individual_role**](docs/LinkApi.md#delete_individual_role) | **DELETE** /individual/role/{individual_id} | Odebere roli uživateli
+*LinkApi* | [**delete_person_member**](docs/LinkApi.md#delete_person_member) | **DELETE** /person/member/{person_id} | Odebere člena osobě
+*LinkApi* | [**delete_person_role**](docs/LinkApi.md#delete_person_role) | **DELETE** /person/role/{person_id} | Odebere roli osobě
+*LinkApi* | [**get_individual_roles**](docs/LinkApi.md#get_individual_roles) | **GET** /individual/role/{individual_id} | Získá všechny role pro uživatele
+*LinkApi* | [**get_person_members**](docs/LinkApi.md#get_person_members) | **GET** /person/member/{person_id} | Získá všechny uživatele pro osobu
+*LinkApi* | [**get_person_roles**](docs/LinkApi.md#get_person_roles) | **GET** /person/role/{person_id} | Získá všechny role pro osobu
+*LinkApi* | [**put_individual_role**](docs/LinkApi.md#put_individual_role) | **PUT** /individual/role/{individual_id} | Přiřadí uživateli roli
+*LinkApi* | [**put_person_member**](docs/LinkApi.md#put_person_member) | **PUT** /person/member/{person_id} | Přiřadí uživatela za člena osoby
+*LinkApi* | [**put_person_role**](docs/LinkApi.md#put_person_role) | **PUT** /person/role/{person_id} | Přiřadí osobě roli
+*ManageApi* | [**check_individuals**](docs/ManageApi.md#check_individuals) | **HEAD** /individual/data | Kontroluje existenci kolekce uživatelů
+*ManageApi* | [**check_persons**](docs/ManageApi.md#check_persons) | **HEAD** /person/data | Kontroluje existenci kolekce subjektů
+*ManageApi* | [**check_roles**](docs/ManageApi.md#check_roles) | **HEAD** /role/data | Kontroluje existenci kolekce rolí
+*ManageApi* | [**check_tags**](docs/ManageApi.md#check_tags) | **HEAD** /tag/data | Kontroluje existenci kolekce tagů
+*ManageApi* | [**export_individuals**](docs/ManageApi.md#export_individuals) | **GET** /individual/data | Exportuje všechny uživatele ve formátu BSON
+*ManageApi* | [**export_persons**](docs/ManageApi.md#export_persons) | **GET** /person/data | Exportuje všechny subjekty ve formátu BSON
+*ManageApi* | [**export_roles**](docs/ManageApi.md#export_roles) | **GET** /role/data | Exportuje všechny role ve formátu BSON
+*ManageApi* | [**export_tags**](docs/ManageApi.md#export_tags) | **GET** /tag/data | Exportuje všechny tagy ve formátu BSON
+*ManageApi* | [**import_individuals**](docs/ManageApi.md#import_individuals) | **PUT** /individual/data | Importuje uživatele
+*ManageApi* | [**import_individuals_replace**](docs/ManageApi.md#import_individuals_replace) | **POST** /individual/data | Nahradí všechny uživatele
+*ManageApi* | [**import_persons**](docs/ManageApi.md#import_persons) | **PUT** /person/data | Importuje subjekty
+*ManageApi* | [**import_persons_replace**](docs/ManageApi.md#import_persons_replace) | **POST** /person/data | Nahradí všechny subjekty
+*ManageApi* | [**import_roles**](docs/ManageApi.md#import_roles) | **PUT** /role/data | Importuje role
+*ManageApi* | [**import_roles_replace**](docs/ManageApi.md#import_roles_replace) | **POST** /role/data | Nahradí všechny role
+*ManageApi* | [**import_tags**](docs/ManageApi.md#import_tags) | **PUT** /tag/data | Importuje tagy
+*ManageApi* | [**import_tags_replace**](docs/ManageApi.md#import_tags_replace) | **POST** /tag/data | Nahradí všechny tagy
 *PublicApi* | [**delete_individual**](docs/PublicApi.md#delete_individual) | **DELETE** /individual/{identifier} | odstraní registrační dokument jednotlivce s daným identifikátorem (cruD)
 *PublicApi* | [**delete_person**](docs/PublicApi.md#delete_person) | **DELETE** /person/{identifier} | odstraní registrační dokument subjektu s daným identifikátorem (cruD)
 *PublicApi* | [**delete_role**](docs/PublicApi.md#delete_role) | **DELETE** /role/{identifier} | odstraní roli s daným identifikátorem (cruD)
 *PublicApi* | [**get_context**](docs/PublicApi.md#get_context) | **GET** /context/{identifier} | vrací kontext jednotlivce
 *PublicApi* | [**get_individual**](docs/PublicApi.md#get_individual) | **GET** /individual/{identifier} | vrací registrační dokument jednotlivce s daným identifikátorem (cRud)
 *PublicApi* | [**get_individual_list**](docs/PublicApi.md#get_individual_list) | **GET** /individual | vrací seznam jednotlivců (autocomplete)
 *PublicApi* | [**get_person**](docs/PublicApi.md#get_person) | **GET** /person/{identifier} | vrací registrační dokument subjektu s daným identifikátorem (cRud)
```

### Comparing `sysnet-persons-1.0.0/sysnet_persons.egg-info/SOURCES.txt` & `sysnet-persons-1.0.1/sysnet_persons.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 persons/__init__.py
 persons/api_client.py
 persons/configuration.py
 persons/rest.py
 persons/api/__init__.py
 persons/api/admins_api.py
 persons/api/developers_api.py
+persons/api/link_api.py
+persons/api/manage_api.py
 persons/api/public_api.py
 persons/models/__init__.py
 persons/models/code_value_type.py
 persons/models/config_body.py
 persons/models/contact_type.py
 persons/models/context_type.py
 persons/models/context_type_persons.py
@@ -56,16 +58,18 @@
 test/test_document_entry.py
 test/test_document_entry_list.py
 test/test_document_metadata_type.py
 test/test_geo_point_jtsk_type.py
 test/test_geo_point_type.py
 test/test_individual_type.py
 test/test_issuing_type.py
+test/test_link_api.py
 test/test_location_type.py
 test/test_mail_address_type.py
+test/test_manage_api.py
 test/test_member_type.py
 test/test_person_link_type.py
 test/test_person_list_item.py
 test/test_person_type.py
 test/test_phone_number_type.py
 test/test_public_api.py
 test/test_reference_registry.py
```

### Comparing `sysnet-persons-1.0.0/test/test_admins_api.py` & `sysnet-persons-1.0.1/test/test_admins_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_code_value_type.py` & `sysnet-persons-1.0.1/test/test_code_value_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_config_body.py` & `sysnet-persons-1.0.1/test/test_config_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_contact_type.py` & `sysnet-persons-1.0.1/test/test_contact_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_context_type.py` & `sysnet-persons-1.0.1/test/test_context_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_context_type_persons.py` & `sysnet-persons-1.0.1/test/test_context_type_persons.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_context_type_roles.py` & `sysnet-persons-1.0.1/test/test_context_type_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_department_type.py` & `sysnet-persons-1.0.1/test/test_department_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_developers_api.py` & `sysnet-persons-1.0.1/test/test_developers_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
@@ -31,10 +31,17 @@
     def test_info_api(self):
         """Test case for info_api
 
         vrací servisní informace  # noqa: E501
         """
         pass
 
+    def test_info_api_head(self):
+        """Test case for info_api_head
+
+        vrací informaci o dostupnosti služby  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sysnet-persons-1.0.0/test/test_document_entry.py` & `sysnet-persons-1.0.1/test/test_document_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_document_entry_list.py` & `sysnet-persons-1.0.1/test/test_document_entry_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_document_metadata_type.py` & `sysnet-persons-1.0.1/test/test_document_metadata_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_geo_point_jtsk_type.py` & `sysnet-persons-1.0.1/test/test_geo_point_jtsk_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_geo_point_type.py` & `sysnet-persons-1.0.1/test/test_geo_point_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_individual_type.py` & `sysnet-persons-1.0.1/test/test_individual_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_issuing_type.py` & `sysnet-persons-1.0.1/test/test_issuing_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_location_type.py` & `sysnet-persons-1.0.1/test/test_location_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_mail_address_type.py` & `sysnet-persons-1.0.1/test/test_mail_address_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_member_type.py` & `sysnet-persons-1.0.1/test/test_member_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_person_link_type.py` & `sysnet-persons-1.0.1/test/test_person_link_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_person_list_item.py` & `sysnet-persons-1.0.1/test/test_person_list_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_person_type.py` & `sysnet-persons-1.0.1/test/test_person_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_phone_number_type.py` & `sysnet-persons-1.0.1/test/test_phone_number_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_public_api.py` & `sysnet-persons-1.0.1/test/test_public_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_reference_registry.py` & `sysnet-persons-1.0.1/test/test_reference_registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_role_category_type.py` & `sysnet-persons-1.0.1/test/test_role_category_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_role_list_item.py` & `sysnet-persons-1.0.1/test/test_role_list_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_role_type.py` & `sysnet-persons-1.0.1/test/test_role_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_tag_item_type.py` & `sysnet-persons-1.0.1/test/test_tag_item_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `sysnet-persons-1.0.0/test/test_tag_type.py` & `sysnet-persons-1.0.1/test/test_tag_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Persons Registry API
 
     This is a API to Persons Registry  # noqa: E501
 
-    OpenAPI spec version: 1.0.0
+    OpenAPI spec version: 1.0.1
     Contact: info@sysnet.cz
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

