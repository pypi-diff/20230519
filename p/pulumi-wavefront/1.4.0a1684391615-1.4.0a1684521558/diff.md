# Comparing `tmp/pulumi_wavefront-1.4.0a1684391615.tar.gz` & `tmp/pulumi_wavefront-1.4.0a1684521558.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_wavefront-1.4.0a1684391615.tar", last modified: Thu May 18 06:41:55 2023, max compression
+gzip compressed data, was "pulumi_wavefront-1.4.0a1684521558.tar", last modified: Fri May 19 18:43:57 2023, max compression
```

## Comparing `pulumi_wavefront-1.4.0a1684391615.tar` & `pulumi_wavefront-1.4.0a1684521558.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:41:55.156794 pulumi_wavefront-1.4.0a1684391615/
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-18 06:41:55.156794 pulumi_wavefront-1.4.0a1684391615/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:41:55.156794 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76663 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    48449 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/alert_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_app_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_aws_external_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_azure_activity_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_cloud_trail.py
--rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_cloud_watch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_gcp_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_new_relic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:41:55.156794 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/dashboard_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_default_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_derived_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_external_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_external_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_maintenance_window_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_user_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/ingestion_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/maintenance_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/metrics_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)   209561 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/user_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:41:55.156794 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-18 06:41:55.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-18 06:41:55.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:41:55.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:41:55.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 06:41:55.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 06:41:55.000000 pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 06:41:55.156794 pulumi_wavefront-1.4.0a1684391615/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-18 06:41:54.000000 pulumi_wavefront-1.4.0a1684391615/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:43:57.784058 pulumi_wavefront-1.4.0a1684521558/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-19 18:43:57.780058 pulumi_wavefront-1.4.0a1684521558/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:43:57.780058 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76663 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49247 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36453 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/alert_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46819 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_app_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_aws_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30615 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_azure_activity_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_cloud_trail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36599 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_cloud_watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24093 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29291 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_gcp_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26214 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_new_relic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:43:57.780058 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31568 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/dashboard_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24978 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_default_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_derived_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_external_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_maintenance_window_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_user_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/ingestion_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34484 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/maintenance_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12925 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/metrics_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209561 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14400 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/user_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:43:57.780058 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:43:57.784058 pulumi_wavefront-1.4.0a1684521558/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-19 18:43:57.000000 pulumi_wavefront-1.4.0a1684521558/setup.py
```

### Comparing `pulumi_wavefront-1.4.0a1684391615/PKG-INFO` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi_wavefront
-Version: 1.4.0a1684391615
+Name: pulumi-wavefront
+Version: 1.4.0a1684521558
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-wavefront/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-wavefront/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fwavefront.svg)](https://www.npmjs.com/package/@pulumi/wavefront)
 [![Python version](https://badge.fury.io/py/pulumi-wavefront.svg)](https://pypi.org/project/pulumi-wavefront)
 [![NuGet version](https://badge.fury.io/nu/pulumi.wavefront.svg)](https://badge.fury.io/nu/pulumi.wavefront)
```

### Comparing `pulumi_wavefront-1.4.0a1684391615/README.md` & `pulumi_wavefront-1.4.0a1684521558/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/__init__.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/_inputs.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/_utilities.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/alert.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,36 +35,36 @@
         :param pulumi.Input[int] minutes: The number of consecutive minutes that a series matching the condition query must 
                evaluate to "true" (non-zero value) before the alert fires.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A set of tags to assign to this resource.
         :param pulumi.Input[str] additional_information: User-supplied additional explanatory information for this alert.
                Useful for linking runbooks, migrations, etc.
         :param pulumi.Input[str] alert_type: The type of alert in Wavefront.  Either `CLASSIC` (default) 
                or `THRESHOLD`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of users or groups that can modify this resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of users or groups that can view this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of valid users or groups that can modify this resource on a tenant.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         :param pulumi.Input[str] condition: A Wavefront query that is evaluated at regular intervals (default is 1 minute).
                The alert fires and notifications are triggered when a data series matching this query evaluates
                to a non-zero value for a set number of consecutive minutes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] conditions: a string->string map of `severity` to `condition` 
                for which this alert will trigger.
         :param pulumi.Input[str] display_expression: A second query whose results are displayed in the alert user
                interface instead of the condition query.  This field is often used to display a version
                of the condition query with Boolean operators removed so that numerical values are plotted.
         :param pulumi.Input[str] name: The name of the alert as it is displayed in Wavefront.
         :param pulumi.Input[int] notification_resend_frequency_minutes: How often to re-trigger a continually failing alert. 
                If absent or <= 0, no re-triggering occurs.
