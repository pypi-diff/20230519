# Comparing `tmp/coiled-0.6.5.dev7.tar.gz` & `tmp/coiled-0.6.5.dev9.tar.gz`

## Comparing `coiled-0.6.5.dev7.tar` & `coiled-0.6.5.dev9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/analytics.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/context.py
--rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/magic.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/software.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/types.py
--rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/websockets.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    86022 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    60907 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/login.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/pyproject.toml
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.5.dev7/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/analytics.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/coiled.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/context.py
+-rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/exceptions.py
+-rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/magic.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/software.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/types.py
+-rw-r--r--   0        0        0    49062 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/websockets.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    87872 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    60907 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/login.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0    11294 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/README.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/pyproject.toml
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 coiled-0.6.5.dev9/PKG-INFO
```

### Comparing `coiled-0.6.5.dev7/coiled/__init__.py` & `coiled-0.6.5.dev9/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/analytics.py` & `coiled-0.6.5.dev9/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cluster.py` & `coiled-0.6.5.dev9/coiled/cluster.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/coiled.yaml` & `coiled-0.6.5.dev9/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/context.py` & `coiled-0.6.5.dev9/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/core.py` & `coiled-0.6.5.dev9/coiled/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/exceptions.py` & `coiled-0.6.5.dev9/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/magic.py` & `coiled-0.6.5.dev9/coiled/magic.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/scan.py` & `coiled-0.6.5.dev9/coiled/scan.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/software.py` & `coiled-0.6.5.dev9/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/types.py` & `coiled-0.6.5.dev9/coiled/types.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/utils.py` & `coiled-0.6.5.dev9/coiled/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/websockets.py` & `coiled-0.6.5.dev9/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/_beta/cluster.py` & `coiled-0.6.5.dev9/coiled/_beta/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,22 @@
     Parameters
     ----------
     n_workers
         Number of workers in this cluster. Defaults to 4.
     name
         Name to use for identifying this cluster. Defaults to ``None``.
     software
-        Name of the software environment to use.
+        Name of the software environment to use; this allows you to use and re-use existing
+        Coiled software environments, and should not be used with package sync or when specifying
+        a container to use for this specific cluster.
+    container
+        Name or URI of container image to use; when using a pre-made container image with Coiled,
+        this allows you to skip the step of explicitly creating a Coiled software environment
+        from that image. Note that this should not be used with package sync or when specifying
+        an existing Coiled software environment.
     worker_class
         Worker class to use. Defaults to :class:`distributed.nanny.Nanny`.
     worker_options
         Mapping with keyword arguments to pass to ``worker_class``. Defaults
         to ``{}``.
     worker_vm_types
         List of instance types that you would like workers to use, default instance type
@@ -284,14 +291,15 @@
     _instances = weakref.WeakSet()
 
     def __init__(
         self: ClusterSyncAsync,
         name: Optional[str] = None,
         *,
         software: Optional[str] = None,
+        container: Optional[str] = None,
         n_workers: int = 4,
         worker_class: Optional[str] = None,
         worker_options: Optional[dict] = None,
         worker_vm_types: Optional[list] = None,
         worker_cpu: Optional[Union[int, List[int]]] = None,
         worker_memory: Optional[Union[str, List[str]]] = None,
         worker_disk_size: Optional[int] = None,
@@ -335,16 +343,22 @@
         arm: Optional[bool] = None,
     ):
         # NOTE:
         # this attribute is only updated while we wait for cluster to come up
         self.errored_worker_count: int = 0
         self.init_time = datetime.datetime.now()
         type(self)._instances.add(self)
-        if package_sync and software:
-            raise ValueError("Both parameters 'software' and 'package_sync'" "were passed. Please only pass one")
+
+        senv_kwargs = {"package_sync": package_sync, "software": software, "container": container}
+        set_senv_kwargs = [name for name, value in senv_kwargs.items() if value]
+        if len(set_senv_kwargs) > 1:
+            raise ValueError(
+                f"Multiple software environment parameters are set: {', '.join(set_senv_kwargs)}. "
+                "You must use only one of these."
+            )
         self.package_sync = bool(package_sync)  # TODO: this should be mutually exclusive with passing a software env
         self.package_sync_ignore = package_sync_ignore
         if isinstance(package_sync, list):
             # ensure python is always included
             self.package_sync_only = set(package_sync)
             self.package_sync_only.add("python")
         else:
@@ -420,17 +434,21 @@
         self.timeout = timeout if timeout is not None else self.cloud.default_cluster_timeout
 
         # Set cluster attributes from kwargs (first choice) or dask config
 
         self.private_to_creator = (
             dask.config.get("coiled.private-to-creator") if private_to_creator is None else private_to_creator
         )
+
+        # FIXME what happens when no kwargs passed but coiled.software is set in dask config?
         self.software_environment = software or dask.config.get("coiled.software")
-        if not software and not package_sync:
+        self.software_container = container
+        if not container and not software and not package_sync:
             self.package_sync = True
+
         self.worker_class = worker_class or dask.config.get("coiled.worker.class")
         self.worker_cpu = worker_cpu or cast(Union[int, List[int]], dask.config.get("coiled.worker.cpu"))
 
         if isinstance(worker_cpu, int) and worker_cpu <= 1:
             if not arm:
                 raise ValueError("`worker_cpu` should be at least 2 for x86 instance types.")
             elif worker_cpu < 1:
@@ -976,23 +994,14 @@
                 # avoid creating the cluster if it's not valid.
                 #
                 # (We can't do this check earlier because we don't know until now if we're
                 # creating a cluster, and if we're not then "_start_n_workers" may be the wrong
                 # number of workers...)
                 parse_wait_for_workers(self._start_n_workers, self._wait_for_workers_arg)
 
-                # Validate software environment name, setting `can_have_revision` to False since
-                # we don't seem to be using this yet.
-                if not self.package_sync:
-                    parse_identifier(
-                        self.software_environment,
-                        property_name="software_environment",
-                        can_have_revision=False,
-                    )
-
                 # Determine software environment (legacy or package sync)
                 # TODO: Add GCP support for architecture detection
                 architecture = (
                     ArchitectureTypesEnum.ARM64
                     if (
                         user_provider == "aws"
                         and all(
@@ -1014,23 +1023,47 @@
                 # (It also catches if our code to pick ARM instances types returns an x86 instance type.)
                 if architecture != self.arch:
                     # TODO (future PR) more specific error about which instance type doesn't match
                     raise RuntimeError(
                         f"Requested cluster architecture ({self.arch.vm_arch}) does not match "
                         f"architecture of some instance types ({scheduler_vm_types_to_use}, {worker_vm_types_to_use})."
                     )
-                # TODO (future PR) still used strict mode for GPU cluster if local env also has GPU
+                # TODO (future PR) still use strict mode for GPU cluster if local env also has GPU
                 if (
                     platform.machine() == architecture
                     and platform.system() == "Linux"
                     and not is_system_python()
                     and not self._is_gpu_cluster
                 ):
                     self.package_sync_strict = True
 
+                # create an ad hoc software environment if container was specified
+                if self.software_container:
+                    # make a valid software env name unique for this container
+                    image_and_tag = self.software_container.split("/")[-1]
+                    uri_uuid = str(uuid.uuid5(uuid.NAMESPACE_DNS, self.software_container))
+                    container_senv_name = re.sub(r"[^A-Za-z0-9-_]", "_", f"{image_and_tag}-{self.arch}-{uri_uuid}")
+
+                    await cloud._create_software_environment(
+                        name=container_senv_name,
+                        container=self.software_container,
+                        account=self.account,
+                        architecture=self.arch,
+                    )
+                    self.software_environment = container_senv_name
+
+                # Validate software environment name, setting `can_have_revision` to False since
+                # we don't seem to be using this yet.
+                if not self.package_sync:
+                    parse_identifier(
+                        self.software_environment,
+                        property_name="software_environment",
+                        can_have_revision=False,
+                    )
+
                 senv_v2_id = await self._determine_senv(architecture=architecture, gpu_enabled=self._is_gpu_cluster)
                 self.cluster_id = await cloud._create_cluster(
                     account=self.account,
                     name=self.name,
                     workers=self._start_n_workers,
                     software_environment=self.software_environment,
                     worker_class=self.worker_class,
```

### Comparing `coiled-0.6.5.dev7/coiled/_beta/core.py` & `coiled-0.6.5.dev9/coiled/_beta/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/_beta/cwi_log_link.py` & `coiled-0.6.5.dev9/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/_beta/states.py` & `coiled-0.6.5.dev9/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/_beta/widgets/__init__.py` & `coiled-0.6.5.dev9/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/_beta/widgets/rich.py` & `coiled-0.6.5.dev9/coiled/_beta/widgets/rich.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/_beta/widgets/util.py` & `coiled-0.6.5.dev9/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/config.py` & `coiled-0.6.5.dev9/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/core.py` & `coiled-0.6.5.dev9/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/curl.py` & `coiled-0.6.5.dev9/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/env.py` & `coiled-0.6.5.dev9/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/login.py` & `coiled-0.6.5.dev9/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/package_sync.py` & `coiled-0.6.5.dev9/coiled/cli/package_sync.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/utils.py` & `coiled-0.6.5.dev9/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/cluster/__init__.py` & `coiled-0.6.5.dev9/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/cluster/better_logs.py` & `coiled-0.6.5.dev9/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/cluster/logs.py` & `coiled-0.6.5.dev9/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/cluster/ssh.py` & `coiled-0.6.5.dev9/coiled/cli/cluster/ssh.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/notebook/__init__.py` & `coiled-0.6.5.dev9/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/notebook/notebook.py` & `coiled-0.6.5.dev9/coiled/cli/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/setup/__init__.py` & `coiled-0.6.5.dev9/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/setup/amp.py` & `coiled-0.6.5.dev9/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/setup/aws.py` & `coiled-0.6.5.dev9/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/setup/entry.py` & `coiled-0.6.5.dev9/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/setup/gcp.py` & `coiled-0.6.5.dev9/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/cli/setup/prometheus.py` & `coiled-0.6.5.dev9/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/coiled/v2/__init__.py` & `coiled-0.6.5.dev9/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/LICENSE` & `coiled-0.6.5.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/README.md` & `coiled-0.6.5.dev9/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/pyproject.toml` & `coiled-0.6.5.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.5.dev7/PKG-INFO` & `coiled-0.6.5.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.5.dev7
+Version: 0.6.5.dev9
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
-Metadata-Version: 2.1 Name: coiled Version: 0.6.5.dev7 Project-URL: Homepage,
+Metadata-Version: 2.1 Name: coiled Version: 0.6.5.dev9 Project-URL: Homepage,
 https://coiled.io Maintainer-email: Coiled
 coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
 jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
```

