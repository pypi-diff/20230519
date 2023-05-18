# Comparing `tmp/coiled-0.6.5.dev9.tar.gz` & `tmp/coiled-0.6.6.dev1.tar.gz`

## Comparing `coiled-0.6.5.dev9.tar` & `coiled-0.6.6.dev1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/context.py
--rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/magic.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/software.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/types.py
--rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    87872 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    60907 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/pyproject.toml
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/context.py
+-rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/magic.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/software.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/types.py
+-rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/websockets.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    88052 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    61035 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.6.dev1/PKG-INFO
```

### Comparing `coiled-0.6.5.dev9/coiled/__init__.py` & `coiled-0.6.6.dev1/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/analytics.py` & `coiled-0.6.6.dev1/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cluster.py` & `coiled-0.6.6.dev1/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/coiled.yaml` & `coiled-0.6.6.dev1/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/context.py` & `coiled-0.6.6.dev1/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/core.py` & `coiled-0.6.6.dev1/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/exceptions.py` & `coiled-0.6.6.dev1/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/magic.py` & `coiled-0.6.6.dev1/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/scan.py` & `coiled-0.6.6.dev1/coiled/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         # that claims to have this pypi name
         for possible_name in [name] + [p["name"] for p in packages]:
             if pip_env.get(possible_name):
                 found = True
                 pip_package = pip_env[possible_name]
                 if isinstance(pip_package, CondaPlaceHolder):
                     # find the conda package that actually matches with what is importable
-                    importable_package = next(p for p in packages if p["name"] == pip_package["name"])
+                    importable_package = next(p for p in packages if p["name"].lower() == pip_package["name"].lower())
                     filtered_conda[name] = importable_package
                     break
                 elif next((p for p in packages if p["version"] == pip_package["version"]), None):
                     # if the versions match, we can fall back to using the conda version
                     pip_env.pop(possible_name, None)
                     filtered_conda[name] = next((p for p in packages if p["version"] == pip_package["version"]))
                     break
```

### Comparing `coiled-0.6.5.dev9/coiled/software.py` & `coiled-0.6.6.dev1/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/types.py` & `coiled-0.6.6.dev1/coiled/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -199,7 +199,29 @@
 
     @property
     def vm_arch(self) -> Literal["x86_64", "arm64"]:
         if self == ArchitectureTypesEnum.ARM64:
             return "arm64"
         else:
             return self.value
+
+
+class ClusterDetailsState(TypedDict):
+    state: str
+    reason: str
+    updated: str
+
+
+class ClusterDetailsProcess(TypedDict):
+    created: str
+    name: str
+    current_state: ClusterDetailsState
+    instance: dict
+
+
+class ClusterDetails(TypedDict):
+    id: int
+    name: str
+    workers: List[ClusterDetailsProcess]
+    scheduler: Optional[ClusterDetailsProcess]
+    current_state: ClusterDetailsState
+    created: str
```

### Comparing `coiled-0.6.5.dev9/coiled/utils.py` & `coiled-0.6.6.dev1/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/websockets.py` & `coiled-0.6.6.dev1/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/_beta/cluster.py` & `coiled-0.6.6.dev1/coiled/_beta/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,35 +922,38 @@
                     "\tpip install --upgrade dask distributed"
                 )
             raise
 
     @track_context
     async def _start(self):
         did_error = False
+        cluster_created = False
+
         await self.cloud
         try:
             cloud = self.cloud
             self.account = self.account or self.cloud.default_account
 
             (
                 scheduler_vm_types_to_use,
                 worker_vm_types_to_use,
             ) = await self._get_cluster_vm_types_to_use()
 
             # check_create_or_reuse has the side effect of creating a name
             # if none is assigned
-            should_create = await self._check_create_or_reuse()
+            should_try_create = await self._check_create_or_reuse()
+            self.name = self.name or (self.account or cloud.default_account) + "-" + str(uuid.uuid4())[:10]
             assert self.name
 
             # Set shutdown_on_close here instead of in __init__ to make sure
             # the dask config default isn't used when we are reusing a cluster
             if self.shutdown_on_close is None:
-                self.shutdown_on_close = should_create and dask.config.get("coiled.shutdown-on-close")
+                self.shutdown_on_close = should_try_create and dask.config.get("coiled.shutdown-on-close")
 