-        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes.
+        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         :param pulumi.Input[int] resolve_after_minutes: The number of consecutive minutes that a firing series matching the condition
                query must evaluate to "false" (zero value) before the alert resolves.  When unset, this defaults to
                the same value as `minutes`.
         :param pulumi.Input[str] severity: Severity of the alert, valid values are `INFO`, `SMOKE`, `WARN`, `SEVERE`.
         :param pulumi.Input[str] target: A comma-separated list of the email address or integration endpoint 
                (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
                Alert target format: ({email}|pd:{pd_key}|target:{alert-target-id}).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: Targets for severity
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: A string to string map of Targets for severity.
         """
         pulumi.set(__self__, "minutes", minutes)
         pulumi.set(__self__, "tags", tags)
         if additional_information is not None:
             pulumi.set(__self__, "additional_information", additional_information)
         if alert_type is not None:
             pulumi.set(__self__, "alert_type", alert_type)
@@ -144,27 +144,27 @@
     def alert_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alert_type", value)
 
     @property
     @pulumi.getter(name="canModifies")
     def can_modifies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of users or groups that can modify this resource.
+        A list of valid users or groups that can modify this resource on a tenant.
         """
         return pulumi.get(self, "can_modifies")
 
     @can_modifies.setter
     def can_modifies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "can_modifies", value)
 
     @property
     @pulumi.getter(name="canViews")
     def can_views(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of users or groups that can view this resource.
+        A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         """
         return pulumi.get(self, "can_views")
 
     @can_views.setter
     def can_views(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "can_views", value)
 
@@ -234,15 +234,15 @@
     def notification_resend_frequency_minutes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "notification_resend_frequency_minutes", value)
 
     @property
     @pulumi.getter(name="processRateMinutes")
     def process_rate_minutes(self) -> Optional[pulumi.Input[int]]:
         """
-        The specified query is executed every `process_rate_minutes` minutes.
+        The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         """
         return pulumi.get(self, "process_rate_minutes")
 
     @process_rate_minutes.setter
     def process_rate_minutes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "process_rate_minutes", value)
 
@@ -286,15 +286,15 @@
     def target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target", value)
 
     @property
     @pulumi.getter(name="thresholdTargets")
     def threshold_targets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Targets for severity
+        A string to string map of Targets for severity.
         """
         return pulumi.get(self, "threshold_targets")
 
     @threshold_targets.setter
     def threshold_targets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "threshold_targets", value)
 
@@ -320,39 +320,39 @@
                  threshold_targets: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Alert resources.
         :param pulumi.Input[str] additional_information: User-supplied additional explanatory information for this alert.
                Useful for linking runbooks, migrations, etc.
         :param pulumi.Input[str] alert_type: The type of alert in Wavefront.  Either `CLASSIC` (default) 
                or `THRESHOLD`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of users or groups that can modify this resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of users or groups that can view this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of valid users or groups that can modify this resource on a tenant.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         :param pulumi.Input[str] condition: A Wavefront query that is evaluated at regular intervals (default is 1 minute).
                The alert fires and notifications are triggered when a data series matching this query evaluates
                to a non-zero value for a set number of consecutive minutes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] conditions: a string->string map of `severity` to `condition` 
                for which this alert will trigger.
         :param pulumi.Input[str] display_expression: A second query whose results are displayed in the alert user
                interface instead of the condition query.  This field is often used to display a version
                of the condition query with Boolean operators removed so that numerical values are plotted.
         :param pulumi.Input[int] minutes: The number of consecutive minutes that a series matching the condition query must 
                evaluate to "true" (non-zero value) before the alert fires.
         :param pulumi.Input[str] name: The name of the alert as it is displayed in Wavefront.
         :param pulumi.Input[int] notification_resend_frequency_minutes: How often to re-trigger a continually failing alert. 
                If absent or <= 0, no re-triggering occurs.
