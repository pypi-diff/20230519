# Comparing `tmp/helsing_scm-0.1.0.post0.tar.gz` & `tmp/helsing_scm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helsing_scm-0.1.0.post0.tar", max compression
+gzip compressed data, was "helsing_scm-0.2.0.tar", max compression
```

## Comparing `helsing_scm-0.1.0.post0.tar` & `helsing_scm-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      998 2023-05-16 11:16:42.680037 helsing_scm-0.1.0.post0/LICENSE
--rw-r--r--   0        0        0     3581 2023-05-17 00:36:39.323869 helsing_scm-0.1.0.post0/README.md
--rw-r--r--   0        0        0     1681 2023-05-19 12:05:39.336649 helsing_scm-0.1.0.post0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-05-19 12:05:39.340649 helsing_scm-0.1.0.post0/src/helsing/scm/__init__.py
--rw-r--r--   0        0        0     2586 2023-05-19 09:53:57.439708 helsing_scm-0.1.0.post0/src/helsing/scm/__main__.py
--rw-r--r--   0        0        0        0 2023-05-16 11:16:42.680037 helsing_scm-0.1.0.post0/src/helsing/scm/py.typed
--rw-r--r--   0        0        0      161 2023-05-19 09:53:41.519631 helsing_scm-0.1.0.post0/src/helsing/scm/resources/__init__.py
--rw-r--r--   0        0        0     1001 2023-05-19 09:53:41.519631 helsing_scm-0.1.0.post0/src/helsing/scm/resources/v1alpha/AwsAccount.py
--rw-r--r--   0        0        0     3587 2023-05-19 09:53:41.519631 helsing_scm-0.1.0.post0/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py
--rw-r--r--   0        0        0      239 2023-05-19 09:53:41.559631 helsing_scm-0.1.0.post0/src/helsing/scm/resources/v1alpha/__init__.py
--rw-r--r--   0        0        0     2070 2023-05-19 09:53:57.459709 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/__init__.py
--rw-r--r--   0        0        0      426 2023-05-19 09:53:57.475709 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/__init__.py
--rw-r--r--   0        0        0     2570 2023-05-19 09:53:57.487709 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/account_service.py
--rw-r--r--   0        0        0     2230 2023-05-19 09:53:57.483708 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/create_account.py
--rw-r--r--   0        0        0     4387 2023-05-19 09:53:41.519631 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/settings.py
--rw-r--r--   0        0        0      301 2023-05-19 09:53:57.467708 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-19 09:53:41.519631 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/account_service.py
--rw-r--r--   0        0        0     4835 2023-05-19 09:53:57.467708 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/create_workspace.py
--rw-r--r--   0        0        0     1555 2023-05-19 09:53:41.519631 helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/settings.py
--rw-r--r--   0        0        0      888 2023-05-16 13:22:02.179812 helsing_scm-0.1.0.post0/src/helsing/scm/utils/develop.py
--rw-r--r--   0        0        0      680 2023-05-16 22:09:24.316728 helsing_scm-0.1.0.post0/src/helsing/scm/utils/templating.py
--rw-r--r--   0        0        0      513 2023-05-16 13:57:46.413910 helsing_scm-0.1.0.post0/src/helsing/scm/utils/types.py
--rw-r--r--   0        0        0     4345 1970-01-01 00:00:00.000000 helsing_scm-0.1.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-05-16 11:16:42.680037 helsing_scm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3581 2023-05-17 00:36:39.323869 helsing_scm-0.2.0/README.md
+-rw-r--r--   0        0        0     1675 2023-05-19 12:27:28.398825 helsing_scm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-05-19 12:27:28.398825 helsing_scm-0.2.0/src/helsing/scm/__init__.py
+-rw-r--r--   0        0        0     2661 2023-05-19 12:25:21.926250 helsing_scm-0.2.0/src/helsing/scm/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:16:42.680037 helsing_scm-0.2.0/src/helsing/scm/py.typed
+-rw-r--r--   0        0        0      161 2023-05-19 09:53:41.519631 helsing_scm-0.2.0/src/helsing/scm/resources/__init__.py
+-rw-r--r--   0        0        0     1000 2023-05-19 12:19:18.312362 helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/AwsAccount.py
+-rw-r--r--   0        0        0     3586 2023-05-19 12:19:25.152424 helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py
+-rw-r--r--   0        0        0      239 2023-05-19 09:53:41.559631 helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-19 09:53:57.459709 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-19 09:53:57.475709 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/__init__.py
+-rw-r--r--   0        0        0     2570 2023-05-19 09:53:57.487709 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/account_service.py
+-rw-r--r--   0        0        0     2326 2023-05-19 12:24:16.217957 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/create_account.py
+-rw-r--r--   0        0        0     4566 2023-05-19 12:21:07.165025 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/settings.py
+-rw-r--r--   0        0        0      301 2023-05-19 09:53:57.467708 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-19 09:53:41.519631 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/account_service.py
+-rw-r--r--   0        0        0     4927 2023-05-19 12:24:28.730014 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/create_workspace.py
+-rw-r--r--   0        0        0     1627 2023-05-19 12:23:49.733833 helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/settings.py
+-rw-r--r--   0        0        0      888 2023-05-16 13:22:02.179812 helsing_scm-0.2.0/src/helsing/scm/utils/develop.py
+-rw-r--r--   0        0        0      680 2023-05-16 22:09:24.316728 helsing_scm-0.2.0/src/helsing/scm/utils/templating.py
+-rw-r--r--   0        0        0      513 2023-05-16 13:57:46.413910 helsing_scm-0.2.0/src/helsing/scm/utils/types.py
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 helsing_scm-0.2.0/PKG-INFO
```

### Comparing `helsing_scm-0.1.0.post0/LICENSE` & `helsing_scm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/README.md` & `helsing_scm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/pyproject.toml` & `helsing_scm-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "helsing-scm"
-version = "0.1.0.post0"
+version = "0.2.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "helsing/scm", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/__main__.py` & `helsing_scm-0.2.0/src/helsing/scm/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from logging import basicConfig, getLogger
 from pathlib import Path
 from subprocess import DEVNULL, run
 
 from adjudicator import Rule, RulesEngine
