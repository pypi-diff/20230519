# Comparing `tmp/cgcsdk-0.8.5.tar.gz` & `tmp/cgcsdk-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-0.8.5.tar", last modified: Fri Apr 21 11:28:58 2023, max compression
+gzip compressed data, was "cgcsdk-0.8.6.tar", last modified: Fri May 19 13:18:09 2023, max compression
```

## Comparing `cgcsdk-0.8.5.tar` & `cgcsdk-0.8.6.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.495473 cgcsdk-0.8.5/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.5/LICENSE
--rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1101 2023-04-21 11:28:58.494476 cgcsdk-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.233253 cgcsdk-0.8.5/cgc/
--rw-rw-rw-   0        0        0      234 2023-04-21 11:23:47.000000 cgcsdk-0.8.5/cgc/.env
--rw-rw-rw-   0        0        0     3518 2023-04-21 11:25:14.000000 cgcsdk-0.8.5/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/__init__.py
--rw-rw-rw-   0        0        0     1327 2023-04-18 11:39:07.000000 cgcsdk-0.8.5/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.252297 cgcsdk-0.8.5/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.268926 cgcsdk-0.8.5/cgc/commands/auth/
--rw-rw-rw-   0        0        0      265 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1202 2023-02-17 10:49:54.000000 cgcsdk-0.8.5/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     3922 2023-03-22 14:29:23.000000 cgcsdk-0.8.5/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.288411 cgcsdk-0.8.5/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     2031 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.5/cgc/commands/cgc_cmd_responses.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.307542 cgcsdk-0.8.5/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.314019 cgcsdk-0.8.5/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.5/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.319918 cgcsdk-0.8.5/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.5/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.326249 cgcsdk-0.8.5/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/commands/resource/resource_cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.341671 cgcsdk-0.8.5/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.5/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.5/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/config.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.360074 cgcsdk-0.8.5/cgc/sdk/
--rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.5/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.5/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     1499 2023-04-18 10:58:48.000000 cgcsdk-0.8.5/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.367139 cgcsdk-0.8.5/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.374972 cgcsdk-0.8.5/cgc/tests/
--rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.5/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.406579 cgcsdk-0.8.5/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.5/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.5/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.441933 cgcsdk-0.8.5/cgc/utils/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2560 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.450100 cgcsdk-0.8.5/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1318 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1122 2023-03-23 11:15:14.000000 cgcsdk-0.8.5/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.464623 cgcsdk-0.8.5/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.5/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.5/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.5/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.5/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     1973 2023-02-15 11:40:43.000000 cgcsdk-0.8.5/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     4727 2023-03-23 11:24:38.000000 cgcsdk-0.8.5/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.5/cgc/utils/update.py
--rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.5/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:28:58.491014 cgcsdk-0.8.5/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     1101 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 11:28:58.000000 cgcsdk-0.8.5/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 11:28:58.496458 cgcsdk-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.783755 cgcsdk-0.8.6/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-02-15 12:59:37.000000 cgcsdk-0.8.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1101 2023-05-19 13:18:09.781681 cgcsdk-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.506079 cgcsdk-0.8.6/cgc/
+-rw-rw-rw-   0        0        0      261 2023-05-19 13:13:56.000000 cgcsdk-0.8.6/cgc/.env
+-rw-rw-rw-   0        0        0     3921 2023-05-19 13:08:19.000000 cgcsdk-0.8.6/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-05-18 09:42:45.000000 cgcsdk-0.8.6/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.528270 cgcsdk-0.8.6/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.547596 cgcsdk-0.8.6/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-0.8.6/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-19 11:45:44.000000 cgcsdk-0.8.6/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1783 2023-05-19 13:13:56.000000 cgcsdk-0.8.6/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     3893 2023-05-18 13:54:23.000000 cgcsdk-0.8.6/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.565073 cgcsdk-0.8.6/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     3450 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4696 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4006 2023-05-19 13:07:28.000000 cgcsdk-0.8.6/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2026 2023-04-21 11:24:43.000000 cgcsdk-0.8.6/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1207 2023-05-19 10:34:54.000000 cgcsdk-0.8.6/cgc/commands/cgc_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.588482 cgcsdk-0.8.6/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0     4783 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      925 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5175 2023-04-18 11:02:46.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     3353 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.596198 cgcsdk-0.8.6/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3293 2023-04-18 10:50:41.000000 cgcsdk-0.8.6/cgc/commands/db/db_cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.603014 cgcsdk-0.8.6/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-0.8.6/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.609498 cgcsdk-0.8.6/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     3156 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/commands/resource/resource_cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.631504 cgcsdk-0.8.6/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-03-22 14:29:23.000000 cgcsdk-0.8.6/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     6784 2023-03-22 14:29:23.000000 cgcsdk-0.8.6/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/config.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.652733 cgcsdk-0.8.6/cgc/sdk/
+-rw-rw-rw-   0        0        0      194 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/sdk/handlers.py
+-rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-0.8.6/cgc/sdk/mongodb.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-0.8.6/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0     2786 2023-05-18 09:34:33.000000 cgcsdk-0.8.6/cgc/sdk/redis.py
+-rw-rw-rw-   0        0        0     1452 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.661237 cgcsdk-0.8.6/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-0.8.6/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.670280 cgcsdk-0.8.6/cgc/tests/
+-rw-rw-rw-   0        0        0   102744 2023-04-18 11:02:26.000000 cgcsdk-0.8.6/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.706000 cgcsdk-0.8.6/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-0.8.6/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-0.8.6/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.739237 cgcsdk-0.8.6/cgc/utils/
+-rw-rw-rw-   0        0        0     3405 2023-05-19 13:08:19.000000 cgcsdk-0.8.6/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-0.8.6/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2729 2023-05-19 13:09:02.000000 cgcsdk-0.8.6/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.747617 cgcsdk-0.8.6/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-05-18 13:48:23.000000 cgcsdk-0.8.6/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1112 2023-05-19 08:15:55.000000 cgcsdk-0.8.6/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.760738 cgcsdk-0.8.6/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-0.8.6/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2067 2023-03-08 09:29:27.000000 cgcsdk-0.8.6/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1556 2023-02-20 14:42:03.000000 cgcsdk-0.8.6/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2354 2023-02-17 10:02:49.000000 cgcsdk-0.8.6/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     1973 2023-05-18 13:28:20.000000 cgcsdk-0.8.6/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     4913 2023-05-19 13:09:48.000000 cgcsdk-0.8.6/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-0.8.6/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     2959 2023-04-18 09:56:45.000000 cgcsdk-0.8.6/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2023-05-19 13:18:09.779093 cgcsdk-0.8.6/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     1101 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2446 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      124 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-19 13:18:09.000000 cgcsdk-0.8.6/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-0.8.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 13:18:09.784922 cgcsdk-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-04-18 10:14:17.000000 cgcsdk-0.8.6/setup.py
```

### Comparing `cgcsdk-0.8.5/PKG-INFO` & `cgcsdk-0.8.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.5/cgc/CHANGELOG.md` & `cgcsdk-0.8.6/cgc/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Change Log
 