-        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes.
+        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         :param pulumi.Input[int] resolve_after_minutes: The number of consecutive minutes that a firing series matching the condition
                query must evaluate to "false" (zero value) before the alert resolves.  When unset, this defaults to
                the same value as `minutes`.
         :param pulumi.Input[str] severity: Severity of the alert, valid values are `INFO`, `SMOKE`, `WARN`, `SEVERE`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A set of tags to assign to this resource.
         :param pulumi.Input[str] target: A comma-separated list of the email address or integration endpoint 
                (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
                Alert target format: ({email}|pd:{pd_key}|target:{alert-target-id}).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: Targets for severity
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: A string to string map of Targets for severity.
         """
         if additional_information is not None:
             pulumi.set(__self__, "additional_information", additional_information)
         if alert_type is not None:
             pulumi.set(__self__, "alert_type", alert_type)
         if can_modifies is not None:
             pulumi.set(__self__, "can_modifies", can_modifies)
@@ -409,27 +409,27 @@
     def alert_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alert_type", value)
 
     @property
     @pulumi.getter(name="canModifies")
     def can_modifies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of users or groups that can modify this resource.
+        A list of valid users or groups that can modify this resource on a tenant.
         """
         return pulumi.get(self, "can_modifies")
 
     @can_modifies.setter
     def can_modifies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "can_modifies", value)
 
     @property
     @pulumi.getter(name="canViews")
     def can_views(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of users or groups that can view this resource.
+        A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         """
         return pulumi.get(self, "can_views")
 
     @can_views.setter
     def can_views(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "can_views", value)
 
@@ -512,15 +512,15 @@
     def notification_resend_frequency_minutes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "notification_resend_frequency_minutes", value)
 
     @property
     @pulumi.getter(name="processRateMinutes")
     def process_rate_minutes(self) -> Optional[pulumi.Input[int]]:
         """
-        The specified query is executed every `process_rate_minutes` minutes.
+        The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         """
         return pulumi.get(self, "process_rate_minutes")
 
     @process_rate_minutes.setter
     def process_rate_minutes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "process_rate_minutes", value)
 
@@ -576,15 +576,15 @@
     def target(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target", value)
 
     @property
     @pulumi.getter(name="thresholdTargets")
     def threshold_targets(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Targets for severity
+        A string to string map of Targets for severity.
         """
         return pulumi.get(self, "threshold_targets")
 
     @threshold_targets.setter
     def threshold_targets(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "threshold_targets", value)
 
@@ -643,39 +643,39 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] additional_information: User-supplied additional explanatory information for this alert.
                Useful for linking runbooks, migrations, etc.
         :param pulumi.Input[str] alert_type: The type of alert in Wavefront.  Either `CLASSIC` (default) 
                or `THRESHOLD`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of users or groups that can modify this resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of users or groups that can view this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of valid users or groups that can modify this resource on a tenant.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         :param pulumi.Input[str] condition: A Wavefront query that is evaluated at regular intervals (default is 1 minute).
                The alert fires and notifications are triggered when a data series matching this query evaluates
                to a non-zero value for a set number of consecutive minutes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] conditions: a string->string map of `severity` to `condition` 
                for which this alert will trigger.
         :param pulumi.Input[str] display_expression: A second query whose results are displayed in the alert user
                interface instead of the condition query.  This field is often used to display a version
                of the condition query with Boolean operators removed so that numerical values are plotted.
         :param pulumi.Input[int] minutes: The number of consecutive minutes that a series matching the condition query must 
                evaluate to "true" (non-zero value) before the alert fires.
         :param pulumi.Input[str] name: The name of the alert as it is displayed in Wavefront.
         :param pulumi.Input[int] notification_resend_frequency_minutes: How often to re-trigger a continually failing alert. 
                If absent or <= 0, no re-triggering occurs.
