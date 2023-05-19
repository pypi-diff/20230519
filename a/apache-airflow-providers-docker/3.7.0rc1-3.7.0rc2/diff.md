# Comparing `tmp/apache-airflow-providers-docker-3.7.0rc1.tar.gz` & `tmp/apache-airflow-providers-docker-3.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-docker-3.7.0rc1.tar", last modified: Tue May 16 15:53:43 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-docker-3.7.0rc2.tar", last modified: Fri May 19 17:52:18 2023, max compression
```

## Comparing `apache-airflow-providers-docker-3.7.0rc1.tar` & `apache-airflow-providers-docker-3.7.0rc2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.7.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.7.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    16588 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15061 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-16 15:39:21.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-03-16 20:46:35.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0 root         (0) root         (0)     3259 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7953 2023-04-14 11:39:41.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/docker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22731 2023-05-03 19:47:07.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker_swarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16588 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-docker-3.7.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-16 15:53:43.000000 apache-airflow-providers-docker-3.7.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-16 15:53:42.000000 apache-airflow-providers-docker-3.7.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.7.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:17.000000 apache-airflow-providers-docker-3.7.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-docker-3.7.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    16931 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15404 2023-05-19 17:52:17.000000 apache-airflow-providers-docker-3.7.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-05-19 12:05:39.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-03-16 20:46:35.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-05-19 17:52:17.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-04-14 11:39:41.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/hooks/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23367 2023-05-18 08:56:29.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-02-24 18:43:53.000000 apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/docker_swarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16931 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-docker-3.7.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-05-19 17:52:18.000000 apache-airflow-providers-docker-3.7.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-19 17:52:17.000000 apache-airflow-providers-docker-3.7.0rc2/setup.py
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/LICENSE` & `apache-airflow-providers-docker-3.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/MANIFEST.in` & `apache-airflow-providers-docker-3.7.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/PKG-INFO` & `apache-airflow-providers-docker-3.7.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
@@ -125,14 +125,19 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``adding docker port expose capability (#30730)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/README.rst` & `apache-airflow-providers-docker-3.7.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
@@ -92,14 +92,19 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``adding docker port expose capability (#30730)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/__init__.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-import airflow
+__all__ = ["__version__"]
 
-__all__ = ["version"]
+__version__ = "3.7.0"
 
-version = "3.7.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-docker:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-docker:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/__init__.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/decorators/docker.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/decorators/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/get_provider_info.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/__init__.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/hooks/docker.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/hooks/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/__init__.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,14 +155,18 @@
     :param log_opts_max_file: The maximum number of log files that can be present.
         If rolling the logs creates excess files, the oldest file is removed.
         Only effective when max-size is also set. A positive integer. Defaults to 1.
     :param ipc_mode: Set the IPC mode for the container.
     :param skip_on_exit_code: If task exits with this exit code, leave the task
         in ``skipped`` state (default: None). If set to ``None``, any non-zero
         exit code will be treated as a failure.
+    :param port_bindings: Publish a container's port(s) to the host. It is a
+        dictionary of value where the key indicates the port to open inside the container
+        and value indicates the host port that binds to the container port.
+        Incompatible with ``host`` in ``network_mode``.
     """
 
     template_fields: Sequence[str] = ("image", "command", "environment", "env_file", "container_name")
     template_fields_renderers = {"env_file": "yaml"}
     template_ext: Sequence[str] = (
         ".sh",
         ".bash",
@@ -213,14 +217,15 @@
         timeout: int = DEFAULT_TIMEOUT_SECONDS,
         device_requests: list[DeviceRequest] | None = None,
         log_opts_max_size: str | None = None,
         log_opts_max_file: str | None = None,
         ipc_mode: str | None = None,
         skip_exit_code: int | None = None,
         skip_on_exit_code: int | Container[int] | None = None,
+        port_bindings: dict | None = None,
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.api_version = api_version
         if type(auto_remove) == bool:
             warnings.warn(
                 "bool value for auto_remove is deprecated, please use 'never', 'success', or 'force' instead",
@@ -289,14 +294,17 @@
         self.skip_on_exit_code = (
             skip_on_exit_code
             if isinstance(skip_on_exit_code, Container)
             else [skip_on_exit_code]
             if skip_on_exit_code
             else []
         )
+        self.port_bindings = port_bindings or {}
+        if self.port_bindings and self.network_mode == "host":
+            raise ValueError("Port bindings is not supported in the host network mode")
 
     @cached_property
     def hook(self) -> DockerHook:
         """Create and return an DockerHook (cached)."""
         tls_config = DockerHook.construct_tls_config(
             ca_cert=self.tls_ca_cert,
             client_cert=self.tls_client_cert,
@@ -355,22 +363,24 @@
         env_file_vars = {}
         if self.env_file is not None:
             env_file_vars = self.unpack_environment_variables(self.env_file)
         self.container = self.cli.create_container(
             command=self.format_command(self.command),
             name=self.container_name,
             environment={**env_file_vars, **self.environment, **self._private_environment},
+            ports=list(self.port_bindings),
             host_config=self.cli.create_host_config(
                 auto_remove=False,
                 mounts=target_mounts,
                 network_mode=self.network_mode,
                 shm_size=self.shm_size,
                 dns=self.dns,
                 dns_search=self.dns_search,
                 cpu_shares=int(round(self.cpus * 1024)),
+                port_bindings=self.port_bindings,
                 mem_limit=self.mem_limit,
                 cap_add=self.cap_add,
                 extra_hosts=self.extra_hosts,
                 privileged=self.privileged,
                 device_requests=self.device_requests,
                 log_config=LogConfig(config=docker_log_config),
                 ipc_mode=self.ipc_mode,
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/airflow/providers/docker/operators/docker_swarm.py` & `apache-airflow-providers-docker-3.7.0rc2/airflow/providers/docker/operators/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/PKG-INFO` & `apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.7.0rc1
+Version: 3.7.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.0rc1``
+Release: ``3.7.0rc2``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
@@ -125,14 +125,19 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``adding docker port expose capability (#30730)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
 
 3.6.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt` & `apache-airflow-providers-docker-3.7.0rc2/apache_airflow_providers_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.0rc1/pyproject.toml` & `apache-airflow-providers-docker-3.7.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
+    # "D400", WIP: see #31135
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/setup.cfg` & `apache-airflow-providers-docker-3.7.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -54,10 +54,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.docker.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.docker
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-docker-3.7.0rc1/setup.py` & `apache-airflow-providers-docker-3.7.0rc2/setup.py`

 * *Files identical despite different names*