-from equilibrium import Resource, ResourceContext, Service
+from equilibrium import Namespace, Resource, ResourceContext, Service
 from rich.logging import RichHandler
 from typer import Argument, Typer
 
 from helsing.scm.tfcodegen import generate_terraform_code
 
 logger = getLogger(__name__)
 app = Typer(pretty_exceptions_enable=False)
@@ -64,14 +64,15 @@
         level="INFO",
         format="%(message)s",
         datefmt="[%X]",
         handlers=[RichHandler(rich_tracebacks=True)],
     )
 
     context = ResourceContext.create(ResourceContext.InMemoryBackend())
+    context.resources.put(Namespace.create_resource("default"))
     for resource_type in get_resources():
         logger.info("Register resource type '%s'", resource_type.TYPE)
         context.resource_types.register(resource_type)
     for service_type in get_services():
         logger.info("Register service '%s' for resource type '%s'", service_type.SERVICE_ID, service_type.RESOURCE_TYPE)
         context.services.register(service_type)
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/resources/v1alpha/AwsAccount.py` & `helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/AwsAccount.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from helsing.scm import DOMAIN
 
 ACCOUNT_NAME_REGEX = r"^[a-zA-Z0-9][a-zA-Z0-9._-]*$"
 
 
 @dataclass(frozen=True)
