# Comparing `tmp/sila2-0.9.1.tar.gz` & `tmp/sila2-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nme\Projects\sila_python\dist\tmpt9e0h3wb\sila2-0.9.1.tar", last modified: Thu Jul 28 08:30:15 2022, max compression
+gzip compressed data, was "C:\Users\nme\Projects\sila_python\dist\tmpnlxnu2g2\sila2-0.9.2.tar", last modified: Mon Aug  1 21:23:29 2022, max compression
```

## Comparing `sila2-0.9.1.tar` & `sila2-0.9.2.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/
--rw-rw-rw-   0        0        0     1092 2022-07-08 09:18:19.000000 sila2-0.9.1/LICENSE
--rw-rw-rw-   0        0        0     8618 2022-07-28 08:30:15.000000 sila2-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     6245 2022-07-08 09:18:19.000000 sila2-0.9.1/README.md
--rw-rw-rw-   0        0        0     3167 2022-07-28 08:29:57.000000 sila2-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-07-28 08:30:15.000000 sila2-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     1486 2022-07-08 09:18:19.000000 sila2-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/
--rw-rw-rw-   0        0        0      692 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/client/
--rw-rw-rw-   0        0        0     1093 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/__init__.py
--rw-rw-rw-   0        0        0     2831 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_feature.py
--rw-rw-rw-   0        0        0     2466 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_metadata.py
--rw-rw-rw-   0        0        0     2733 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_observable_command.py
--rw-rw-rw-   0        0        0     8694 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_observable_command_instance.py
--rw-rw-rw-   0        0        0     2471 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_observable_property.py
--rw-rw-rw-   0        0        0     1958 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_unobservable_command.py
--rw-rw-rw-   0        0        0     2695 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/client_unobservable_property.py
--rw-rw-rw-   0        0        0     1739 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/execution_info_subscription_thread.py
--rw-rw-rw-   0        0        0     1588 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/grpc_stream_subscription.py
--rw-rw-rw-   0        0        0     1689 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/polling_subscription.py
--rw-rw-rw-   0        0        0     9346 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/sila_client.py
--rw-rw-rw-   0        0        0     2115 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/client/subscription.py
--rw-rw-rw-   0        0        0     3876 2022-07-25 13:53:28.000000 sila2-0.9.1/src/sila2/client/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/code_generator/
--rw-rw-rw-   0        0        0      310 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/__init__.py
--rw-rw-rw-   0        0        0     8653 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/__main__.py
--rw-rw-rw-   0        0        0     7778 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/code_generator.py
--rw-rw-rw-   0        0        0     2271 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/code_generator_base.py
--rw-rw-rw-   0        0        0    10445 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/feature_generator.py
--rw-rw-rw-   0        0        0      389 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_environment.py
--rw-rw-rw-   0        0        0      429 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_loader.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/code_generator/template_objects/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_objects/__init__.py
--rw-rw-rw-   0        0        0     1236 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_objects/base.py
--rw-rw-rw-   0        0        0     3112 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_objects/basics.py
--rw-rw-rw-   0        0        0     1322 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_objects/client.py
--rw-rw-rw-   0        0        0     1194 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/code_generator/template_objects/types.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/discovery/
--rw-rw-rw-   0        0        0       96 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/discovery/__init__.py
--rw-rw-rw-   0        0        0      754 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/discovery/broadcaster.py
--rw-rw-rw-   0        0        0     3502 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/discovery/browser.py
--rw-rw-rw-   0        0        0     5113 2022-07-25 12:20:26.000000 sila2-0.9.1/src/sila2/discovery/listener.py
--rw-rw-rw-   0        0        0     1267 2022-07-25 13:48:58.000000 sila2-0.9.1/src/sila2/discovery/service_info.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/features/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/features/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/features/authenticationservice/
--rw-rw-rw-   0        0        0     5274 2022-07-08 09:33:03.000000 sila2-0.9.1/src/sila2/features/authenticationservice/AuthenticationService.sila.xml
--rw-rw-rw-   0        0        0      664 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authenticationservice/__init__.py
--rw-rw-rw-   0        0        0     1887 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_base.py
--rw-rw-rw-   0        0        0     1693 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_client.py
--rw-rw-rw-   0        0        0      937 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_errors.py
--rw-rw-rw-   0        0        0      238 2022-07-08 09:33:03.000000 sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_feature.py
--rw-rw-rw-   0        0        0      552 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_types.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/
--rw-rw-rw-   0        0        0     3614 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/AuthorizationProviderService.sila.xml
--rw-rw-rw-   0        0        0      698 2022-07-08 09:33:06.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/__init__.py
--rw-rw-rw-   0        0        0     1151 2022-07-08 09:33:05.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_base.py
--rw-rw-rw-   0        0        0     1023 2022-07-08 09:33:05.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_client.py
--rw-rw-rw-   0        0        0     1040 2022-07-08 09:33:06.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_errors.py
--rw-rw-rw-   0        0        0      252 2022-07-08 09:33:04.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_feature.py
--rw-rw-rw-   0        0        0      331 2022-07-08 09:33:06.000000 sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_types.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/features/authorizationservice/
--rw-rw-rw-   0        0        0     1319 2022-07-08 09:33:06.000000 sila2-0.9.1/src/sila2/features/authorizationservice/AuthorizationService.sila.xml
--rw-rw-rw-   0        0        0      478 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/authorizationservice/__init__.py
--rw-rw-rw-   0        0        0      992 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_base.py
--rw-rw-rw-   0        0        0      824 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_client.py
--rw-rw-rw-   0        0        0      606 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_errors.py
--rw-rw-rw-   0        0        0      236 2022-07-08 09:33:06.000000 sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_feature.py
--rw-rw-rw-   0        0        0       99 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_types.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/features/lockcontroller/
--rw-rw-rw-   0        0        0     5480 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/lockcontroller/LockController.sila.xml
--rw-rw-rw-   0        0        0      654 2022-07-08 09:33:11.000000 sila2-0.9.1/src/sila2/features/lockcontroller/__init__.py
--rw-rw-rw-   0        0        0     3286 2022-07-08 09:33:11.000000 sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_base.py
--rw-rw-rw-   0        0        0     2793 2022-07-08 09:33:11.000000 sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_client.py
--rw-rw-rw-   0        0        0     1273 2022-07-08 09:33:11.000000 sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_errors.py
--rw-rw-rw-   0        0        0      224 2022-07-08 09:33:08.000000 sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_feature.py
--rw-rw-rw-   0        0        0      248 2022-07-08 09:33:11.000000 sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_types.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/features/silaservice/
--rw-rw-rw-   0        0        0     7896 2022-07-08 09:33:12.000000 sila2-0.9.1/src/sila2/features/silaservice/SiLAService.sila.xml
--rw-rw-rw-   0        0        0      551 2022-07-08 09:33:14.000000 sila2-0.9.1/src/sila2/features/silaservice/__init__.py
--rw-rw-rw-   0        0        0     5799 2022-07-08 09:33:14.000000 sila2-0.9.1/src/sila2/features/silaservice/silaservice_base.py
--rw-rw-rw-   0        0        0     3597 2022-07-08 09:33:14.000000 sila2-0.9.1/src/sila2/features/silaservice/silaservice_client.py
--rw-rw-rw-   0        0        0      635 2022-07-08 09:33:14.000000 sila2-0.9.1/src/sila2/features/silaservice/silaservice_errors.py
--rw-rw-rw-   0        0        0      218 2022-07-08 09:33:12.000000 sila2-0.9.1/src/sila2/features/silaservice/silaservice_feature.py
--rw-rw-rw-   0        0        0      383 2022-07-08 09:33:14.000000 sila2-0.9.1/src/sila2/features/silaservice/silaservice_types.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/framework/
--rw-rw-rw-   0        0        0     3688 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/framework/abc/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/__init__.py
--rw-rw-rw-   0        0        0     1036 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/binary_transfer_handler.py
--rw-rw-rw-   0        0        0     5819 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/composite_message_mappable.py
--rw-rw-rw-   0        0        0     4334 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/constraint.py
--rw-rw-rw-   0        0        0     3531 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/data_type.py
--rw-rw-rw-   0        0        0     1143 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/message_mappable.py
--rw-rw-rw-   0        0        0      768 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/named_data_node.py
--rw-rw-rw-   0        0        0      611 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/named_node.py
--rw-rw-rw-   0        0        0     3416 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/abc/sila_error.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/__init__.py
--rw-rw-rw-   0        0        0      288 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/binary_download_failed.py
--rw-rw-rw-   0        0        0     2776 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/binary_transfer_error.py
--rw-rw-rw-   0        0        0      284 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/binary_upload_failed.py
--rw-rw-rw-   0        0        0     4821 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/client_binary_transfer_handler.py
--rw-rw-rw-   0        0        0     4877 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/download_servicer.py
--rw-rw-rw-   0        0        0      299 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/invalid_binary_transfer_uuid.py
--rw-rw-rw-   0        0        0     2060 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/server_binary_transfer_handler.py
--rw-rw-rw-   0        0        0     5769 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/binary_transfer/upload_servicer.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/framework/command/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/__init__.py
--rw-rw-rw-   0        0        0     2462 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/command.py
--rw-rw-rw-   0        0        0     2002 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/command_confirmation.py
--rw-rw-rw-   0        0        0     1031 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/command_execution_uuid.py
--rw-rw-rw-   0        0        0     1057 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/duration.py
--rw-rw-rw-   0        0        0     3399 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/execution_info.py
--rw-rw-rw-   0        0        0     1095 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/intermediate_response.py
--rw-rw-rw-   0        0        0     1338 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/observable_command.py
--rw-rw-rw-   0        0        0     1005 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/parameter.py
--rw-rw-rw-   0        0        0      997 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/response.py
--rw-rw-rw-   0        0        0      353 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/command/unobservable_command.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/framework/constraints/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/__init__.py
--rw-rw-rw-   0        0        0     1221 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/allowed_types.py
--rw-rw-rw-   0        0        0     3568 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/comparison_constraint.py
--rw-rw-rw-   0        0        0     1945 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/content_type.py
--rw-rw-rw-   0        0        0      772 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/element_count.py
--rw-rw-rw-   0        0        0      907 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/fully_qualified_identifier.py
--rw-rw-rw-   0        0        0      962 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/length.py
--rw-rw-rw-   0        0        0      780 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/maximal_element_count.py
--rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/maximal_exclusive.py
--rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/maximal_inclusive.py
--rw-rw-rw-   0        0        0      965 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/maximal_length.py
--rw-rw-rw-   0        0        0      780 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/minimal_element_count.py
--rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/minimal_exclusive.py
--rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/minimal_inclusive.py
--rw-rw-rw-   0        0        0     1021 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/minimal_length.py
--rw-rw-rw-   0        0        0      745 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/pattern.py
--rw-rw-rw-   0        0        0     4877 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/schema.py
--rw-rw-rw-   0        0        0     2579 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/set.py
--rw-rw-rw-   0        0        0     2462 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/constraints/unit.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/framework/data_types/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/__init__.py
--rw-rw-rw-   0        0        0     3830 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/any.py
--rw-rw-rw-   0        0        0     2741 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/binary.py
--rw-rw-rw-   0        0        0      898 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/boolean.py
--rw-rw-rw-   0        0        0     2145 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/constrained.py
--rw-rw-rw-   0        0        0     1595 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/data_type_definition.py
--rw-rw-rw-   0        0        0     1875 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/date.py
--rw-rw-rw-   0        0        0     1087 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/integer.py
--rw-rw-rw-   0        0        0     1506 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/list.py
--rw-rw-rw-   0        0        0     1345 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/real.py
--rw-rw-rw-   0        0        0     1125 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/string.py
--rw-rw-rw-   0        0        0     1075 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/structure.py
--rw-rw-rw-   0        0        0     1933 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/time.py
--rw-rw-rw-   0        0        0     2526 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/timestamp.py
--rw-rw-rw-   0        0        0     1990 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/data_types/timezone.py
--rw-rw-rw-   0        0        0      870 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/defined_execution_error_node.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/framework/errors/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/__init__.py
--rw-rw-rw-   0        0        0      437 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/command_execution_not_accepted.py
--rw-rw-rw-   0        0        0      522 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/command_execution_not_finished.py
--rw-rw-rw-   0        0        0     2708 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/defined_execution_error.py
--rw-rw-rw-   0        0        0     2934 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/framework_error.py
--rw-rw-rw-   0        0        0      580 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/invalid_command_execution_uuid.py
--rw-rw-rw-   0        0        0      478 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/invalid_metadata.py
--rw-rw-rw-   0        0        0      459 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/no_metadata_allowed.py
--rw-rw-rw-   0        0        0     1023 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/sila_connection_error.py
--rw-rw-rw-   0        0        0     1566 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/undefined_execution_error.py
--rw-rw-rw-   0        0        0     2092 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/errors/validation_error.py
--rw-rw-rw-   0        0        0     8630 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/feature.py
--rw-rw-rw-   0        0        0     3144 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/fully_qualified_identifier.py
--rw-rw-rw-   0        0        0     4083 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/metadata.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/framework/pb2/
--rw-rw-rw-   0        0        0    10023 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/pb2/SiLABinaryTransfer_pb2.py
--rw-rw-rw-   0        0        0    12191 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/pb2/SiLABinaryTransfer_pb2_grpc.py
--rw-rw-rw-   0        0        0    13454 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/pb2/SiLAFramework_pb2.py
--rw-rw-rw-   0        0        0      148 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/pb2/SiLAFramework_pb2_grpc.py
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/pb2/__init__.py
--rw-rw-rw-   0        0        0      528 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/pb2/custom_protocols.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/framework/property/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/property/__init__.py
--rw-rw-rw-   0        0        0      715 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/property/observable_property.py
--rw-rw-rw-   0        0        0     2855 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/property/property.py
--rw-rw-rw-   0        0        0      717 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/framework/property/unobservable_property.py
--rw-rw-rw-   0        0        0     8466 2022-07-25 13:53:08.000000 sila2-0.9.1/src/sila2/framework/utils.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/__init__.py
--rw-rw-rw-   0        0        0     5854 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/base.jinja2
--rw-rw-rw-   0        0        0     3531 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/client.jinja2
--rw-rw-rw-   0        0        0      641 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/errors.jinja2
--rw-rw-rw-   0        0        0      183 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/feature.jinja2
--rw-rw-rw-   0        0        0     2681 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/impl.jinja2
--rw-rw-rw-   0        0        0     1681 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/init.jinja2
--rw-rw-rw-   0        0        0      930 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/types.jinja2
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/__init__.py
--rw-rw-rw-   0        0        0     1452 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/client.jinja2
--rw-rw-rw-   0        0        0       27 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/gitignore.jinja2
--rw-rw-rw-   0        0        0      107 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/init.jinja2
--rw-rw-rw-   0        0        0     4273 2022-07-28 08:27:41.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/main.jinja2
--rw-rw-rw-   0        0        0      444 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/pyproject_toml.jinja2
--rw-rw-rw-   0        0        0      209 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/readme.jinja2
--rw-rw-rw-   0        0        0     2330 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/server.jinja2
--rw-rw-rw-   0        0        0      161 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/resources/code_generator_templates/package/setup_py.jinja2
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/proto/
--rw-rw-rw-   0        0        0     2016 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/proto/SiLABinaryTransfer.proto
--rw-rw-rw-   0        0        0     2628 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/proto/SiLAFramework.proto
--rw-rw-rw-   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/proto/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/xsd/
--rw-rw-rw-   0        0        0      409 2022-07-08 09:18:26.000000 sila2-0.9.1/src/sila2/resources/xsd/AnyTypeDataType.xsd
--rw-rw-rw-   0        0        0     8924 2022-07-08 09:18:26.000000 sila2-0.9.1/src/sila2/resources/xsd/Constraints.xsd
--rw-rw-rw-   0        0        0     2536 2022-07-08 09:18:26.000000 sila2-0.9.1/src/sila2/resources/xsd/DataTypes.xsd
--rw-rw-rw-   0        0        0     6034 2022-07-08 09:18:26.000000 sila2-0.9.1/src/sila2/resources/xsd/FeatureDefinition.xsd
--rw-rw-rw-   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/xsd/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/resources/xsl/
--rw-rw-rw-   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/xsl/__init__.py
--rw-rw-rw-   0        0        0    27669 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/xsl/fdl-validation.xsl
--rw-rw-rw-   0        0        0    12395 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/xsl/fdl2proto-messages.xsl
--rw-rw-rw-   0        0        0     5767 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/xsl/fdl2proto-service.xsl
--rw-rw-rw-   0        0        0     4727 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2/resources/xsl/fdl2proto.xsl
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/server/
--rw-rw-rw-   0        0        0      622 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/server/default_feature_implementations/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/default_feature_implementations/__init__.py
--rw-rw-rw-   0        0        0     2493 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/default_feature_implementations/authenticationservice_impl.py
--rw-rw-rw-   0        0        0     1669 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/default_feature_implementations/authorizationproviderservice_impl.py
--rw-rw-rw-   0        0        0     2237 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/default_feature_implementations/authorizationservice_impl.py
--rw-rw-rw-   0        0        0     2904 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/default_feature_implementations/lockcontroller_impl.py
--rw-rw-rw-   0        0        0     3192 2022-07-25 13:23:29.000000 sila2-0.9.1/src/sila2/server/encryption.py
--rw-rw-rw-   0        0        0     2904 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/feature_implementation_base.py
--rw-rw-rw-   0        0        0    20992 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/feature_implementation_servicer.py
--rw-rw-rw-   0        0        0     1417 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/metadata_dict.py
--rw-rw-rw-   0        0        0     1499 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/metadata_interceptor.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:15.000000 sila2-0.9.1/src/sila2/server/observables/
--rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/observables/__init__.py
--rw-rw-rw-   0        0        0     3902 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/observables/observable_command_instance.py
--rw-rw-rw-   0        0        0     4992 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/observables/observable_command_manager.py
--rw-rw-rw-   0        0        0     1230 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/observables/stream.py
--rw-rw-rw-   0        0        0     2445 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/observables/subscription_manager_thread.py
--rw-rw-rw-   0        0        0    17215 2022-07-27 14:56:23.000000 sila2-0.9.1/src/sila2/server/sila_server.py
--rw-rw-rw-   0        0        0     1887 2022-07-08 09:18:19.000000 sila2-0.9.1/src/sila2/server/silaservice_impl.py
-drwxrwxrwx   0        0        0        0 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/
--rw-rw-rw-   0        0        0     8618 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10893 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      486 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-07-28 08:30:14.000000 sila2-0.9.1/src/sila2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/
+-rw-rw-rw-   0        0        0     1092 2022-07-08 09:18:19.000000 sila2-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0     8618 2022-08-01 21:23:29.000000 sila2-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6245 2022-07-08 09:18:19.000000 sila2-0.9.2/README.md
+-rw-rw-rw-   0        0        0     3439 2022-08-01 21:15:20.000000 sila2-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-08-01 21:23:29.000000 sila2-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     1486 2022-07-08 09:18:19.000000 sila2-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/
+-rw-rw-rw-   0        0        0      692 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/client/
+-rw-rw-rw-   0        0        0     1093 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/__init__.py
+-rw-rw-rw-   0        0        0     2831 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_feature.py
+-rw-rw-rw-   0        0        0     2466 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_metadata.py
+-rw-rw-rw-   0        0        0     2733 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_observable_command.py
+-rw-rw-rw-   0        0        0     8694 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_observable_command_instance.py
+-rw-rw-rw-   0        0        0     2471 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_observable_property.py
+-rw-rw-rw-   0        0        0     1958 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_unobservable_command.py
+-rw-rw-rw-   0        0        0     2695 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/client_unobservable_property.py
+-rw-rw-rw-   0        0        0     1739 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/execution_info_subscription_thread.py
+-rw-rw-rw-   0        0        0     1588 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/grpc_stream_subscription.py
+-rw-rw-rw-   0        0        0     1689 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/polling_subscription.py
+-rw-rw-rw-   0        0        0     9391 2022-07-28 08:40:31.000000 sila2-0.9.2/src/sila2/client/sila_client.py
+-rw-rw-rw-   0        0        0     2115 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/client/subscription.py
+-rw-rw-rw-   0        0        0     3876 2022-07-25 13:53:28.000000 sila2-0.9.2/src/sila2/client/utils.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/code_generator/
+-rw-rw-rw-   0        0        0      310 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/__init__.py
+-rw-rw-rw-   0        0        0     8548 2022-08-01 20:20:54.000000 sila2-0.9.2/src/sila2/code_generator/__main__.py
+-rw-rw-rw-   0        0        0     7778 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/code_generator.py
+-rw-rw-rw-   0        0        0     2271 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/code_generator_base.py
+-rw-rw-rw-   0        0        0    10445 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/feature_generator.py
+-rw-rw-rw-   0        0        0      389 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_environment.py
+-rw-rw-rw-   0        0        0      429 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_loader.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/code_generator/template_objects/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_objects/__init__.py
+-rw-rw-rw-   0        0        0     1236 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_objects/base.py
+-rw-rw-rw-   0        0        0     3112 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_objects/basics.py
+-rw-rw-rw-   0        0        0     1322 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_objects/client.py
+-rw-rw-rw-   0        0        0     1194 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/code_generator/template_objects/types.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/discovery/
+-rw-rw-rw-   0        0        0       96 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/discovery/__init__.py
+-rw-rw-rw-   0        0        0      754 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/discovery/broadcaster.py
+-rw-rw-rw-   0        0        0     3502 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/discovery/browser.py
+-rw-rw-rw-   0        0        0     5113 2022-07-25 12:20:26.000000 sila2-0.9.2/src/sila2/discovery/listener.py
+-rw-rw-rw-   0        0        0     1267 2022-07-25 13:48:58.000000 sila2-0.9.2/src/sila2/discovery/service_info.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/features/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/features/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/features/authenticationservice/
+-rw-rw-rw-   0        0        0     5274 2022-07-08 09:33:03.000000 sila2-0.9.2/src/sila2/features/authenticationservice/AuthenticationService.sila.xml
+-rw-rw-rw-   0        0        0      664 2022-08-01 21:18:19.000000 sila2-0.9.2/src/sila2/features/authenticationservice/__init__.py
+-rw-rw-rw-   0        0        0     1887 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_base.py
+-rw-rw-rw-   0        0        0     1693 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_client.py
+-rw-rw-rw-   0        0        0      937 2022-08-01 21:18:19.000000 sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_errors.py
+-rw-rw-rw-   0        0        0      238 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_feature.py
+-rw-rw-rw-   0        0        0      552 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_types.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/
+-rw-rw-rw-   0        0        0     3614 2022-07-08 09:33:04.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/AuthorizationProviderService.sila.xml
+-rw-rw-rw-   0        0        0      698 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/__init__.py
+-rw-rw-rw-   0        0        0     1151 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_base.py
+-rw-rw-rw-   0        0        0     1023 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_client.py
+-rw-rw-rw-   0        0        0     1040 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_errors.py
+-rw-rw-rw-   0        0        0      252 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_feature.py
+-rw-rw-rw-   0        0        0      331 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_types.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/features/authorizationservice/
+-rw-rw-rw-   0        0        0     1319 2022-07-08 09:33:06.000000 sila2-0.9.2/src/sila2/features/authorizationservice/AuthorizationService.sila.xml
+-rw-rw-rw-   0        0        0      478 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationservice/__init__.py
+-rw-rw-rw-   0        0        0      992 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_base.py
+-rw-rw-rw-   0        0        0      824 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_client.py
+-rw-rw-rw-   0        0        0      606 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_errors.py
+-rw-rw-rw-   0        0        0      236 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_feature.py
+-rw-rw-rw-   0        0        0       99 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_types.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/features/lockcontroller/
+-rw-rw-rw-   0        0        0     5480 2022-07-08 09:33:08.000000 sila2-0.9.2/src/sila2/features/lockcontroller/LockController.sila.xml
+-rw-rw-rw-   0        0        0      654 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/lockcontroller/__init__.py
+-rw-rw-rw-   0        0        0     3286 2022-08-01 21:18:19.000000 sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_base.py
+-rw-rw-rw-   0        0        0     2793 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_client.py
+-rw-rw-rw-   0        0        0     1273 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_errors.py
+-rw-rw-rw-   0        0        0      224 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_feature.py
+-rw-rw-rw-   0        0        0      248 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_types.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/features/silaservice/
+-rw-rw-rw-   0        0        0     7896 2022-07-08 09:33:12.000000 sila2-0.9.2/src/sila2/features/silaservice/SiLAService.sila.xml
+-rw-rw-rw-   0        0        0      551 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/silaservice/__init__.py
+-rw-rw-rw-   0        0        0     5799 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/silaservice/silaservice_base.py
+-rw-rw-rw-   0        0        0     3597 2022-08-01 21:18:19.000000 sila2-0.9.2/src/sila2/features/silaservice/silaservice_client.py
+-rw-rw-rw-   0        0        0      635 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/silaservice/silaservice_errors.py
+-rw-rw-rw-   0        0        0      218 2022-08-01 21:18:18.000000 sila2-0.9.2/src/sila2/features/silaservice/silaservice_feature.py
+-rw-rw-rw-   0        0        0      383 2022-08-01 21:18:17.000000 sila2-0.9.2/src/sila2/features/silaservice/silaservice_types.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/
+-rw-rw-rw-   0        0        0     3688 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/abc/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/__init__.py
+-rw-rw-rw-   0        0        0     1036 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/binary_transfer_handler.py
+-rw-rw-rw-   0        0        0     5819 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/composite_message_mappable.py
+-rw-rw-rw-   0        0        0     4334 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/constraint.py
+-rw-rw-rw-   0        0        0     3531 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/data_type.py
+-rw-rw-rw-   0        0        0     1143 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/message_mappable.py
+-rw-rw-rw-   0        0        0      768 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/named_data_node.py
+-rw-rw-rw-   0        0        0      611 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/named_node.py
+-rw-rw-rw-   0        0        0     3416 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/abc/sila_error.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/__init__.py
+-rw-rw-rw-   0        0        0      288 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/binary_download_failed.py
+-rw-rw-rw-   0        0        0     2776 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/binary_transfer_error.py
+-rw-rw-rw-   0        0        0      284 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/binary_upload_failed.py
+-rw-rw-rw-   0        0        0     4821 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/client_binary_transfer_handler.py
+-rw-rw-rw-   0        0        0     4877 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/download_servicer.py
+-rw-rw-rw-   0        0        0      299 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/invalid_binary_transfer_uuid.py
+-rw-rw-rw-   0        0        0     2060 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/server_binary_transfer_handler.py
+-rw-rw-rw-   0        0        0     5769 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/binary_transfer/upload_servicer.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/command/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/__init__.py
+-rw-rw-rw-   0        0        0     2462 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/command.py
+-rw-rw-rw-   0        0        0     2002 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/command_confirmation.py
+-rw-rw-rw-   0        0        0     1031 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/command_execution_uuid.py
+-rw-rw-rw-   0        0        0     1057 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/duration.py
+-rw-rw-rw-   0        0        0     3399 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/execution_info.py
+-rw-rw-rw-   0        0        0     1095 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/intermediate_response.py
+-rw-rw-rw-   0        0        0     1338 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/observable_command.py
+-rw-rw-rw-   0        0        0     1005 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/parameter.py
+-rw-rw-rw-   0        0        0      997 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/response.py
+-rw-rw-rw-   0        0        0      353 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/command/unobservable_command.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/constraints/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/__init__.py
+-rw-rw-rw-   0        0        0     1221 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/allowed_types.py
+-rw-rw-rw-   0        0        0     3568 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/comparison_constraint.py
+-rw-rw-rw-   0        0        0     1945 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/content_type.py
+-rw-rw-rw-   0        0        0      772 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/element_count.py
+-rw-rw-rw-   0        0        0      907 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/fully_qualified_identifier.py
+-rw-rw-rw-   0        0        0      962 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/length.py
+-rw-rw-rw-   0        0        0      780 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/maximal_element_count.py
+-rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/maximal_exclusive.py
+-rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/maximal_inclusive.py
+-rw-rw-rw-   0        0        0      965 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/maximal_length.py
+-rw-rw-rw-   0        0        0      780 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/minimal_element_count.py
+-rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/minimal_exclusive.py
+-rw-rw-rw-   0        0        0     1011 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/minimal_inclusive.py
+-rw-rw-rw-   0        0        0     1021 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/minimal_length.py
+-rw-rw-rw-   0        0        0      745 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/pattern.py
+-rw-rw-rw-   0        0        0     4877 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/schema.py
+-rw-rw-rw-   0        0        0     2579 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/set.py
+-rw-rw-rw-   0        0        0     2462 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/constraints/unit.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/data_types/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/__init__.py
+-rw-rw-rw-   0        0        0     3830 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/any.py
+-rw-rw-rw-   0        0        0     2741 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/binary.py
+-rw-rw-rw-   0        0        0      898 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/boolean.py
+-rw-rw-rw-   0        0        0     2145 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/constrained.py
+-rw-rw-rw-   0        0        0     1595 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/data_type_definition.py
+-rw-rw-rw-   0        0        0     1875 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/date.py
+-rw-rw-rw-   0        0        0     1087 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/integer.py
+-rw-rw-rw-   0        0        0     1506 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/list.py
+-rw-rw-rw-   0        0        0     1345 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/real.py
+-rw-rw-rw-   0        0        0     1125 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/string.py
+-rw-rw-rw-   0        0        0     1075 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/structure.py
+-rw-rw-rw-   0        0        0     1933 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/time.py
+-rw-rw-rw-   0        0        0     2526 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/timestamp.py
+-rw-rw-rw-   0        0        0     1990 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/data_types/timezone.py
+-rw-rw-rw-   0        0        0      870 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/defined_execution_error_node.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/framework/errors/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/__init__.py
+-rw-rw-rw-   0        0        0      437 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/command_execution_not_accepted.py
+-rw-rw-rw-   0        0        0      522 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/command_execution_not_finished.py
+-rw-rw-rw-   0        0        0     2708 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/defined_execution_error.py
+-rw-rw-rw-   0        0        0     2934 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/framework_error.py
+-rw-rw-rw-   0        0        0      580 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/invalid_command_execution_uuid.py
+-rw-rw-rw-   0        0        0      478 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/invalid_metadata.py
+-rw-rw-rw-   0        0        0      459 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/no_metadata_allowed.py
+-rw-rw-rw-   0        0        0     1023 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/sila_connection_error.py
+-rw-rw-rw-   0        0        0     1566 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/undefined_execution_error.py
+-rw-rw-rw-   0        0        0     2092 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/errors/validation_error.py
+-rw-rw-rw-   0        0        0     8630 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/feature.py
+-rw-rw-rw-   0        0        0     3144 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/fully_qualified_identifier.py
+-rw-rw-rw-   0        0        0     4083 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/metadata.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/framework/pb2/
+-rw-rw-rw-   0        0        0    10023 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/pb2/SiLABinaryTransfer_pb2.py
+-rw-rw-rw-   0        0        0    12191 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/pb2/SiLABinaryTransfer_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13454 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/pb2/SiLAFramework_pb2.py
+-rw-rw-rw-   0        0        0      148 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/pb2/SiLAFramework_pb2_grpc.py
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/pb2/__init__.py
+-rw-rw-rw-   0        0        0      528 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/pb2/custom_protocols.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/framework/property/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/property/__init__.py
+-rw-rw-rw-   0        0        0      715 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/property/observable_property.py
+-rw-rw-rw-   0        0        0     2855 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/property/property.py
+-rw-rw-rw-   0        0        0      717 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/framework/property/unobservable_property.py
+-rw-rw-rw-   0        0        0     8828 2022-07-29 08:10:35.000000 sila2-0.9.2/src/sila2/framework/utils.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/__init__.py
+-rw-rw-rw-   0        0        0     5799 2022-08-01 19:56:59.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/base.jinja2
+-rw-rw-rw-   0        0        0     3531 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/client.jinja2
+-rw-rw-rw-   0        0        0      641 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/errors.jinja2
+-rw-rw-rw-   0        0        0      183 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/feature.jinja2
+-rw-rw-rw-   0        0        0     2767 2022-08-01 20:00:07.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/impl.jinja2
+-rw-rw-rw-   0        0        0     1681 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/init.jinja2
+-rw-rw-rw-   0        0        0      930 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/types.jinja2
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/__init__.py
+-rw-rw-rw-   0        0        0     1452 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/client.jinja2
+-rw-rw-rw-   0        0        0       27 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/gitignore.jinja2
+-rw-rw-rw-   0        0        0      107 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/init.jinja2
+-rw-rw-rw-   0        0        0     4398 2022-07-29 08:20:58.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/main.jinja2
+-rw-rw-rw-   0        0        0      444 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/pyproject_toml.jinja2
+-rw-rw-rw-   0        0        0      209 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/readme.jinja2
+-rw-rw-rw-   0        0        0     2330 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/server.jinja2
+-rw-rw-rw-   0        0        0      161 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/resources/code_generator_templates/package/setup_py.jinja2
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/proto/
+-rw-rw-rw-   0        0        0     2016 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/proto/SiLABinaryTransfer.proto
+-rw-rw-rw-   0        0        0     2628 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/proto/SiLAFramework.proto
+-rw-rw-rw-   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/proto/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/xsd/
+-rw-rw-rw-   0        0        0      409 2022-07-08 09:18:26.000000 sila2-0.9.2/src/sila2/resources/xsd/AnyTypeDataType.xsd
+-rw-rw-rw-   0        0        0     8924 2022-07-08 09:18:26.000000 sila2-0.9.2/src/sila2/resources/xsd/Constraints.xsd
+-rw-rw-rw-   0        0        0     2536 2022-07-08 09:18:26.000000 sila2-0.9.2/src/sila2/resources/xsd/DataTypes.xsd
+-rw-rw-rw-   0        0        0     6034 2022-07-08 09:18:26.000000 sila2-0.9.2/src/sila2/resources/xsd/FeatureDefinition.xsd
+-rw-rw-rw-   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/xsd/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/resources/xsl/
+-rw-rw-rw-   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/xsl/__init__.py
+-rw-rw-rw-   0        0        0    27669 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/xsl/fdl-validation.xsl
+-rw-rw-rw-   0        0        0    12395 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/xsl/fdl2proto-messages.xsl
+-rw-rw-rw-   0        0        0     5767 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/xsl/fdl2proto-service.xsl
+-rw-rw-rw-   0        0        0     4727 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2/resources/xsl/fdl2proto.xsl
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/server/
+-rw-rw-rw-   0        0        0      622 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/server/default_feature_implementations/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/default_feature_implementations/__init__.py
+-rw-rw-rw-   0        0        0     2493 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/default_feature_implementations/authenticationservice_impl.py
+-rw-rw-rw-   0        0        0     1669 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/default_feature_implementations/authorizationproviderservice_impl.py
+-rw-rw-rw-   0        0        0     2237 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/default_feature_implementations/authorizationservice_impl.py
+-rw-rw-rw-   0        0        0     2904 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/default_feature_implementations/lockcontroller_impl.py
+-rw-rw-rw-   0        0        0     3192 2022-07-25 13:23:29.000000 sila2-0.9.2/src/sila2/server/encryption.py
+-rw-rw-rw-   0        0        0     2904 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/feature_implementation_base.py
+-rw-rw-rw-   0        0        0    20992 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/feature_implementation_servicer.py
+-rw-rw-rw-   0        0        0     1417 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/metadata_dict.py
+-rw-rw-rw-   0        0        0     1499 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/metadata_interceptor.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:29.000000 sila2-0.9.2/src/sila2/server/observables/
+-rw-rw-rw-   0        0        0        0 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/observables/__init__.py
+-rw-rw-rw-   0        0        0     3902 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/observables/observable_command_instance.py
+-rw-rw-rw-   0        0        0     4992 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/observables/observable_command_manager.py
+-rw-rw-rw-   0        0        0     1230 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/observables/stream.py
+-rw-rw-rw-   0        0        0     2445 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/observables/subscription_manager_thread.py
+-rw-rw-rw-   0        0        0    17215 2022-07-27 14:56:23.000000 sila2-0.9.2/src/sila2/server/sila_server.py
+-rw-rw-rw-   0        0        0     1887 2022-07-08 09:18:19.000000 sila2-0.9.2/src/sila2/server/silaservice_impl.py
+drwxrwxrwx   0        0        0        0 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/
+-rw-rw-rw-   0        0        0     8618 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10893 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      512 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-08-01 21:23:28.000000 sila2-0.9.2/src/sila2.egg-info/top_level.txt
```

### Comparing `sila2-0.9.1/LICENSE` & `sila2-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/PKG-INFO` & `sila2-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sila2
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python implementation of the SiLA 2 standard for lab automation
 Author-email: Niklas Mertsch <niklas.mertsch@wega-it.com>
 License: MIT License
         
         Copyright (c) 2022 Niklas Mertsch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sila2-0.9.1/README.md` & `sila2-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/pyproject.toml` & `sila2-0.9.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sila2"