-        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes.
+        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         :param pulumi.Input[int] resolve_after_minutes: The number of consecutive minutes that a firing series matching the condition
                query must evaluate to "false" (zero value) before the alert resolves.  When unset, this defaults to
                the same value as `minutes`.
         :param pulumi.Input[str] severity: Severity of the alert, valid values are `INFO`, `SMOKE`, `WARN`, `SEVERE`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A set of tags to assign to this resource.
         :param pulumi.Input[str] target: A comma-separated list of the email address or integration endpoint 
                (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
                Alert target format: ({email}|pd:{pd_key}|target:{alert-target-id}).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: Targets for severity
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: A string to string map of Targets for severity.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: AlertArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -802,39 +802,39 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] additional_information: User-supplied additional explanatory information for this alert.
                Useful for linking runbooks, migrations, etc.
         :param pulumi.Input[str] alert_type: The type of alert in Wavefront.  Either `CLASSIC` (default) 
                or `THRESHOLD`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of users or groups that can modify this resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of users or groups that can view this resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_modifies: A list of valid users or groups that can modify this resource on a tenant.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] can_views: A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         :param pulumi.Input[str] condition: A Wavefront query that is evaluated at regular intervals (default is 1 minute).
                The alert fires and notifications are triggered when a data series matching this query evaluates
                to a non-zero value for a set number of consecutive minutes.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] conditions: a string->string map of `severity` to `condition` 
                for which this alert will trigger.
         :param pulumi.Input[str] display_expression: A second query whose results are displayed in the alert user
                interface instead of the condition query.  This field is often used to display a version
                of the condition query with Boolean operators removed so that numerical values are plotted.
         :param pulumi.Input[int] minutes: The number of consecutive minutes that a series matching the condition query must 
                evaluate to "true" (non-zero value) before the alert fires.
         :param pulumi.Input[str] name: The name of the alert as it is displayed in Wavefront.
         :param pulumi.Input[int] notification_resend_frequency_minutes: How often to re-trigger a continually failing alert. 
                If absent or <= 0, no re-triggering occurs.
-        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes.
+        :param pulumi.Input[int] process_rate_minutes: The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         :param pulumi.Input[int] resolve_after_minutes: The number of consecutive minutes that a firing series matching the condition
                query must evaluate to "false" (zero value) before the alert resolves.  When unset, this defaults to
                the same value as `minutes`.
         :param pulumi.Input[str] severity: Severity of the alert, valid values are `INFO`, `SMOKE`, `WARN`, `SEVERE`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A set of tags to assign to this resource.
         :param pulumi.Input[str] target: A comma-separated list of the email address or integration endpoint 
                (such as PagerDuty or webhook) to notify when the alert status changes. Multiple target types can be in the list.
                Alert target format: ({email}|pd:{pd_key}|target:{alert-target-id}).
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: Targets for severity
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] threshold_targets: A string to string map of Targets for severity.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AlertState.__new__(_AlertState)
 
         __props__.__dict__["additional_information"] = additional_information
         __props__.__dict__["alert_type"] = alert_type
@@ -872,23 +872,23 @@
         """
         return pulumi.get(self, "alert_type")
 
     @property
     @pulumi.getter(name="canModifies")
     def can_modifies(self) -> pulumi.Output[Sequence[str]]:
         """