+## 0.8.6
+
+Release on May 19, 2023.
+
+* added get_redis_client_async() for RedisConnector
+* get_redis_access() - async_client: bool, new parameter
+* new command: cgc context switch [number]
+  * switch between user contexts
+* new command: cgc context list
+  * list all configuration files
+* updated command: cgc register
+  * allow to have multiple user contexts
+* increased timeout for requests to 30 sec
+
 ## 0.8.5
 
 Release on Apr 21, 2023.
 
 * update for cgc status: resource_keys in cgc_status_response
 
 ## 0.8.4
```

### Comparing `cgcsdk-0.8.5/cgc/cgc.py` & `cgcsdk-0.8.6/cgc/cgc.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 
 from cgc.commands.debug.debug_cmd import debug_group
 from cgc.commands.cgc_cmd import (
     cgc_rm,
     cgc_status,
     sending_telemetry_permission,
     resource_events,
+    context_group,
 )
 from cgc.utils.version_control import check_version, _get_version
 from cgc.utils.click_group import CustomGroup
 
 
 @click.group(cls=CustomGroup)
 @click.version_option(_get_version())
 def cli():
     """CGC application developed by Comtegra S.A."""
     check_version()
 
 
 cli.add_command(debug_group)
+cli.add_command(context_group)
 cli.add_command(auth_register)
 cli.add_command(api_keys_group)
 cli.add_command(volume_group)
 cli.add_command(compute_group)
 cli.add_command(db_group)
 cli.add_command(cgc_rm)
 cli.add_command(resource_events)