-class AwsAccount(Resource.Spec, apiVersion=f"{DOMAIN}/v1alpha1", kind="AwsAccount", namespaced=False):
+class AwsAccount(Resource.Spec, apiVersion=f"{DOMAIN}/v1alpha1", kind="AwsAccount", namespaced=True):
     """
     Represents an AWS account.
     """
 
     #: The name of the AWS account in the AWS console.
     accountName: str
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py` & `helsing_scm-0.2.0/src/helsing/scm/resources/v1alpha/TerraformWorkspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     #: should not conflict with variables specified in the #TerraformWorkspace.variables list.
     variables: list[Variable] = field(default_factory=list)
 
     type: Literal["ApiDriven"] = "ApiDriven"
 
 
 @dataclass(frozen=True)
-class TerraformWorkspace(Resource.Spec, apiVersion=f"{DOMAIN}/v1alpha1", kind="TerraformWorkspace", namespaced=False):
+class TerraformWorkspace(Resource.Spec, apiVersion=f"{DOMAIN}/v1alpha1", kind="TerraformWorkspace", namespaced=True):
     """
     Represents a Terraorm workspace which may be given access to an AWS account.
     """
 
     #: The name of the Terraform workspace.
     workspaceName: str
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/__init__.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/__init__.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/account_service.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/account_service.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/create_account.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/create_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 @rule
 def create_aws_account(context: ResourceContext, aws_account: Resource[AwsAccount]) -> AwsAccountCreationCode:
     """
     Generate Terraform code that creates an AWS account and stores its credentials in Vault.
     """
 