-        A list of users or groups that can modify this resource.
+        A list of valid users or groups that can modify this resource on a tenant.
         """
         return pulumi.get(self, "can_modifies")
 
     @property
     @pulumi.getter(name="canViews")
     def can_views(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        A list of users or groups that can view this resource.
+        A list of valid users or groups that can view this resource on a tenant. Default is Empty list.
         """
         return pulumi.get(self, "can_views")
 
     @property
     @pulumi.getter
     def condition(self) -> pulumi.Output[Optional[str]]:
         """
@@ -943,15 +943,15 @@
         """
         return pulumi.get(self, "notification_resend_frequency_minutes")
 
     @property
     @pulumi.getter(name="processRateMinutes")
     def process_rate_minutes(self) -> pulumi.Output[Optional[int]]:
         """
-        The specified query is executed every `process_rate_minutes` minutes.
+        The specified query is executed every `process_rate_minutes` minutes. Default value is 5 minutes.
         """
         return pulumi.get(self, "process_rate_minutes")
 
     @property
     @pulumi.getter(name="resolveAfterMinutes")
     def resolve_after_minutes(self) -> pulumi.Output[Optional[int]]:
         """
@@ -987,11 +987,11 @@
         """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter(name="thresholdTargets")
     def threshold_targets(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Targets for severity
+        A string to string map of Targets for severity.
         """
         return pulumi.get(self, "threshold_targets")
```

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/alert_target.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/alert_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_app_dynamics.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_app_dynamics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_aws_external_id.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_aws_external_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_azure.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_azure.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_azure_activity_log.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_azure_activity_log.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_cloud_trail.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_cloud_trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_cloud_watch.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_cloud_watch.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_ec2.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_ec2.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_gcp.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_gcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_gcp_billing.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_gcp_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/cloud_integration_new_relic.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/cloud_integration_new_relic.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/config/vars.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/dashboard.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/dashboard_json.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/dashboard_json.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/derived_metric.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/event.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/external_link.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_alert.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_alert.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_alerts.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_dashboard.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_dashboards.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_dashboards.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_default_user_group.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_default_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_derived_metric.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_derived_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_derived_metrics.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_derived_metrics.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_event.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_event.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_events.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_external_link.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_external_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_external_links.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_external_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_maintenance_window.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_maintenance_window_all.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_maintenance_window_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_metrics_policy.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_role.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_roles.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_user.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_user_group.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_user_groups.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/get_users.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/ingestion_policy.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/ingestion_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/maintenance_window.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/metrics_policy.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/metrics_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/outputs.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/provider.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/role.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/service_account.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/user.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront/user_group.py` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront/user_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/PKG-INFO` & `pulumi_wavefront-1.4.0a1684521558/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
-Name: pulumi-wavefront
-Version: 1.4.0a1684391615
+Name: pulumi_wavefront
+Version: 1.4.0a1684521558
 Summary: A Pulumi package for creating and managing wavefront cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-wavefront
 Keywords: pulumi wavefront
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-wavefront/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-wavefront/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fwavefront.svg)](https://www.npmjs.com/package/@pulumi/wavefront)
 [![Python version](https://badge.fury.io/py/pulumi-wavefront.svg)](https://pypi.org/project/pulumi-wavefront)
 [![NuGet version](https://badge.fury.io/nu/pulumi.wavefront.svg)](https://badge.fury.io/nu/pulumi.wavefront)
```

### Comparing `pulumi_wavefront-1.4.0a1684391615/pulumi_wavefront.egg-info/SOURCES.txt` & `pulumi_wavefront-1.4.0a1684521558/pulumi_wavefront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_wavefront-1.4.0a1684391615/setup.py` & `pulumi_wavefront-1.4.0a1684521558/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.4.0a1684391615"
-PLUGIN_VERSION = "1.4.0-alpha.1684391615+5bcb28e2"
+VERSION = "1.4.0a1684521558"
+PLUGIN_VERSION = "1.4.0-alpha.1684521558+08d43cd3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'wavefront', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "wavefront Pulumi Package - Development Version"
 
 
 setup(name='pulumi_wavefront',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing wavefront cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