```

### Comparing `cgcsdk-0.8.5/cgc/commands/auth/auth_cmd.py` & `cgcsdk-0.8.6/cgc/commands/auth/auth_cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,47 +3,58 @@
 from cgc.commands.auth.auth_responses import (
     auth_register_response,
     login_successful_response,
 )
 from cgc.commands.auth.auth_utils import (
     auth_create_api_key_with_save,
 )
-
 from cgc.utils.prepare_headers import get_url_and_prepare_headers_register
 from cgc.utils.cryptography import rsa_crypto
 from cgc.utils.click_group import CustomCommand, CustomGroup
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
+from cgc.utils import (
+    check_if_config_exist,
+    require_confirm_loop,
+    find_first_available_config_name,
+)
 
 
 @click.group("api-keys", cls=CustomGroup, hidden=True)
 def api_keys_group():
     """
     Management of API keys.
     """
     pass
 
 
 @click.command("register", cls=CustomCommand)
-@click.option("--user_id", "-u", "user_id", prompt=True)
-@click.option("--access_key", "-k", "access_key", prompt=True)
-def auth_register(user_id: str, access_key: str):
+# @click.option("--user_id", "-u", "user_id", prompt=True)
+# @click.option("--access_key", "-k", "access_key", prompt=True)
+def auth_register(config_filename: str = "cfg.json"):
     """Register a user in system using user id and access key.\n
     Enabling/Disabling Telemetry sending is available, if set to yes CGC will send
     usage metrics for application improvements purposes.
     \f
     :param user_id: username received in invite
     :type user_id: str
     :param access_key: access key received in invite
     :type access_key: str
     :paaram telemetry_sending: if set to yes CGC will send
     usage metrics for application improvements purposes
     :type telemetry_sending: bool
     """
 
