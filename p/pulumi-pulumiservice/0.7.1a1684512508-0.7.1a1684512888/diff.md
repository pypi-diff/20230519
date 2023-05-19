# Comparing `tmp/pulumi_pulumiservice-0.7.1a1684512508.tar.gz` & `tmp/pulumi_pulumiservice-0.7.1a1684512888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_pulumiservice-0.7.1a1684512508.tar", last modified: Fri May 19 16:12:22 2023, max compression
+gzip compressed data, was "dist/pulumi_pulumiservice-0.7.1a1684512888.tar", last modified: Fri May 19 16:18:25 2023, max compression
```

## Comparing `pulumi_pulumiservice-0.7.1a1684512508.tar` & `pulumi_pulumiservice-0.7.1a1684512888.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/deployment_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/org_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/stack_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/team_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/team_stack_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-19 16:12:22.000000 pulumi_pulumiservice-0.7.1a1684512508/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/deployment_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/org_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/stack_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_stack_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/setup.py
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/PKG-INFO` & `pulumi_pulumiservice-0.7.1a1684512888/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_pulumiservice
-Version: 0.7.1a1684512508
+Version: 0.7.1a1684512888
 Summary: A native Pulumi package for creating and managing Pulumi Service constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
 Description: # Pulumi Service Provider
         
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/README.md` & `pulumi_pulumiservice-0.7.1a1684512888/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/__init__.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/_enums.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/_inputs.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/_utilities.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/access_token.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/config/vars.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/deployment_settings.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/deployment_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,23 @@
                  operation_context: Optional[pulumi.Input[pulumi.InputType['DeploymentSettingsOperationContextArgs']]] = None,
                  organization: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  source_context: Optional[pulumi.Input[pulumi.InputType['DeploymentSettingsSourceContextArgs']]] = None,
                  stack: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Deployment settings configure Pulumi Deployments for a stack
+        Deployment settings configure Pulumi Deployments for a stack.
+
+        ### Import
+
+        Deployment settings can be imported using the `id`, which for deployment settings is {org}/{project}/{stack} e.g.,
+
+        ```sh
+         $ pulumi import pulumiservice:index:DeploymentSettings my_settings `my-org/my-project/my-stack`
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['DeploymentSettingsExecutorContextArgs']] executor_context: Settings related to the deployment executor.
         :param pulumi.Input[pulumi.InputType['DeploymentSettingsGithubArgs']] github: GitHub settings for the deployment.
         :param pulumi.Input[pulumi.InputType['DeploymentSettingsOperationContextArgs']] operation_context: Settings related to the Pulumi operation environment during the deployment.
         :param pulumi.Input[str] organization: Organization name.
@@ -157,15 +165,23 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DeploymentSettingsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Deployment settings configure Pulumi Deployments for a stack
+        Deployment settings configure Pulumi Deployments for a stack.
+
+        ### Import
+
+        Deployment settings can be imported using the `id`, which for deployment settings is {org}/{project}/{stack} e.g.,
+
+        ```sh
+         $ pulumi import pulumiservice:index:DeploymentSettings my_settings `my-org/my-project/my-stack`
+        ```
 
         :param str resource_name: The name of the resource.
         :param DeploymentSettingsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/org_access_token.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/org_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/provider.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/stack_tag.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/stack_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/team.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/team_access_token.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/team_stack_permission.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_stack_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice/webhook.py` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,22 @@
                  project_name: Optional[pulumi.Input[str]] = None,
                  secret: Optional[pulumi.Input[str]] = None,
                  stack_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Pulumi Webhooks allow you to notify external services of events happening within your Pulumi organization or stack. For example, you can trigger a notification whenever a stack is updated. Whenever an event occurs, Pulumi will send an HTTP POST request to all registered webhooks. The webhook can then be used to emit some notification, start running integration tests, or even update additional stacks.
 
+        ### Import
+
+        Pulumi webhooks can be imported using the `id`, which for webhooks is `{org}/{project}/{stack}/{webhook-name}` e.g.,
+
+        ```sh
+         $ pulumi import pulumiservice:index:Webhook my_webhook my-org/my-project/my-stack/4b0d0671
+        ```
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] active: Indicates whether this webhook is enabled or not.
         :param pulumi.Input[str] display_name: The friendly name displayed in the Pulumi Service.
         :param pulumi.Input[Sequence[pulumi.Input['WebhookFilters']]] filters: Optional set of filters to apply to the webhook. See [webhook docs](https://www.pulumi.com/docs/intro/pulumi-service/webhooks/#filters) for more information.
         :param pulumi.Input['WebhookFormat'] format: Format of the webhook payload. Can be either `raw` or `slack`. Defaults to `raw`.
         :param pulumi.Input[str] organization_name: Name of the organization.
@@ -197,14 +205,22 @@
     def __init__(__self__,
                  resource_name: str,
                  args: WebhookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Pulumi Webhooks allow you to notify external services of events happening within your Pulumi organization or stack. For example, you can trigger a notification whenever a stack is updated. Whenever an event occurs, Pulumi will send an HTTP POST request to all registered webhooks. The webhook can then be used to emit some notification, start running integration tests, or even update additional stacks.
 
+        ### Import
+
+        Pulumi webhooks can be imported using the `id`, which for webhooks is `{org}/{project}/{stack}/{webhook-name}` e.g.,
+
+        ```sh
+         $ pulumi import pulumiservice:index:Webhook my_webhook my-org/my-project/my-stack/4b0d0671
+        ```
+
         :param str resource_name: The name of the resource.
         :param WebhookArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(WebhookArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/PKG-INFO` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-pulumiservice
-Version: 0.7.1a1684512508
+Version: 0.7.1a1684512888
 Summary: A native Pulumi package for creating and managing Pulumi Service constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
 Description: # Pulumi Service Provider
         
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/pulumi_pulumiservice.egg-info/SOURCES.txt` & `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512508/setup.py` & `pulumi_pulumiservice-0.7.1a1684512888/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.1a1684512508"
-PLUGIN_VERSION = "0.7.1-alpha.1684512508+5abc43d8"
+VERSION = "0.7.1a1684512888"
+PLUGIN_VERSION = "0.7.1-alpha.1684512888+4fa1a7d9"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pulumiservice', PLUGIN_VERSION])
         except OSError as error:
```