-version = "0.9.1"
+version = "0.9.2"
 description = "Python implementation of the SiLA 2 standard for lab automation"
 readme = "README.md"
 authors = [
     { name = "Niklas Mertsch", email = "niklas.mertsch@wega-it.com" },
 ]
 license = {file = "LICENSE"}
 classifiers = [
@@ -33,14 +33,16 @@
     "pytest-cov",
 ]
 dev = [
     "black",
     "isort",
     "pytest",
     "pytest-cov",
+    # flake8 does not support pyproject.toml config natively; pyproject-flake8 does not support flake8 >= 5.0.0
+    "flake8 < 5.0.0",
     "pyproject-flake8",
 ]
 docs = [
     "sphinx",
     "sphinxcontrib-napoleon",
     "sphinxcontrib-runcmd",
 ]
@@ -53,14 +55,16 @@
 jsonschema = ["jsonschema"]
 xmlschema = ["xmlschema"]
 full = [
     "black",
     "isort",
     "jinja2",
     "jsonschema",
+    # flake8 does not support pyproject.toml config natively; pyproject-flake8 does not support flake8 >= 5.0.0
+    "flake8 < 5.0.0",
     "pyproject-flake8",
     "pytest",
     "pytest-cov",
     "sphinx",
     "sphinxcontrib-napoleon",
     "sphinxcontrib-runcmd",
     "typer",
```

### Comparing `sila2-0.9.1/setup.py` & `sila2-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/__init__.py` & `sila2-0.9.2/src/sila2/__init__.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/__init__.py` & `sila2-0.9.2/src/sila2/client/__init__.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_feature.py` & `sila2-0.9.2/src/sila2/client/client_feature.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_metadata.py` & `sila2-0.9.2/src/sila2/client/client_metadata.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_observable_command.py` & `sila2-0.9.2/src/sila2/client/client_observable_command.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_observable_command_instance.py` & `sila2-0.9.2/src/sila2/client/client_observable_command_instance.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_observable_property.py` & `sila2-0.9.2/src/sila2/client/client_observable_property.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_unobservable_command.py` & `sila2-0.9.2/src/sila2/client/client_unobservable_command.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/client_unobservable_property.py` & `sila2-0.9.2/src/sila2/client/client_unobservable_property.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/execution_info_subscription_thread.py` & `sila2-0.9.2/src/sila2/client/execution_info_subscription_thread.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/grpc_stream_subscription.py` & `sila2-0.9.2/src/sila2/client/grpc_stream_subscription.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/polling_subscription.py` & `sila2-0.9.2/src/sila2/client/polling_subscription.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/sila_client.py` & `sila2-0.9.2/src/sila2/client/sila_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,17 @@
         --------
         Using unencrypted communication violates the SiLA specification and should only be used for testing purposes
         """
         self.__address = address
         self.__port = port
 
         target = f"{self.__address}:{self.__port}"
+
         expected_server_uuid: Optional[UUID] = None
-        if any(par is not None for par in (root_certs, private_key, cert_chain)):
+        if root_certs is not None or private_key is not None or cert_chain is not None:
             if insecure:
                 raise ValueError("Cannot use certificate information with insecure connections")
 
             credentials = grpc.ssl_channel_credentials(
                 root_certificates=root_certs, private_key=private_key, certificate_chain=cert_chain
             )
             cert = x509.load_pem_x509_certificate(
@@ -112,15 +113,16 @@
             except ExtensionNotFound:
                 warnings.warn("Server certificate is missing the extension 1.3.6.1.4.1.58583 to specify its UUID")
 
             self._channel = grpc.secure_channel(target, credentials=credentials)
         elif insecure:
             self._channel = grpc.insecure_channel(target)
         else:
-            raise ValueError("Either use an insecure connection, or provide certificate information")
+            # use default trust store
+            self._channel = grpc.secure_channel(target, credentials=grpc.ssl_channel_credentials())
 
         self._features = {}
         self._children_by_fully_qualified_identifier = {}
         self._registered_defined_execution_error_classes = {}
 
         # import locally to prevent circular import
         from sila2.features.silaservice import SiLAServiceFeature, UnimplementedFeature
```

### Comparing `sila2-0.9.1/src/sila2/client/subscription.py` & `sila2-0.9.2/src/sila2/client/subscription.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/client/utils.py` & `sila2-0.9.2/src/sila2/client/utils.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/__main__.py` & `sila2-0.9.2/src/sila2/code_generator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from contextlib import contextmanager
 from glob import glob
 from os.path import isdir, join
 from typing import Dict, List
 
 from typer import Argument, Option, Typer
 
-from sila2.framework import FullyQualifiedFeatureIdentifier
 from sila2.framework.utils import parse_feature_definition, xpath_sila
 
 main = Typer(help="SiLA 2 Python Code Generator")
 __DEBUG = False
 
 
 def _get_feature_definition_paths(feature_definition_paths: List[str]) -> List[str]:
@@ -148,43 +147,43 @@
     from sila2.code_generator.feature_generator import FeatureGenerator
     from sila2.framework.feature import Feature
 
     with print_exception_if_not_debug():
         generated_dir = find_matching_directory(join(package_directory, "*", "generated"))
         implementation_dir = find_matching_directory(join(package_directory, "*", "feature_implementations"))
 
-        features: Dict[FullyQualifiedFeatureIdentifier, Feature] = {}
         generator = CodeGenerator(overwrite=True)
 
         # give precedence to explicitly stated features
         def get_identifier(fdl_filepath: str) -> str:
             return xpath_sila(parse_feature_definition(fdl_filepath), "/sila:Feature/sila:Identifier/text()")[0]
 
         fdl_files_by_identifier: Dict[str, str] = {
             get_identifier(f): f for f in glob(join(generated_dir, "*", "*.sila.xml"))
         }
         fdl_files_by_identifier.update({get_identifier(f): f for f in feature_definitions})
-        print(fdl_files_by_identifier)
 
+        features: List[Feature] = []
         for fdl_file in fdl_files_by_identifier.values():
             feature = Feature(fdl_file)
+            features.append(feature)
             feature_generator = FeatureGenerator(feature, overwrite=True)
             feature_dir = join(generated_dir, feature._identifier.lower())
             with open(f"{feature_dir}/{feature._identifier.lower()}_base.py") as fp:
                 old_base = fp.read()
 
             feature_generator.generate_feature_files(feature_dir)
             with open(f"{feature_dir}/{feature._identifier.lower()}_base.py") as fp:
                 new_base = fp.read()
 
             # if base class changed: generate new impl
             if old_base != new_base:
                 feature_generator.generate_impl(implementation_dir, prefix="updated_")
             generator.generated_files.extend(feature_generator.generated_files)
-        generator._generate_client(features.values(), generated_dir)
+        generator._generate_client(features, generated_dir)
         generator.format_generated_files()
 
 
 @main.command()
 def generate_feature_files(
     output_directory: str = Option(".", "--output-directory", "-o", help="Output directory"),
     overwrite: bool = Option(default=False, help="Overwrite existing files"),
```

### Comparing `sila2-0.9.1/src/sila2/code_generator/code_generator.py` & `sila2-0.9.2/src/sila2/code_generator/code_generator.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/code_generator_base.py` & `sila2-0.9.2/src/sila2/code_generator/code_generator_base.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/feature_generator.py` & `sila2-0.9.2/src/sila2/code_generator/feature_generator.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/template_objects/base.py` & `sila2-0.9.2/src/sila2/code_generator/template_objects/base.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/template_objects/basics.py` & `sila2-0.9.2/src/sila2/code_generator/template_objects/basics.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/template_objects/client.py` & `sila2-0.9.2/src/sila2/code_generator/template_objects/client.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/code_generator/template_objects/types.py` & `sila2-0.9.2/src/sila2/code_generator/template_objects/types.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/discovery/broadcaster.py` & `sila2-0.9.2/src/sila2/discovery/broadcaster.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/discovery/browser.py` & `sila2-0.9.2/src/sila2/discovery/browser.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/discovery/listener.py` & `sila2-0.9.2/src/sila2/discovery/listener.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/discovery/service_info.py` & `sila2-0.9.2/src/sila2/discovery/service_info.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/features/authenticationservice/AuthenticationService.sila.xml` & `sila2-0.9.2/src/sila2/features/authenticationservice/AuthenticationService.sila.xml`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/features/authenticationservice/__init__.py` & `sila2-0.9.2/src/sila2/features/authenticationservice/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from .authenticationservice_base import AuthenticationServiceBase
 from .authenticationservice_client import AuthenticationServiceClient
 from .authenticationservice_errors import AuthenticationFailed, InvalidAccessToken
 from .authenticationservice_feature import AuthenticationServiceFeature
 from .authenticationservice_types import Login_Responses, Logout_Responses
 
 __all__ = [
```

### Comparing `sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_base.py` & `sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List
 
 from sila2.server import FeatureImplementationBase, MetadataDict
```

### Comparing `sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_client.py` & `sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 # -----
 # This class does not do anything useful at runtime. Its only purpose is to provide type annotations.
 # Since sphinx does not support .pyi files (yet?), so this is a .py file.
 # -----
 
 from __future__ import annotations
```

### Comparing `sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_errors.py` & `sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from typing import Optional
 
 from sila2.framework.errors.defined_execution_error import DefinedExecutionError
 
 from .authenticationservice_feature import AuthenticationServiceFeature
```

### Comparing `sila2-0.9.1/src/sila2/features/authenticationservice/authenticationservice_types.py` & `sila2-0.9.2/src/sila2/features/authenticationservice/authenticationservice_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from typing import NamedTuple
 
 
 class Login_Responses(NamedTuple):
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationproviderservice/AuthorizationProviderService.sila.xml` & `sila2-0.9.2/src/sila2/features/authorizationproviderservice/AuthorizationProviderService.sila.xml`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/features/authorizationproviderservice/__init__.py` & `sila2-0.9.2/src/sila2/features/authorizationproviderservice/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from .authorizationproviderservice_base import AuthorizationProviderServiceBase
 from .authorizationproviderservice_client import AuthorizationProviderServiceClient
 from .authorizationproviderservice_errors import AuthorizationFailed, InvalidAccessToken
 from .authorizationproviderservice_feature import AuthorizationProviderServiceFeature
 from .authorizationproviderservice_types import Verify_Responses
 
 __all__ = [
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_base.py` & `sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
 from sila2.server import FeatureImplementationBase, MetadataDict
 
 from .authorizationproviderservice_types import Verify_Responses
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_client.py` & `sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 # -----
 # This class does not do anything useful at runtime. Its only purpose is to provide type annotations.
 # Since sphinx does not support .pyi files (yet?), so this is a .py file.
 # -----
 
 from __future__ import annotations
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationproviderservice/authorizationproviderservice_errors.py` & `sila2-0.9.2/src/sila2/features/authorizationproviderservice/authorizationproviderservice_errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from typing import Optional
 
 from sila2.framework.errors.defined_execution_error import DefinedExecutionError
 
 from .authorizationproviderservice_feature import AuthorizationProviderServiceFeature
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationservice/AuthorizationService.sila.xml` & `sila2-0.9.2/src/sila2/features/authorizationservice/AuthorizationService.sila.xml`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_base.py` & `sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List, Union
 
 from sila2.framework import Command, Feature, FullyQualifiedIdentifier, Property
 from sila2.server import FeatureImplementationBase
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_client.py` & `sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 # -----
 # This class does not do anything useful at runtime. Its only purpose is to provide type annotations.
 # Since sphinx does not support .pyi files (yet?), so this is a .py file.
 # -----
 
 from __future__ import annotations
```

### Comparing `sila2-0.9.1/src/sila2/features/authorizationservice/authorizationservice_errors.py` & `sila2-0.9.2/src/sila2/features/authorizationservice/authorizationservice_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from typing import Optional
 
 from sila2.framework.errors.defined_execution_error import DefinedExecutionError
 
 from .authorizationservice_feature import AuthorizationServiceFeature
```

### Comparing `sila2-0.9.1/src/sila2/features/lockcontroller/LockController.sila.xml` & `sila2-0.9.2/src/sila2/features/lockcontroller/LockController.sila.xml`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/features/lockcontroller/__init__.py` & `sila2-0.9.2/src/sila2/features/lockcontroller/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from .lockcontroller_base import LockControllerBase
 from .lockcontroller_client import LockControllerClient
 from .lockcontroller_errors import InvalidLockIdentifier, ServerAlreadyLocked, ServerNotLocked
 from .lockcontroller_feature import LockControllerFeature
 from .lockcontroller_types import LockServer_Responses, UnlockServer_Responses
 
 __all__ = [
```

### Comparing `sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_base.py` & `sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List, Union
 
 from sila2.framework import Command, Feature, FullyQualifiedIdentifier, Property
 from sila2.server import FeatureImplementationBase, MetadataDict
```

### Comparing `sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_client.py` & `sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 # -----
 # This class does not do anything useful at runtime. Its only purpose is to provide type annotations.
 # Since sphinx does not support .pyi files (yet?), so this is a .py file.
 # -----
 
 from __future__ import annotations
```

### Comparing `sila2-0.9.1/src/sila2/features/lockcontroller/lockcontroller_errors.py` & `sila2-0.9.2/src/sila2/features/lockcontroller/lockcontroller_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from typing import Optional
 
 from sila2.framework.errors.defined_execution_error import DefinedExecutionError
 
 from .lockcontroller_feature import LockControllerFeature
```

### Comparing `sila2-0.9.1/src/sila2/features/silaservice/SiLAService.sila.xml` & `sila2-0.9.2/src/sila2/features/silaservice/SiLAService.sila.xml`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/features/silaservice/__init__.py` & `sila2-0.9.2/src/sila2/features/silaservice/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from .silaservice_base import SiLAServiceBase
 from .silaservice_client import SiLAServiceClient
 from .silaservice_errors import UnimplementedFeature
 from .silaservice_feature import SiLAServiceFeature
 from .silaservice_types import GetFeatureDefinition_Responses, SetServerName_Responses
 
 __all__ = [
```

### Comparing `sila2-0.9.1/src/sila2/features/silaservice/silaservice_base.py` & `sila2-0.9.2/src/sila2/features/silaservice/silaservice_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import List
 
 from sila2.server import FeatureImplementationBase, MetadataDict
```

### Comparing `sila2-0.9.1/src/sila2/features/silaservice/silaservice_client.py` & `sila2-0.9.2/src/sila2/features/silaservice/silaservice_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 # -----
 # This class does not do anything useful at runtime. Its only purpose is to provide type annotations.
 # Since sphinx does not support .pyi files (yet?), so this is a .py file.
 # -----
 
 from __future__ import annotations
```

### Comparing `sila2-0.9.1/src/sila2/features/silaservice/silaservice_errors.py` & `sila2-0.9.2/src/sila2/features/silaservice/silaservice_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by sila2.code_generator; sila2.__version__: 0.8.3
+# Generated by sila2.code_generator; sila2.__version__: 0.9.2
 from __future__ import annotations
 
 from typing import Optional
 
 from sila2.framework.errors.defined_execution_error import DefinedExecutionError
 
 from .silaservice_feature import SiLAServiceFeature
```

### Comparing `sila2-0.9.1/src/sila2/framework/__init__.py` & `sila2-0.9.2/src/sila2/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/binary_transfer_handler.py` & `sila2-0.9.2/src/sila2/framework/abc/binary_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/composite_message_mappable.py` & `sila2-0.9.2/src/sila2/framework/abc/composite_message_mappable.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/constraint.py` & `sila2-0.9.2/src/sila2/framework/abc/constraint.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/data_type.py` & `sila2-0.9.2/src/sila2/framework/abc/data_type.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/message_mappable.py` & `sila2-0.9.2/src/sila2/framework/abc/message_mappable.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/named_data_node.py` & `sila2-0.9.2/src/sila2/framework/abc/named_data_node.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/named_node.py` & `sila2-0.9.2/src/sila2/framework/abc/named_node.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/abc/sila_error.py` & `sila2-0.9.2/src/sila2/framework/abc/sila_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/binary_transfer/binary_transfer_error.py` & `sila2-0.9.2/src/sila2/framework/binary_transfer/binary_transfer_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/binary_transfer/client_binary_transfer_handler.py` & `sila2-0.9.2/src/sila2/framework/binary_transfer/client_binary_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/binary_transfer/download_servicer.py` & `sila2-0.9.2/src/sila2/framework/binary_transfer/download_servicer.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/binary_transfer/server_binary_transfer_handler.py` & `sila2-0.9.2/src/sila2/framework/binary_transfer/server_binary_transfer_handler.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/binary_transfer/upload_servicer.py` & `sila2-0.9.2/src/sila2/framework/binary_transfer/upload_servicer.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/command.py` & `sila2-0.9.2/src/sila2/framework/command/command.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/command_confirmation.py` & `sila2-0.9.2/src/sila2/framework/command/command_confirmation.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/command_execution_uuid.py` & `sila2-0.9.2/src/sila2/framework/command/command_execution_uuid.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/duration.py` & `sila2-0.9.2/src/sila2/framework/command/duration.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/execution_info.py` & `sila2-0.9.2/src/sila2/framework/command/execution_info.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/intermediate_response.py` & `sila2-0.9.2/src/sila2/framework/command/intermediate_response.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/observable_command.py` & `sila2-0.9.2/src/sila2/framework/command/observable_command.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/parameter.py` & `sila2-0.9.2/src/sila2/framework/command/parameter.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/command/response.py` & `sila2-0.9.2/src/sila2/framework/command/response.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/allowed_types.py` & `sila2-0.9.2/src/sila2/framework/constraints/allowed_types.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/comparison_constraint.py` & `sila2-0.9.2/src/sila2/framework/constraints/comparison_constraint.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/content_type.py` & `sila2-0.9.2/src/sila2/framework/constraints/content_type.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/element_count.py` & `sila2-0.9.2/src/sila2/framework/constraints/element_count.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/fully_qualified_identifier.py` & `sila2-0.9.2/src/sila2/framework/constraints/fully_qualified_identifier.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/length.py` & `sila2-0.9.2/src/sila2/framework/constraints/length.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/maximal_element_count.py` & `sila2-0.9.2/src/sila2/framework/constraints/maximal_element_count.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/maximal_exclusive.py` & `sila2-0.9.2/src/sila2/framework/constraints/maximal_exclusive.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/maximal_inclusive.py` & `sila2-0.9.2/src/sila2/framework/constraints/maximal_inclusive.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/maximal_length.py` & `sila2-0.9.2/src/sila2/framework/constraints/maximal_length.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/minimal_element_count.py` & `sila2-0.9.2/src/sila2/framework/constraints/minimal_element_count.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/minimal_exclusive.py` & `sila2-0.9.2/src/sila2/framework/constraints/minimal_exclusive.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/minimal_inclusive.py` & `sila2-0.9.2/src/sila2/framework/constraints/minimal_inclusive.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/minimal_length.py` & `sila2-0.9.2/src/sila2/framework/constraints/minimal_length.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/pattern.py` & `sila2-0.9.2/src/sila2/framework/constraints/pattern.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/schema.py` & `sila2-0.9.2/src/sila2/framework/constraints/schema.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/set.py` & `sila2-0.9.2/src/sila2/framework/constraints/set.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/constraints/unit.py` & `sila2-0.9.2/src/sila2/framework/constraints/unit.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/any.py` & `sila2-0.9.2/src/sila2/framework/data_types/any.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/binary.py` & `sila2-0.9.2/src/sila2/framework/data_types/binary.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/boolean.py` & `sila2-0.9.2/src/sila2/framework/data_types/boolean.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/constrained.py` & `sila2-0.9.2/src/sila2/framework/data_types/constrained.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/data_type_definition.py` & `sila2-0.9.2/src/sila2/framework/data_types/data_type_definition.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/date.py` & `sila2-0.9.2/src/sila2/framework/data_types/date.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/integer.py` & `sila2-0.9.2/src/sila2/framework/data_types/integer.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/list.py` & `sila2-0.9.2/src/sila2/framework/data_types/list.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/real.py` & `sila2-0.9.2/src/sila2/framework/data_types/real.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/string.py` & `sila2-0.9.2/src/sila2/framework/data_types/string.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/structure.py` & `sila2-0.9.2/src/sila2/framework/data_types/structure.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/time.py` & `sila2-0.9.2/src/sila2/framework/data_types/time.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/timestamp.py` & `sila2-0.9.2/src/sila2/framework/data_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/data_types/timezone.py` & `sila2-0.9.2/src/sila2/framework/data_types/timezone.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/defined_execution_error_node.py` & `sila2-0.9.2/src/sila2/framework/defined_execution_error_node.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/command_execution_not_finished.py` & `sila2-0.9.2/src/sila2/framework/errors/command_execution_not_finished.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/defined_execution_error.py` & `sila2-0.9.2/src/sila2/framework/errors/defined_execution_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/framework_error.py` & `sila2-0.9.2/src/sila2/framework/errors/framework_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/invalid_command_execution_uuid.py` & `sila2-0.9.2/src/sila2/framework/errors/invalid_command_execution_uuid.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/sila_connection_error.py` & `sila2-0.9.2/src/sila2/framework/errors/sila_connection_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/undefined_execution_error.py` & `sila2-0.9.2/src/sila2/framework/errors/undefined_execution_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/errors/validation_error.py` & `sila2-0.9.2/src/sila2/framework/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/feature.py` & `sila2-0.9.2/src/sila2/framework/feature.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/fully_qualified_identifier.py` & `sila2-0.9.2/src/sila2/framework/fully_qualified_identifier.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/metadata.py` & `sila2-0.9.2/src/sila2/framework/metadata.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/pb2/SiLABinaryTransfer_pb2.py` & `sila2-0.9.2/src/sila2/framework/pb2/SiLABinaryTransfer_pb2.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/pb2/SiLABinaryTransfer_pb2_grpc.py` & `sila2-0.9.2/src/sila2/framework/pb2/SiLABinaryTransfer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/pb2/SiLAFramework_pb2.py` & `sila2-0.9.2/src/sila2/framework/pb2/SiLAFramework_pb2.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/pb2/custom_protocols.py` & `sila2-0.9.2/src/sila2/framework/pb2/custom_protocols.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/property/observable_property.py` & `sila2-0.9.2/src/sila2/framework/property/observable_property.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/property/property.py` & `sila2-0.9.2/src/sila2/framework/property/property.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/property/unobservable_property.py` & `sila2-0.9.2/src/sila2/framework/property/unobservable_property.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/framework/utils.py` & `sila2-0.9.2/src/sila2/framework/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,7 +210,22 @@
         return [ipaddress.ip_address(host).exploded]
     except ValueError:
         try:
             # host is a valid hostname
             return [socket.gethostbyname(host)]
         except socket.gaierror as e:
             raise ValueError(f"Failed to resolve host '{host}': {e.strerror}")
+
+
+def running_in_docker() -> bool:
+    if os.path.exists("/.dockerenv"):
+        return True
+
+    cgroup_file = "/proc/self/cgroup"
+    if not os.path.isfile(cgroup_file):
+        return False
+
+    with open(cgroup_file) as cgroup_fp:
+        for line in cgroup_fp:
+            if ":/docker/" in line:
+                return True
+    return False
```

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/base.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/base.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 from .{{ feature._identifier|lower }}_types import {{ i }}
 {% endfor %}
 
 {% for import_ in imports %}
 from {{ import_.origin }} import {{ import_.target }}
 {% endfor %}
 
+from typing import TYPE_CHECKING
 {% if metadata %}
 from typing import List, Union
 from sila2.framework import Feature, Command, Property, FullyQualifiedIdentifier
 {% endif %}
 {% if observable_properties %}
-from typing import Optional, TYPE_CHECKING
+from typing import Optional
 from queue import Queue
 {% endif %}
 {% for cmd in unobservable_commands %}
 from .{{ feature._identifier|lower }}_types import {{ cmd.name }}_Responses
 {% endfor %}
 {% for cmd in observable_commands %}
 from .{{ feature._identifier|lower }}_types import {{ cmd.name }}_Responses
@@ -34,36 +35,33 @@
 from .{{ feature._identifier|lower }}_types import {{ cmd.name }}_IntermediateResponses
 from sila2.server import ObservableCommandInstanceWithIntermediateResponses
     {% else %}
 from sila2.server import ObservableCommandInstance
     {% endif %}
 {% endfor %}
 
-
-{% if observable_properties %}
 if TYPE_CHECKING:
-    from sila2.server import SilaServer
-{% endif %}
+    from ...server import Server
 
 class {{ feature._identifier }}Base(FeatureImplementationBase, ABC):
+    parent_server: Server
+
 {% for prop in observable_properties %}
     _{{ prop.name }}_producer_queue: Queue[{{ prop.type.representation }}]
 {% endfor %}
 
-{% if observable_properties %}
-    def __init__(self, parent_server: SilaServer):
+    def __init__(self, parent_server: Server):
         """
         {{ feature._description }}
         """
         super().__init__(parent_server=parent_server)
 
     {% for prop in observable_properties %}
         self._{{ prop.name }}_producer_queue = Queue()
     {% endfor %}
-{% endif %}
 
 {% for prop in unobservable_properties %}
     @abstractmethod
     def get_{{ prop.name }}(self, *, metadata: MetadataDict) -> {{ prop.type.representation }}:
         """
         {{ prop.docstring }}
```

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/client.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/client.jinja2`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/errors.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/errors.jinja2`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/impl.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/impl.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -28,18 +28,24 @@
     {% else %}
 from sila2.server import ObservableCommandInstance
     {% endif %}
 {% endfor %}
 
 from ..generated.{{ feature._identifier|lower }} import {{ feature._identifier }}Base
 
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ..server import Server
+
+
 class {{ feature._identifier }}Impl({{ feature._identifier }}Base):
-{% if not unobservable_properties and not observable_commands and not unobservable_commands %}
-    pass
-{% endif %}
+    def __init__(self, parent_server: Server) -> None:
+        super().__init__(parent_server=parent_server)
+
 {% for prop in unobservable_properties %}
     def get_{{ prop.name }}(self, *, metadata: MetadataDict) -> {{ prop.type.representation }}:
         raise NotImplementedError  # TODO
 {% endfor %}
 
 {% for cmd in unobservable_commands %}
     def {{ cmd.name }}(
```

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/init.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/init.jinja2`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/feature/types.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/feature/types.jinja2`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/package/client.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/package/client.jinja2`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/package/main.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/package/main.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import logging
 import signal
 from typing import Optional
 from uuid import UUID
 
 import typer
 from typer import BadParameter, Option
+from sila2.framework.utils import running_in_docker
 
 from .server import Server
 
 logger = logging.getLogger(__name__)
 
 
 def main(
-    ip_address: str = Option("127.0.0.1", "-a", "--ip-address", help="The IP address"),
+    ip_address: str = Option(
+        "0.0.0.0" if running_in_docker() else "127.0.0.1",
+        "-a", "--ip-address",
+        help="The IP address"
+    ),
     port: int = Option(50052, "-p", "--port", help="The port"),
     server_uuid: Optional[str] = Option(
         None, "--server-uuid", help="The server UUID [default: generate]", show_default=False
     ),
     disable_discovery: bool = Option(False, "--disable-discovery", help="Enable SiLA Server Discovery"),
     insecure: bool = Option(False, "--insecure", help="Start without encryption"),
     private_key_file: Optional[str] = Option(
```

### Comparing `sila2-0.9.1/src/sila2/resources/code_generator_templates/package/server.jinja2` & `sila2-0.9.2/src/sila2/resources/code_generator_templates/package/server.jinja2`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/proto/SiLABinaryTransfer.proto` & `sila2-0.9.2/src/sila2/resources/proto/SiLABinaryTransfer.proto`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/proto/SiLAFramework.proto` & `sila2-0.9.2/src/sila2/resources/proto/SiLAFramework.proto`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsd/Constraints.xsd` & `sila2-0.9.2/src/sila2/resources/xsd/Constraints.xsd`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsd/DataTypes.xsd` & `sila2-0.9.2/src/sila2/resources/xsd/DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsd/FeatureDefinition.xsd` & `sila2-0.9.2/src/sila2/resources/xsd/FeatureDefinition.xsd`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsl/fdl-validation.xsl` & `sila2-0.9.2/src/sila2/resources/xsl/fdl-validation.xsl`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsl/fdl2proto-messages.xsl` & `sila2-0.9.2/src/sila2/resources/xsl/fdl2proto-messages.xsl`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsl/fdl2proto-service.xsl` & `sila2-0.9.2/src/sila2/resources/xsl/fdl2proto-service.xsl`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/resources/xsl/fdl2proto.xsl` & `sila2-0.9.2/src/sila2/resources/xsl/fdl2proto.xsl`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/__init__.py` & `sila2-0.9.2/src/sila2/server/__init__.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/default_feature_implementations/authenticationservice_impl.py` & `sila2-0.9.2/src/sila2/server/default_feature_implementations/authenticationservice_impl.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/default_feature_implementations/authorizationproviderservice_impl.py` & `sila2-0.9.2/src/sila2/server/default_feature_implementations/authorizationproviderservice_impl.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/default_feature_implementations/authorizationservice_impl.py` & `sila2-0.9.2/src/sila2/server/default_feature_implementations/authorizationservice_impl.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/default_feature_implementations/lockcontroller_impl.py` & `sila2-0.9.2/src/sila2/server/default_feature_implementations/lockcontroller_impl.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/encryption.py` & `sila2-0.9.2/src/sila2/server/encryption.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/feature_implementation_base.py` & `sila2-0.9.2/src/sila2/server/feature_implementation_base.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/feature_implementation_servicer.py` & `sila2-0.9.2/src/sila2/server/feature_implementation_servicer.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/metadata_dict.py` & `sila2-0.9.2/src/sila2/server/metadata_dict.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/metadata_interceptor.py` & `sila2-0.9.2/src/sila2/server/metadata_interceptor.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/observables/observable_command_instance.py` & `sila2-0.9.2/src/sila2/server/observables/observable_command_instance.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/observables/observable_command_manager.py` & `sila2-0.9.2/src/sila2/server/observables/observable_command_manager.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/observables/stream.py` & `sila2-0.9.2/src/sila2/server/observables/stream.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/observables/subscription_manager_thread.py` & `sila2-0.9.2/src/sila2/server/observables/subscription_manager_thread.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/sila_server.py` & `sila2-0.9.2/src/sila2/server/sila_server.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2/server/silaservice_impl.py` & `sila2-0.9.2/src/sila2/server/silaservice_impl.py`

 * *Files identical despite different names*

### Comparing `sila2-0.9.1/src/sila2.egg-info/PKG-INFO` & `sila2-0.9.2/src/sila2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sila2
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python implementation of the SiLA 2 standard for lab automation
 Author-email: Niklas Mertsch <niklas.mertsch@wega-it.com>
 License: MIT License
         
         Copyright (c) 2022 Niklas Mertsch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sila2-0.9.1/src/sila2.egg-info/SOURCES.txt` & `sila2-0.9.2/src/sila2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