+    if check_if_config_exist(config_filename):
+        click.echo("Already registered.")
+        require_confirm_loop("Do you want to add new context?")
+        config_filename = find_first_available_config_name()
+
+    user_id = input("User ID: ")
+    access_key = input("Access key: ")
     url, headers = get_url_and_prepare_headers_register(user_id, access_key)
     metric = "auth.register"
     pub_key_bytes, priv_key_bytes = rsa_crypto.key_generate_pair()
     __payload = pub_key_bytes
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
@@ -52,14 +63,15 @@
         allow_redirects=True,
     )
     click.echo(
         auth_register_response(
             retrieve_and_validate_response_send_metric(__res, metric, False),
             user_id,
             priv_key_bytes,
+            config_filename,
         )
     )
 
 
 @api_keys_group.command("create", cls=CustomCommand)
 def api_keys_create():
     """Login a user in system using user id and password, then creates new API key pair and overwrites existing.
```

### Comparing `cgcsdk-0.8.5/cgc/commands/auth/auth_responses.py` & `cgcsdk-0.8.6/cgc/commands/auth/auth_responses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import shutil
 import os
 
 from cgc.commands.auth import auth_utils
-from cgc.utils.consts.env_consts import TMP_DIR
-from cgc.utils.config_utils import get_config_path, save_to_config, user_config_file
+from cgc.utils.consts.env_consts import TMP_DIR, get_config_file_name
+from cgc.utils.config_utils import get_config_path, save_to_config
 from cgc.utils.message_utils import key_error_decorator_for_helpers
 
 
 @key_error_decorator_for_helpers
-def auth_register_response(response, user_id, priv_key_bytes) -> str:
+def auth_register_response(response, user_id, priv_key_bytes, config_filename) -> str:
     TMP_DIR_PATH = os.path.join(get_config_path(), TMP_DIR)
-    unzip_dir = auth_utils.save_and_unzip_file(response)
+    unzip_dir, namespace = auth_utils.save_and_unzip_file(response)
     aes_key, password = auth_utils.get_aes_key_and_password(unzip_dir, priv_key_bytes)
 
-    save_to_config(user_id=user_id, password=password, aes_key=aes_key)
+    os.environ["CONFIG_FILE_NAME"] = config_filename
+    save_to_config(
+        user_id=user_id, password=password, aes_key=aes_key, namespace=namespace
+    )
     auth_utils.auth_create_api_key_with_save()
     shutil.rmtree(TMP_DIR_PATH)
-    return f"Register successful! You can now use the CLI. Saved data to: {user_config_file}\n\
-        Consider backup this file. It stores data with which you can access CGC platform."
+    # config.json
+    if config_filename == "config.json":
+        return f"Register successful! You can now use the CLI. Saved data to:{os.path.join(get_config_path(),config_filename)}\n\
+        Consider backup this file. It stores data accessible only to you with which you can access CGC platform."
+    return f"New context created successfully! \nNew config file saved to: {os.path.join(get_config_path(),config_filename)}\n\
+Consider backup this file. It stores data accessible only to you with which you can access CGC platform.\n \n\
+To switch context use \ncgc context switch"
 
 
 @key_error_decorator_for_helpers
 def login_successful_response():
     return f"Successfully logged in, created new API key pair.\n\
-                Saved data to: {user_config_file}.\n\
-                Consider backup this file. It stores data with which you can access CGC platform."
+                Saved data to: {os.path.join(get_config_path(), get_config_file_name())}.\n\
+                Consider backup this file. It stores data accessible only to you with which you can access CGC platform."
```

### Comparing `cgcsdk-0.8.5/cgc/commands/auth/auth_utils.py` & `cgcsdk-0.8.6/cgc/commands/auth/auth_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,26 +72,25 @@
     :param res: API response with file to save and unzip
     :type res: requests.Response
     :return: path to the directory containing the file
     :rtype: str
     """
     zip_file = res.headers.get("content-disposition").split('"')[1]
     namespace = zip_file.split("---")[-1].split(".")[0]
-    save_to_config(namespace=namespace)
 
     if not os.path.isdir(TMP_DIR_PATH):
         os.makedirs(TMP_DIR_PATH)
     zip_file_path = f"{TMP_DIR_PATH}/{zip_file}"
     with open(zip_file_path, "wb") as f:
         f.write(res.content)
 
     unzip_dir = zip_file_path[:-4]
     shutil.unpack_archive(zip_file_path, unzip_dir)
 
-    return unzip_dir
+    return unzip_dir, namespace
 
 
 def get_aes_key_and_password(unzip_dir: str, priv_key_bytes: bytes):
     """Function to get AES key and password from the unzipped file.
 
     :param unzip_dir: path to the directory containing the file
     :type unzip_dir: str
```

### Comparing `cgcsdk-0.8.5/cgc/commands/billing/__init__.py` & `cgcsdk-0.8.6/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/billing/billing_cmd.py` & `cgcsdk-0.8.6/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/billing/billing_responses.py` & `cgcsdk-0.8.6/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/billing/billing_utils.py` & `cgcsdk-0.8.6/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/cgc_cmd.py` & `cgcsdk-0.8.6/cgc/commands/resource/resource_cmd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,100 @@
 import click
 import json
 
-from cgc.commands.cgc_cmd_responses import cgc_status_response
-from cgc.commands.resource.resource_cmd import resource_delete
-from cgc.utils.requests_helper import call_api, EndpointTypes
-from cgc.utils.click_group import CustomCommand
+from cgc.commands.compute.compute_models import EntityList, DatabasesList
+from cgc.commands.compute.compute_responses import (
+    template_list_response,
+    template_get_start_path_response,
+    compute_restart_response,
+    compute_delete_response,
+)
+
+from cgc.commands.compute.compute_utills import compute_delete_payload
+
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
-from cgc.telemetry.basic import telemetry_permission_set
-from cgc.commands.compute.compute_responses import compute_logs_response
+from cgc.utils.click_group import CustomGroup, CustomCommand
+from cgc.utils.requests_helper import call_api, EndpointTypes
 
 
-@click.command("rm", cls=CustomCommand)
-@click.argument("name", type=click.STRING)
-def cgc_rm(name: str):
+@click.group(name="resource", cls=CustomGroup, hidden=True)
+def resource_group():
     """