-            if should_create:
+            if should_try_create:
                 user_provider = await self._get_account_cloud_provider_name()
 
                 # Update backend options for cluster based on the friendlier kwargs
                 if self.scheduler_gpu:
                     if user_provider == "gcp":
                         self.backend_options = {
                             **GCP_SCHEDULER_GPU,
@@ -1057,15 +1060,15 @@
                     parse_identifier(
                         self.software_environment,
                         property_name="software_environment",
                         can_have_revision=False,
                     )
 
                 senv_v2_id = await self._determine_senv(architecture=architecture, gpu_enabled=self._is_gpu_cluster)
-                self.cluster_id = await cloud._create_cluster(
+                self.cluster_id, cluster_created = await cloud._create_cluster(
                     account=self.account,
                     name=self.name,
                     workers=self._start_n_workers,
                     software_environment=self.software_environment,
                     worker_class=self.worker_class,
                     worker_options=self.worker_options,
                     worker_disk_size=self.worker_disk_size,
@@ -1084,22 +1087,22 @@
                     senv_v2_id=senv_v2_id,
                     private_to_creator=self.private_to_creator,
                 )
 
             if not self.cluster_id:
                 raise RuntimeError(f"Failed to find/create cluster {self.name}")
 
-            if should_create:
+            if cluster_created:
                 logger.info(
                     f"Creating Cluster (name: {self.name}, {self.details_url} ). This might take a few minutes..."
                 )
             else:
                 logger.info(f"Attaching to existing cluster (name: {self.name}, {self.details_url} )")
 
-            await self._attach_to_cluster(is_new_cluster=should_create)
+            await self._attach_to_cluster(is_new_cluster=cluster_created)
             await super()._start()
 
             # Set adaptive maximum value based on available config and user quota
             self._set_adaptive_options()
         except Exception as e:
             if self._asynchronous:
                 did_error = True
@@ -1170,15 +1173,15 @@
     def _maybe_log_summary(self, cluster_details):
         now = time.time()
         if self._last_logged_state_summary is None or now > self._last_logged_state_summary + 5:
             logger.info(summarize_status(cluster_details))
             self._last_logged_state_summary = now
 
     @track_context
-    async def _wait_until_ready(self, is_new_cluster) -> None:
+    async def _wait_until_ready(self, is_new_cluster: bool) -> None:
         cloud = self.cloud
         cluster_id = self._assert_cluster_id()
         timeout_at = (
             datetime.datetime.now() + datetime.timedelta(seconds=self.timeout) if self.timeout is not None else None
         )
         self._latest_dt_seen = None
```

### Comparing `coiled-0.6.5.dev9/coiled/_beta/core.py` & `coiled-0.6.6.dev1/coiled/_beta/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,15 +702,15 @@
         gcp_worker_gpu_count: Optional[int] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[AWSOptions, GCPOptions, dict]] = None,
         use_scheduler_public_ip: Optional[bool] = None,
         use_dashboard_https: Optional[bool] = None,
         private_to_creator: Optional[bool] = None,
-    ) -> int:
+    ) -> Tuple[int, bool]:
         # TODO (Declarative): support these args, or decide not to
         # https://gitlab.com/coiled/cloud/-/issues/4305
 
         if scheduler_class is not None:
             raise ValueError("scheduler_class is not supported in beta/new Coiled yet")
 
         account = account or self.default_account
@@ -826,15 +826,15 @@
             else:
                 if "message" in response_json:
                     raise ServerError(response_json["message"])
                 if "detail" in response_json:
                     raise ServerError(response_json["detail"])
                 raise ServerError(response_json)
 
-        return response_json["id"]
+        return response_json["id"], response_json["existing"]
 
     @overload
     def create_cluster(
         self: Cloud[Sync],
         name: str,
         *,
         software: Optional[str] = None,
@@ -849,15 +849,15 @@
         dask_config: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-    ) -> int:
+    ) -> Tuple[int, bool]:
         ...
 
     @overload
     def create_cluster(
         self: Cloud[Async],
         name: str,
         *,
@@ -873,15 +873,15 @@
         dask_config: Optional[Dict] = None,
         private_to_creator: Optional[bool] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-    ) -> Awaitable[int]:
+    ) -> Awaitable[Tuple[int, bool]]:
         ...
 
     def create_cluster(
         self,
         name: str,
         *,
         software: Optional[str] = None,
@@ -896,15 +896,15 @@
         private_to_creator: Optional[bool] = None,
         dask_config: Optional[Dict] = None,
         scheduler_vm_types: Optional[list] = None,
         worker_gpu_type: Optional[str] = None,
         worker_vm_types: Optional[list] = None,
         worker_disk_size: Optional[int] = None,
         backend_options: Optional[Union[dict, AWSOptions, GCPOptions]] = None,
-    ) -> Union[int, Awaitable[int]]:
+    ) -> Union[Tuple[int, bool], Awaitable[Tuple[int, bool]]]:
         return self._sync(
             self._create_cluster,
             name=name,
             software_environment=software,
             worker_class=worker_class,
             worker_options=worker_options,
             scheduler_options=scheduler_options,
@@ -1721,15 +1721,15 @@
         Dictionary of dask config to put on cluster
 
     See Also
     --------
     coiled.Cluster
     """
     with CloudBeta(account=account) as cloud:
-        return cloud.create_cluster(
+        cluster, existing = cloud.create_cluster(
             name=name,
             software=software,
             worker_options=worker_options,
             scheduler_options=scheduler_options,
             account=account,
             workers=workers,
             environ=environ,
@@ -1737,14 +1737,15 @@
             dask_config=dask_config,
             private_to_creator=private_to_creator,
             backend_options=backend_options,
             worker_vm_types=worker_vm_types,
             worker_disk_size=worker_disk_size,
             scheduler_vm_types=scheduler_vm_types,
         )
+        return cluster
 
 
 @list_docstring
 def list_clusters(account=None, max_pages: Optional[int] = None):
     with CloudBeta() as cloud:
         return cloud.list_clusters(account=account, max_pages=max_pages)
```

### Comparing `coiled-0.6.5.dev9/coiled/_beta/cwi_log_link.py` & `coiled-0.6.6.dev1/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/_beta/states.py` & `coiled-0.6.6.dev1/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/_beta/widgets/__init__.py` & `coiled-0.6.6.dev1/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/_beta/widgets/rich.py` & `coiled-0.6.6.dev1/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/_beta/widgets/util.py` & `coiled-0.6.6.dev1/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/config.py` & `coiled-0.6.6.dev1/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/core.py` & `coiled-0.6.6.dev1/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/curl.py` & `coiled-0.6.6.dev1/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/env.py` & `coiled-0.6.6.dev1/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/login.py` & `coiled-0.6.6.dev1/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/package_sync.py` & `coiled-0.6.6.dev1/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/utils.py` & `coiled-0.6.6.dev1/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/cluster/__init__.py` & `coiled-0.6.6.dev1/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/cluster/better_logs.py` & `coiled-0.6.6.dev1/coiled/cli/cluster/better_logs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import re
 import time
 from datetime import datetime, timedelta, timezone
-from typing import List, Optional
+from typing import Optional
 
 import click
 from rich.console import Console
 
 import coiled
 
 from ..utils import CONTEXT_SETTINGS
+from .utils import find_cluster
 
 COLORS = [
     "green",
     "yellow",
     "blue",
     "magenta",
     "cyan",
@@ -126,52 +127,24 @@
     system = system or combined
     label = label.lower()
 
     if tail and until:
         raise click.ClickException("You can't use --until when tailing logs.")
 
     with coiled.Cloud(account=account) as cloud:
-        if cluster and cluster.isnumeric():
-            cluster_id = int(cluster)
-        elif cluster:
-            # get cluster by name
-            try:
-                clusters = cloud.get_clusters_by_name(name=cluster)
-                if clusters:
-                    recent_cluster = clusters[-1]
-                else:
-                    raise click.ClickException(
-                        f"Unable to find cluster with name '{cluster}' in account '{cloud.default_account}'"
-                    )
-
-                if tail and recent_cluster["current_state"]["state"] in (
-                    "stopped",
-                    "error",
-                ):
-                    tail = False
-                    console.print(
-                        f"[red]Cluster state is {recent_cluster['current_state']['state']} so not tailing.[/red]"
-                    )
+        cluster_info = find_cluster(cloud, cluster or "")
 
-                cluster_id = recent_cluster["id"]
+    cluster_id = cluster_info["id"]
 
-            except coiled.errors.DoesNotExist:
-                cluster_id = None
-        else:
-            # default to most recent cluster
-            clusters = cloud.list_clusters(max_pages=1)
-            if not clusters:
-                raise ValueError(f"Unable to find any clusters for account '{cloud.default_account}'")
-            match = max(clusters, key=lambda c: c["id"])
-            cluster_id = match["id"]
-
-        if not cluster_id:
-            raise click.ClickException(f"Unable to find cluster `{cluster}`")
-
-        cluster_info = cloud.cluster_details(cluster_id)
+    if tail and cluster_info["current_state"]["state"] in (
+        "stopped",
+        "error",
+    ):
+        tail = False
+        console.print(f"[red]Cluster state is {cluster_info['current_state']['state']} so not tailing.[/red]")
 
     # instance ID's for which to show logs, key maps to label to use
     instances = {}
     if not no_scheduler and cluster_info.get("scheduler", {}).get("instance"):
         scheduler_id = cluster_info["scheduler"]["instance"]["id"]
         instances[scheduler_id] = {
             "label": "scheduler" if label != "none" else "",
@@ -264,30 +237,14 @@
         if tail:
             # TODO stop tailing once cluster is stopped/errored (future MR)
             time.sleep(interval)
         else:
             break
 
 
-def match_cluster(clusters: List[dict], cluster: str) -> dict:
-    if cluster.isnumeric():
-        matches = [c for c in clusters if c["id"] == int(cluster)]
-        if len(matches) == 1:
-            return matches[0]
-        elif len(matches) > 1:
-            raise ValueError(f"Multiple clusters match '{cluster}'")
-
-    # try to match on cluster name
-    matches = sorted([c for c in clusters if c["name"] == cluster], key=lambda c: c["id"])
-    if matches:
-        return matches[-1]
-
-    raise ValueError(f"No clusters match '{cluster}'")
-
-
 def event_dedupe_key(event):
     return f'{event["timestamp"]}#{event["instance_id"]}#{event["message"]}'
 
 
 def print_events(console, events, instances: dict, pretty=True, show_all_timestamps=False):
     for e in events:
         console.print(format_log_event(e, instances, pretty=pretty, show_all_timestamps=show_all_timestamps))
```

### Comparing `coiled-0.6.5.dev9/coiled/cli/cluster/logs.py` & `coiled-0.6.6.dev1/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/cluster/ssh.py` & `coiled-0.6.6.dev1/coiled/cli/cluster/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import click
 from rich import print
 
 import coiled
 
 from ..utils import CONTEXT_SETTINGS
+from .utils import find_cluster
 
 
 def open_ssh(address: str, key: str, jump_to_address: Optional[str] = None):
     """Open an SSH session, relies on `ssh` and `ssh-add` (agent)."""
     if not add_key_to_agent(address, key, t=5):
         return
 
@@ -77,15 +78,15 @@
     # print(ssh_command)
     print(f"===Starting SSH session to {ssh_target_label}===")
     subprocess.run(ssh_command, shell=True)
     print("===SSH session closed===")
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
-@click.argument("cluster")
+@click.argument("cluster", default="", required=False)
 @click.option(
     "--private",
     default=False,
     is_flag=True,
     help="Use private IP address of scheduler (default is public IP address)",
 )
 @click.option(
@@ -103,26 +104,16 @@
     "--delete-key",
     default=False,
     is_flag=True,
     help="Just delete ssh key from local OpenSSH agent",
 )
 def ssh(cluster: str, private: bool, worker: Optional[str], add_key: bool, delete_key: bool):
     with coiled.Cloud() as cloud:
-        if cluster.isnumeric():
-            cluster_id = int(cluster)
-        else:
-            try:
-                cluster_id = cloud.get_cluster_by_name(name=cluster)
-            except coiled.errors.DoesNotExist:
-                cluster_id = None
-
-        if not cluster_id:
-            print(f"Unable to find cluster `{cluster}`")
-            return
-
+        cluster_info = find_cluster(cloud, cluster)
+        cluster_id = cluster_info["id"]
         ssh_info = cloud.get_ssh_key(cluster_id=cluster_id, worker=worker)
 
     scheduler_address = ssh_info["scheduler_private_address"] if private else ssh_info["scheduler_public_address"]
 
     if add_key:
         # just add the key, maybe you want to use rsync or something like that
         add_key_to_agent(scheduler_address, key=ssh_info["private_key"])
```

### Comparing `coiled-0.6.5.dev9/coiled/cli/notebook/__init__.py` & `coiled-0.6.6.dev1/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/notebook/notebook.py` & `coiled-0.6.6.dev1/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/setup/__init__.py` & `coiled-0.6.6.dev1/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/setup/amp.py` & `coiled-0.6.6.dev1/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/setup/aws.py` & `coiled-0.6.6.dev1/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/setup/entry.py` & `coiled-0.6.6.dev1/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/setup/gcp.py` & `coiled-0.6.6.dev1/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/cli/setup/prometheus.py` & `coiled-0.6.6.dev1/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/coiled/v2/__init__.py` & `coiled-0.6.6.dev1/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/LICENSE` & `coiled-0.6.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/README.md` & `coiled-0.6.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/pyproject.toml` & `coiled-0.6.6.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev9/PKG-INFO` & `coiled-0.6.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.5.dev9
+Version: 0.6.6.dev1
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.5.dev9 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.6.dev1 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
```