-    config = AwsTerraformCodegenSettings.get(context)
+    assert aws_account.metadata.namespace is not None
+    config = AwsTerraformCodegenSettings.get(context, namespace=aws_account.metadata.namespace)
     module = config.spec.terraformModule.as_terraform_module()
 
     normalized_name = aws_account.metadata.name.replace("-", "_")
 
     code = template(
         """
         module "aws_account_${normalized_name}" {
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/aws/settings.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/aws/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Any, Literal, Sequence
 
 from equilibrium import Resource, ResourceContext
 
-from helsing.scm import DOMAIN, GIT_REPOSITORY_URL
+from helsing.scm import DOMAIN, GIT_REPOSITORY_URL, __version__
 from helsing.scm.utils.develop import get_develop_root
 from helsing.scm.utils.types import FrozenDict, HashableMapping
 
 # TODO(@NiklasRosenstein): Databind will deserialize Sequence as a list; but we'd actually
 #       want that to be an immutable sequence type. We should maybe update databind to support this.
 JsonValue = str | int | float | bool | FrozenDict[str, Any] | Sequence[Any]
 
@@ -47,14 +47,16 @@
         match self.source:
             case "Local":
                 source = str(get_develop_root() / "modules" / self.name)
             case "Remote":
                 source = f"git::{GIT_REPOSITORY_URL}//modules/{self.name}"
                 if self.ref is not None:
                     source += f"?ref={self.ref}"
+                else:
+                    source += f"?ref={__version__}"
             case _:
                 raise ValueError(f"Invalid source {self.source!r}")
 
         return TerraformModule(
             source=source,
             version=None,
             additionalInputVariables=self.additionalInputVariables,
@@ -84,15 +86,15 @@
 
 
 @dataclass(frozen=True)
 class AwsTerraformCodegenSettings(
     Resource.Spec,
     apiVersion=f"{DOMAIN}/v1alpha1",
     kind="AwsTerraformCodegenSettings",
-    namespaced=False,
+    namespaced=True,
 ):
     """
     Contains settings for Terraform code generation related to AWS account creation.
     """
 
     #: The Terraform module that is used to instantiate the AWS account. The module must have, at minimum, the
     #: following inputs varibales:
@@ -106,18 +108,18 @@
     #: - `account_id`: The AWS account ID.
     #: - `access_key`: The AWS access key.
     #: - `secret_key`: The AWS secret key.
     #: - `admin_role_arn`: The AWS administrator role ARN in the account.
     terraformModule: ScmModule | TerraformModule
 
     @staticmethod
-    def get(context: ResourceContext) -> Resource[AwsTerraformCodegenSettings]:
-        resources = context.resources.list(AwsTerraformCodegenSettings)
+    def get(context: ResourceContext, namespace: str) -> Resource[AwsTerraformCodegenSettings]:
+        resources = context.resources.list(AwsTerraformCodegenSettings, namespace=namespace)
         if len(resources) == 0:
-            raise RuntimeError("No AwsTerraformCodegenSettings resource found.")
+            raise RuntimeError(f"No AwsTerraformCodegenSettings resource found in namespace {namespace!r}.")
         if len(resources) > 1:
-            raise RuntimeError("Multiple AwsTerraformCodegenSettings resources found.")
+            raise RuntimeError(f"Multiple AwsTerraformCodegenSettings resources found in namespace {namespace!r}.")
         return resources[0]
 
 
 def get_resources() -> list[type[Resource.Spec]]:
     return [AwsTerraformCodegenSettings]
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/account_service.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/account_service.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/create_workspace.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/create_workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     context: ResourceContext,
     workspace: Resource[TerraformWorkspace],
 ) -> TerraformWorkspaceCreationCode:
     """
     Generate Terraform code that creates a Terraform workspace using the "tfe" provider.
     """
 
-    settings = TerraformWorkspaceCodegenSettings.get(context)
+    assert workspace.metadata.namespace is not None
+    settings = TerraformWorkspaceCodegenSettings.get(context, namespace=workspace.metadata.namespace)
     terraform_module = settings.spec.terraformModule.as_terraform_module()
 
     normalized_name = workspace.metadata.name.replace("-", "_")
 
     variables = list(workspace.spec.variables)
     provider_variables: list[Variable] = []
     provider_snippets: list[str] = []
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/tfcodegen/tfe/settings.py` & `helsing_scm-0.2.0/src/helsing/scm/tfcodegen/tfe/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 
 
 @dataclass(frozen=True)
 class TerraformWorkspaceCodegenSettings(
     Resource.Spec,
     apiVersion=f"{DOMAIN}/v1alpha1",
     kind="TerraformWorkspaceCodegenSettings",
-    namespaced=False,
+    namespaced=True,
 ):
     """
     Contains settings for Terraform code generation related to TFE workspace creation.
     """
 
     #: The Terraform module that is used to instantiate the AWS account. The module must have, at minimum, the
     #: following inputs varibales:
     #:
     #: - `variables`: A map of variable configurations that are assigned to the workspace. See #Variable.
     #: - `configuration`: A string that represents the Terraform code to execute as part of the workspace.
     terraformModule: ScmModule | TerraformModule
 
     @staticmethod
-    def get(context: ResourceContext) -> Resource[TerraformWorkspaceCodegenSettings]:
-        resources = context.resources.list(TerraformWorkspaceCodegenSettings)
+    def get(context: ResourceContext, namespace: str) -> Resource[TerraformWorkspaceCodegenSettings]:
+        resources = context.resources.list(TerraformWorkspaceCodegenSettings, namespace=namespace)
         if len(resources) == 0:
-            raise RuntimeError("No TerraformWorkspaceCodegenSettings resource found.")
+            raise RuntimeError(f"No TerraformWorkspaceCodegenSettings resource found in {namespace!r}.")
         if len(resources) > 1:
-            raise RuntimeError("Multiple TerraformWorkspaceCodegenSettings resources found.")
+            raise RuntimeError(f"Multiple TerraformWorkspaceCodegenSettings resources found in {namespace!r}.")
         return resources[0]
 
 
 def get_resources() -> list[type[Resource.Spec]]:
     return [TerraformWorkspaceCodegenSettings]
```

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/utils/develop.py` & `helsing_scm-0.2.0/src/helsing/scm/utils/develop.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/utils/templating.py` & `helsing_scm-0.2.0/src/helsing/scm/utils/templating.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/src/helsing/scm/utils/types.py` & `helsing_scm-0.2.0/src/helsing/scm/utils/types.py`

 * *Files identical despite different names*

### Comparing `helsing_scm-0.1.0.post0/PKG-INFO` & `helsing_scm-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helsing-scm
-Version: 0.1.0.post0
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