-    Delete an app in user namespace
+    Management of templates.
     """
-    resource_delete(name)
 
 
-@click.command("events", cls=CustomCommand)
-@click.argument("app_name", type=click.STRING)
-def resource_events(app_name: str):
-    """Get events of given app"""
+@resource_group.command("list_templates", cls=CustomCommand)
+def template_list():
+    """Lists all available templates"""
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/get_pod_events"
-    metric = "resource.events"
-    __payload = {"name": app_name}
-    __res = call_api(
-        request=EndpointTypes.get,
-        url=url,
-        headers=headers,
-        data=json.dumps(__payload),
+    url = f"{api_url}/v1/api/resource/list_available_templates"
+    metric = "resource.template.list"
+    __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
+    click.echo(
+        template_list_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
+
+
+@resource_group.command("get_start_path", cls=CustomCommand)
+@click.argument(
+    "template", type=click.Choice([*EntityList.get_list(), *DatabasesList.get_list()])
+)
+def template_get_start_path(template: str):
+    """Displays start path of specified template"""
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/get_template_start_path?template_name={template}"
+    metric = "resource.template.get_start_path"
+    __res = call_api(request=EndpointTypes.get, url=url, headers=headers)
     click.echo(
-        compute_logs_response(retrieve_and_validate_response_send_metric(__res, metric))
+        template_get_start_path_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
 
 
-@click.command("status", cls=CustomCommand)
-def cgc_status():
-    """Lists available and used resources"""
+@resource_group.command("restart", cls=CustomCommand)
+@click.argument("name", type=click.STRING)
+def compute_restart(name: str):
+    """Restarts the specified app"""
     api_url, headers = get_api_url_and_prepare_headers()
-    url = f"{api_url}/v1/api/resource/status"
-    metric = "resource.status"
+    url = f"{api_url}/v1/api/resource/restart"
+    metric = "resource.restart"
+    __payload = {"name": name}
     __res = call_api(
-        request=EndpointTypes.get,
+        request=EndpointTypes.post,
         url=url,
         headers=headers,
+        data=json.dumps(__payload),
     )
     click.echo(
-        cgc_status_response(retrieve_and_validate_response_send_metric(__res, metric))
+        compute_restart_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
 
 
-@click.command("telemetry", cls=CustomCommand)
-def sending_telemetry_permission():
-    """Changing permission for sending telemetry"""
-
+def resource_delete(name: str):
+    """
+    Delete an app using backend endpoint.
+    \f
+    :param name: name of app to delete
+    :type name: str
+    """
+    api_url, headers = get_api_url_and_prepare_headers()
+    url = f"{api_url}/v1/api/resource/delete"
+    metric = "resource.delete"
+    __payload = compute_delete_payload(name=name)
+    __res = call_api(
+        request=EndpointTypes.delete,
+        url=url,
+        headers=headers,
+        data=json.dumps(__payload),
+    )
     click.echo(
-        f"Sending telemetry is now {'enabled' if telemetry_permission_set() else 'disabled'}"
+        compute_delete_response(
+            retrieve_and_validate_response_send_metric(__res, metric)
+        )
     )
```

### Comparing `cgcsdk-0.8.5/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-0.8.6/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/compute/compute_cmd.py` & `cgcsdk-0.8.6/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/compute/compute_models.py` & `cgcsdk-0.8.6/cgc/commands/compute/compute_models.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/compute/compute_responses.py` & `cgcsdk-0.8.6/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/compute/compute_utills.py` & `cgcsdk-0.8.6/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/db/db_cmd.py` & `cgcsdk-0.8.6/cgc/commands/db/db_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/volume/data_model.py` & `cgcsdk-0.8.6/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/volume/volume_cmd.py` & `cgcsdk-0.8.6/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/volume/volume_responses.py` & `cgcsdk-0.8.6/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/commands/volume/volume_utils.py` & `cgcsdk-0.8.6/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/sdk/handlers.py` & `cgcsdk-0.8.6/cgc/sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/sdk/mongodb.py` & `cgcsdk-0.8.6/cgc/sdk/mongodb.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/sdk/postgresql.py` & `cgcsdk-0.8.6/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/sdk/redis.py` & `cgcsdk-0.8.6/cgc/sdk/redis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,88 @@
-from redis import Redis, ConnectionError
+from redis.asyncio import redis as redis_async
+import redis
 
 
 class RedisConnector:
+    redis_client_async = None
+    redis_client = None
+
     def __init__(
         self, host: str, password: str = None, decode_responses: bool = False
     ) -> None:
         self._host = host
         assert type(host) is str
         "host must be a str containing redis app name"
         self._password = password
         self._decode_responses = decode_responses
-        self.connect()
 
-    def connect(self):
+    def connect(self, async_client: bool = False):
         while True:
             try:
-                self._redis_client = Redis(
-                    host=self._host,
-                    port=6379,
-                    password=self._password,
-                    decode_responses=self._decode_responses,
-                )
+                if not async_client:
+                    self.redis_client = redis.Redis(
+                        host=self._host,
+                        port=6379,
+                        password=self._password,
+                        decode_responses=self._decode_responses,
+                    )
+                else:
+                    self.redis_client_async = redis_async.Redis(
+                        host=self._host,
+                        port=6379,
+                        password=self._password,
+                        decode_responses=self._decode_responses,
+                    )
                 print(f"Connected to Redis: {self._host}")
                 break
-            except (ConnectionError,) as e:
+            except (redis.ConnectionError,) as e:
                 print(f"Redis connection error: {e}")
                 print(f"retrying to connect...")
 
     def get_redis_client(self):
-        return self._redis_client
+        if self.redis_client is None:
+            self.connect()
+        return self.redis_client
+
+    def get_redis_client_async(self):
+        if self.redis_client_async is None:
+            self.connect(async_client=True)
+        return self.redis_client_async
 
 
 def get_redis_access(
-    app_name: str, password: str, decode_responses: bool = False, restart: bool = False
+    app_name: str,
+    password: str,
+    decode_responses: bool = False,
+    restart: bool = False,
+    async_client=False,
 ):
     global _redis_access
+    global _redis_access_async
 
-    def init_access():
+    def init_access(async_client=False):
         global _redis_access
-        _redis_access = RedisConnector(
-            host=app_name, password=password, decode_responses=decode_responses
-        )
+        global _redis_access_async
+
+        if not async_client:
+            _redis_access = RedisConnector(
+                host=app_name, password=password, decode_responses=decode_responses
+            )
+        else:
+            _redis_access_async = RedisConnector(
+                host=app_name, password=password, decode_responses=decode_responses
+            )
 
     try:
-        if not isinstance(_redis_access, RedisConnector) or restart:
-            init_access()
+        if not async_client:
+            if not isinstance(_redis_access, RedisConnector) or restart:
+                init_access()
+        else:
+            if not isinstance(_redis_access_async, RedisConnector) or restart:
+                init_access(True)
     except NameError:
-        init_access()
+        if not async_client:
+            init_access()
+        else:
+            init_access(True)
         pass
-    return _redis_access
+    return _redis_access if async_client else _redis_access_async
```

### Comparing `cgcsdk-0.8.5/cgc/server.crt` & `cgcsdk-0.8.6/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/telemetry/basic.py` & `cgcsdk-0.8.6/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/tests/__init__.py` & `cgcsdk-0.8.6/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-0.8.6/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-0.8.6/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-0.8.6/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/tests/responses_tests.py` & `cgcsdk-0.8.6/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/click_group.py` & `cgcsdk-0.8.6/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/config_utils.py` & `cgcsdk-0.8.6/cgc/utils/config_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import json
 import os
 import sys
 import click
 
-from cgc.commands.auth import NoNamespaceInConfig
+from cgc.commands.auth import NoNamespaceInConfig, NoConfigFileFound
 from cgc.utils.message_utils import prepare_error_message
-from cgc.utils.consts.env_consts import (
-    CONFIG_FILE_NAME,
-)
+from cgc.utils.consts.env_consts import get_config_file_name
 
 
 def get_config_path():
     """Function to get the path to the config file
 
     :return: path to the config file
     :rtype: str
@@ -28,56 +26,59 @@
         click.echo(prepare_error_message(message))
         sys.exit()
 
     return config_path
 
 
 config_path = get_config_path()
-user_config_file = os.path.join(config_path, CONFIG_FILE_NAME)
 
 
 def save_to_config(**kwargs):
     """Function allowing adding a variable number of key-value pairs to the config file.
     If config file does not exist, it is created, otherwise key-value pairs are appended to existing config.
     Values for existing keys are overwritten.
 
     :param kwargs: key-value pairs to be saved in the config file
     :type kwargs: dict
     """
     read_cfg = {}
+    user_config_file = os.path.join(config_path, get_config_file_name())
     if not os.path.isdir(config_path):
         os.makedirs(config_path)
     try:
         f = open(user_config_file, "r+", encoding="UTF-8")
         read_cfg = json.load(f)
     except FileNotFoundError:
         pass
 
     with open(user_config_file, "w", encoding="UTF-8") as f:
         final_cfg = {**read_cfg, **kwargs}
         json.dump(final_cfg, f)
 
 
-def read_from_cfg(key: str):
+def read_from_cfg(key: str, filename=None):
     """Function to read a single value from config
 
     :param key: key name to read the value from config
     :type key: str
     :return: value for the provided key
     :rtype: _type_
     """
+    if filename is None:
+        filename_with_path = os.path.join(config_path, get_config_file_name())
+    else:
+        filename_with_path = os.path.join(config_path, filename)
     try:
-        f = open(user_config_file, "r+", encoding="UTF-8")
-        read_cfg = json.load(f)
-        return read_cfg[key]
+        with open(filename_with_path, "r+", encoding="UTF-8") as f:
+            read_cfg = json.load(f)
+            if key is None:
+                return read_cfg
+            return read_cfg[key]
     except FileNotFoundError:
-        if key == "namespace":
-            raise NoNamespaceInConfig()
-        print("No config file found. Please use cgc register first.")
-        sys.exit()
+        raise NoConfigFileFound()
     except KeyError:
         if key == "namespace":
             raise NoNamespaceInConfig()
         print("Config file is corrupted. Please contact support at support@comtegra.pl")
         sys.exit()
```

### Comparing `cgcsdk-0.8.5/cgc/utils/consts/env_consts.py` & `cgcsdk-0.8.6/cgc/utils/consts/env_consts.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,12 +32,15 @@
 elif API_SECURE_CONNECTION == "no":
     __prefix = "http"
 else:
     raise Exception("not defined API_SECURE_CONNECTION. set yes/no")
 
 API_PORT = os.getenv("API_PORT")
 API_URL = f"{__prefix}://{API_HOST}:{API_PORT}"
-CONFIG_FILE_NAME = os.getenv("CONFIG_FILE_NAME")
 TMP_DIR = os.getenv("TMP_DIR")
 RELEASE = int(os.getenv("RELEASE"))
 MAJOR_VERSION = int(os.getenv("MAJOR_VERSION"))
 MINOR_VERSION = int(os.getenv("MINOR_VERSION"))
+
+
+def get_config_file_name():
+    return os.getenv("CONFIG_FILE_NAME")
```

### Comparing `cgcsdk-0.8.5/cgc/utils/consts/message_consts.py` & `cgcsdk-0.8.6/cgc/utils/consts/message_consts.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 DISABLED_ERROROUTDATED_MAJOR = (
     "You are using outdated version of cgcsdk, please update to the latest version."
 )
 OUTDATED_MINOR = "There is a new release available, consider updating the application."
 OUTDATED_MAJOR = (
     "You are using outdated version of cgcsdk, please update to the latest version."
 )
-UNAUTHORIZED_ERROR = "Unauthorized. Please check your API key and secret key or contact support at support@comtegra.pl"
+UNAUTHORIZED_ERROR = "Unauthorized. Credentials provided are invalid. Contact support at support@comtegra.pl"
 DISABLED_ERROR = "Account has been disabled. If you require assistance, please contact support at support@comtegra.pl"
 ENDPOINT_DISABLED = "Endpoint is currently disabled, please try again later or contact support for additional information at support@comtegra.pl"
```

### Comparing `cgcsdk-0.8.5/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-0.8.6/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-0.8.6/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-0.8.6/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/custom_exceptions.py` & `cgcsdk-0.8.6/cgc/utils/custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/message_utils.py` & `cgcsdk-0.8.6/cgc/utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/prepare_headers.py` & `cgcsdk-0.8.6/cgc/utils/prepare_headers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgc/utils/requests_helper.py` & `cgcsdk-0.8.6/cgc/utils/requests_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     get = requests.get
     post = requests.post
     delete = requests.delete
 
 
 def _process_endpoint_kwargs(**kwargs):
     if not "timeout" in kwargs.keys():
-        kwargs["timeout"] = 10
+        kwargs["timeout"] = 30
     return kwargs
 
 
 def _call_rest_endpoint(request: EndpointTypes, **kwargs):
     kwargs = _process_endpoint_kwargs(**kwargs)
     return request(**kwargs)
```

### Comparing `cgcsdk-0.8.5/cgc/utils/response_utils.py` & `cgcsdk-0.8.6/cgc/utils/response_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import click
 import pprint
 import requests
 import json
 from tabulate import tabulate
-from cgc.commands.auth import NoNamespaceInConfig
+from cgc.commands.auth import NoNamespaceInConfig, NoConfigFileFound
 from cgc.utils.message_utils import prepare_error_message
 from cgc.utils.consts.message_consts import (
     UNKNOWN_ERROR,
     UNAUTHORIZED_ERROR,
     DISABLED_ERROR,
     ENDPOINT_DISABLED,
 )
@@ -34,14 +34,18 @@
     error_message = UNKNOWN_ERROR
     try:
         try:
             if metric is not None:
                 metric = f"{get_namespace()}.{metric}"
         except NoNamespaceInConfig:
             metric = f"unknown-namespace.{metric}"
+        except NoConfigFileFound:
+            print("No config file found. Please use:")
+            print("cgc register")
+            metric = f"bad-client.{metric}"
 
         if response.status_code == 200:
             increment_metric(
                 metric=metric, is_error=False
             )  # if metric is None, will not increment metric
             if json_return:
                 return response.json()
```

### Comparing `cgcsdk-0.8.5/cgc/utils/version_control.py` & `cgcsdk-0.8.6/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-0.8.5/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-0.8.6/cgcsdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 0.8.5
+Version: 0.8.6
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
```

### Comparing `cgcsdk-0.8.5/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-0.8.6/cgcsdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 cgc/__init__.py
 cgc/cgc.py
 cgc/config.py
 cgc/server.crt
 cgc/commands/__init__.py
 cgc/commands/cgc_cmd.py
 cgc/commands/cgc_cmd_responses.py
+cgc/commands/cgc_helpers.py
 cgc/commands/exceptions.py
 cgc/commands/auth/__init__.py
 cgc/commands/auth/auth_cmd.py
 cgc/commands/auth/auth_responses.py
 cgc/commands/auth/auth_utils.py
 cgc/commands/billing/__init__.py
 cgc/commands/billing/billing_cmd.py
```

### Comparing `cgcsdk-0.8.5/setup.py` & `cgcsdk-0.8.6/setup.py`

 * *Files identical despite different names*

