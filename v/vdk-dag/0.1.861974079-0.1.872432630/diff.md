# Comparing `tmp/vdk-dag-0.1.861974079.tar.gz` & `tmp/vdk-dag-0.1.872432630.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-dag-0.1.861974079.tar", last modified: Tue May  9 16:11:21 2023, max compression
+gzip compressed data, was "vdk-dag-0.1.872432630.tar", last modified: Fri May 19 09:16:37 2023, max compression
```

## Comparing `vdk-dag-0.1.861974079.tar` & `vdk-dag-0.1.872432630.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/
--rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7887 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-09 16:11:10.000000 vdk-dag-0.1.861974079/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.374871 vdk-dag-0.1.861974079/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.374871 vdk-dag-0.1.861974079/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.374871 vdk-dag-0.1.861974079/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/src/vdk/plugin/dag/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/src/vdk/plugin/dag/api/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/api/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     9308 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/cached_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6078 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/dags.py
--rw-rw-rw-   0 root         (0) root         (0)     9334 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/src/vdk/plugin/dag/time_based_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8454 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-09 16:11:21.000000 vdk-dag-0.1.861974079/src/vdk_dag.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 16:11:21.378871 vdk-dag-0.1.861974079/tests/
--rw-rw-rw-   0 root         (0) root         (0)    16383 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_dag_object.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_time_based_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-09 16:11:06.000000 vdk-dag-0.1.861974079/tests/test_tracking_job_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/
+-rw-r--r--   0 root         (0) root         (0)     8454 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7887 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-05-19 09:16:26.000000 vdk-dag-0.1.872432630/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/plugin/dag/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.075389 vdk-dag-0.1.872432630/src/vdk/plugin/dag/api/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/api/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)    10184 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/cached_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7481 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6480 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     7838 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     9385 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/src/vdk/plugin/dag/time_based_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8454 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-19 09:16:37.000000 vdk-dag-0.1.872432630/src/vdk_dag.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 09:16:37.079390 vdk-dag-0.1.872432630/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    19438 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_dag_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      899 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_time_based_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2023-05-19 09:16:22.000000 vdk-dag-0.1.872432630/tests/test_tracking_job_executor.py
```

### Comparing `vdk-dag-0.1.861974079/PKG-INFO` & `vdk-dag-0.1.872432630/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.861974079
+Version: 0.1.872432630
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-dag-0.1.861974079/README.md` & `vdk-dag-0.1.872432630/README.md`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/setup.py` & `vdk-dag-0.1.872432630/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.861974079"
+__version__ = "0.1.872432630"
 
 setuptools.setup(
     name="vdk-dag",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Express dependecies between data jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/api/dag.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/api/dag.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/cached_data_job_executor.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/cached_data_job_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,18 @@
         Starts a Data Job.
 
         :param job_name: the job to start and track
         """
         job = self.__get_job(job_name)
         job.start_attempt += 1
         execution_id = self.start_new_job_execution(
-            job_name=job.job_name, team_name=job.team_name, arguments=job.arguments
+            job_name=job.job_name,
+            team_name=job.team_name,
+            started_by=job.details.get("started_by"),
+            arguments=job.arguments,
         )
         log.info(f"Starting new data job execution with id {execution_id}")
         job.execution_id = execution_id
         job.status = JobStatus.SUBMITTED.value
         job.details = self._executor.details_job(
             job.job_name, job.team_name, job.execution_id
         )
@@ -134,14 +137,28 @@
         if job.status in ACTIVE_JOB_STATUSES:
             job.status = self._executor.status_job(
                 job.job_name, job.team_name, job.execution_id
             )
         log.debug(f"Job status: {job}")
         return job.status
 
+    def execution_type(self, job_name: str, team_name: str, execution_id: str) -> str:
+        """
+        Gets the execution type of a job.
+
+        :param execution_id: the execution id of the job
+        :param team_name: the name of the owning team
+        :param job_name: the name of the job
+        :return: the job execution type (manual/scheduled)
+        """
+        details = self._executor.details_job(job_name, team_name, execution_id)
+        log.debug(f"Job execution type: {details.get('type')}")
+        # the default value for execution type is manual
+        return details.get("type", "manual")
+
     def get_finished_job_names(self):
         """
         :return: list of the names of all the finalized jobs
         """
         finalized_jobs = []
         # TODO: optimize
         # Do not call the status every time (use TTL caching)
@@ -171,15 +188,19 @@
     def get_currently_running_jobs(self):
         """
         :return: list of jobs with current status SUBMITTED or RUNNING
         """
         return [j for j in self._jobs_cache.values() if j.status in ACTIVE_JOB_STATUSES]
 
     def start_new_job_execution(
-        self, job_name: str, team_name: str, arguments: IJobArguments = None
+        self,
+        job_name: str,
+        team_name: str,
+        started_by: str = None,
+        arguments: IJobArguments = None,
     ) -> str:
         """
         Start a new data job execution.
         The stages of the process are:
             1) Get the latest available execution_id before any new
                executions have been started.
             2) Start a new execution.
@@ -189,27 +210,30 @@
         NOTE: A loop is used to handle situations, where due to some
         network instability, a socket timeout happens. The execution of
         the data job may have started, but we don't know because an execution
         id was not returned due to the exception.
 
         :param job_name: name of the data job to be executed
         :param team_name: name of the owning team
+        :param started_by: the execution type and the name of the DAG job
         :param arguments: arguments of the data job
         :return: id of the started job execution
         """
         current_retries = 0
         execution_id = None
 
         latest_available_execution_id = self.get_latest_available_execution_id(
             job_name=job_name, team=team_name
         )
 
         while current_retries < ALLOWED_RETRIES:
             try:
-                execution_id = self._executor.start_job(job_name, team_name, arguments)
+                execution_id = self._executor.start_job(
+                    job_name, team_name, started_by, arguments
+                )
                 return execution_id
             except url_exception.TimeoutError as e:
                 log.info(
                     f"A timeout exception occurred while starting the {job_name} data job. "
                     f"Exception was: {e}"
                 )
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List
 
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.api.plugin.plugin_registry import IPluginRegistry
 from vdk.internal.builtin_plugins.config.job_config import JobConfigKeys
 from vdk.internal.builtin_plugins.run.job_context import JobContext
 from vdk.internal.core.config import ConfigurationBuilder
+from vdk.internal.core.statestore import CommonStoreKeys
 from vdk.plugin.dag import dag_runner
 from vdk.plugin.dag.dag_plugin_configuration import add_definitions
 from vdk.plugin.dag.dag_plugin_configuration import DagPluginConfiguration
 
 
 class DagPlugin:
     @staticmethod
@@ -19,14 +20,18 @@
         # TODO: there should be less hacky way
         dag_runner.TEAM_NAME = context.core_context.configuration.get_value(
             JobConfigKeys.TEAM
         )
         dag_runner.DAG_CONFIG = DagPluginConfiguration(
             context.core_context.configuration
         )
+        dag_runner.JOB_NAME = context.name
+        dag_runner.EXECUTION_ID = context.core_context.state.get(
+            CommonStoreKeys.EXECUTION_ID
+        )
 
     @staticmethod
     @hookimpl
     def vdk_configure(config_builder: ConfigurationBuilder) -> None:
         """
         Here we define what configuration settings are needed for DAGs with reasonable defaults.
         """
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_plugin_configuration.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_runner.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from typing import Optional
 
 from vdk.plugin.dag.api.dag import IDagInput
 from vdk.plugin.dag.dag import Dag
 
 TEAM_NAME: Optional[str] = None
 DAG_CONFIG = None
+JOB_NAME: Optional[str] = None
+EXECUTION_ID: Optional[str] = None
 
 log = logging.getLogger(__name__)
 
 
 def get_json(obj):
     return json.loads(json.dumps(obj, default=lambda o: o.__dict__))
 
@@ -27,11 +29,11 @@
     def run_dag(self, jobs: List[Dict]):
         """
         Runs the DAG of jobs - initializes it, builds it, executes it and logs the summary.
 
         :param jobs: the list of jobs that are part of the DAG
         :return:
         """
-        dag = Dag(TEAM_NAME, DAG_CONFIG)
+        dag = Dag(TEAM_NAME, DAG_CONFIG, JOB_NAME, EXECUTION_ID)
         dag.build_dag(jobs)
         dag.execute_dag()
         log.info(f"DAG summary:\n{dag}")
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dag_validator.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dag_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/dags.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/dags.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,17 +12,24 @@
 
 class IDataJobExecutor(abc.ABC):
     """
     This module is responsible for the execution of Data Jobs.
     """
 
     @abc.abstractmethod
-    def start_job(self, job_name: str, team_name: str, arguments: IJobArguments = None):
+    def start_job(
+        self,
+        job_name: str,
+        team_name: str,
+        started_by: str = None,
+        arguments: IJobArguments = None,
+    ):
         """
         Start an execution of a data job and returns its execution id
+        :param started_by:
         :param arguments:
         :param job_name:
         :param team_name:
         :return: execution id
         """
         pass
 
@@ -36,19 +43,19 @@
         :return: status in string as defined by Control Service API
         """
         pass
 
     @abc.abstractmethod
     def details_job(self, job_name: str, team_name: str, execution_id: str) -> dict:
         """
-        Get the current status of a data job execution
+        Get the current details of a data job execution
         :param job_name:
         :param team_name:
         :param execution_id:
-        :return: status in string as defined by Control Service API
+        :return: details in string as defined by Control Service API
         """
         pass
 
     @abc.abstractmethod
     def job_executions_list(
         self, job_name: str, team_name: str
     ) -> Optional[List[DataJobExecution]]:
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     """
 
     def __init__(
         self,
         job_name: str,
         team_name: str,
         rest_api_url: str,
+        started_by: str = None,
         arguments: IJobArguments = None,
         timeout: int = 5,  # TODO: Set reasonable default
         **kwargs,
     ) -> None:
         """
 
         :param job_name: the name of the job
@@ -63,14 +64,15 @@
         :param timeout: timeout
         :param kwargs: extra parameters
         """
         self.__job_name = job_name
         self.__team_name = team_name
         self.__rest_api_url = rest_api_url
         self.__arguments = arguments
+        self.__started_by = started_by
         self.timeout = timeout
         self.deployment_id = "production"  # currently multiple deployments are not supported so this remains hardcoded
         self.auth: Optional[Authentication] = kwargs.pop("auth", None)
 
         # setting these manually to avoid using VDKConfig
         # TODO: set op ID from current job
         self.op_id = f"{uuid.uuid4().hex}"[:16]
@@ -88,29 +90,29 @@
         )
         self.http_read_retries = int(os.getenv("VDK_CONTROL_HTTP_READ_RETRIES", "6"))
 
         self.__execution_api = self._get_execution_api()
 
     def start_job_execution(self) -> str:
         """
-        Triggers a manual Datajob execution.
+        Triggers a Datajob execution.
 
         :param: request_kwargs: Request arguments to be included with the HTTP request
         """
         execution_request = DataJobExecutionRequest(
-            started_by="dag",  # TODO: specify name of dag
+            started_by=self.__started_by,
             args=self.__arguments,
         )
-        _, _, headers = self.__execution_api.data_job_execution_start_with_http_info(
+        headers = self.__execution_api.data_job_execution_start_with_http_info(
             team_name=self.__team_name,
             job_name=self.__job_name,
             deployment_id=self.deployment_id,
             data_job_execution_request=execution_request,
             _request_timeout=self.timeout,
-        )
+        ).headers
         log.debug(f"Received headers: {headers}")
 
         job_execution_id = os.path.basename(headers["Location"])
         return job_execution_id
 
     def cancel_job_execution(self, execution_id: str) -> None:
         """
@@ -134,15 +136,15 @@
         """
         return self.__execution_api.data_job_logs_download(
             team_name=self.__team_name,
             job_name=self.__job_name,
             execution_id=execution_id,
         ).logs
 
-    def get_job_execution_status(self, execution_id: str) -> DataJobExecution:
+    def get_job_execution_details(self, execution_id: str) -> DataJobExecution:
         """
         Returns the execution status for a particular job execution.
 
         :param execution_id: ID of the job execution
         :return: The execution status object listing details about the status of this particular execution
         """
         job_execution: DataJobExecution = self.__execution_api.data_job_execution_read(
@@ -182,15 +184,15 @@
                 log.info(
                     f"Timeout: Data Job execution {execution_id} is not complete after {timeout_seconds}s"
                 )
                 return None
             time.sleep(wait_seconds)
 
             try:
-                job_execution = self.get_job_execution_status(execution_id)
+                job_execution = self.get_job_execution_details(execution_id)
                 job_status = job_execution.status
             except Exception as err:
                 log.info("VDK Control Service returned error: %s", err)
                 continue
 
             if job_status == JobStatus.SUCCEEDED:
                 log.info(f"Job status: {job_execution}")
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/remote_data_job_executor.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/remote_data_job_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,43 @@
 
 
 class RemoteDataJobExecutor(IDataJobExecutor):
     """
     This module is responsible for executing remote Data Jobs.
     """
 
-    def start_job(self, job_name: str, team_name: str, arguments: IJobArguments = None):
+    def start_job(
+        self,
+        job_name: str,
+        team_name: str,
+        started_by: str = None,
+        arguments: IJobArguments = None,
+    ):
         vdk_cfg = VDKConfig()
         job = RemoteDataJob(
-            job_name, team_name, vdk_cfg.control_service_rest_api_url, arguments
+            job_name,
+            team_name,
+            vdk_cfg.control_service_rest_api_url,
+            started_by,
+            arguments,
         )
         return job.start_job_execution()
         # catch error on 409
 
     def status_job(self, job_name: str, team_name: str, execution_id: str) -> str:
         vdk_cfg = VDKConfig()
         job = RemoteDataJob(job_name, team_name, vdk_cfg.control_service_rest_api_url)
-        status = job.get_job_execution_status(execution_id)
-        return status.status
+        details = job.get_job_execution_details(execution_id)
+        return details.status
 
     def details_job(self, job_name: str, team_name: str, execution_id: str) -> dict:
         vdk_cfg = VDKConfig()
         job = RemoteDataJob(job_name, team_name, vdk_cfg.control_service_rest_api_url)
-        status = job.get_job_execution_status(execution_id)
-        return status.to_dict()
+        details = job.get_job_execution_details(execution_id)
+        return details.to_dict()
 
     def job_executions_list(
         self, job_name: str, team_name: str
     ) -> Optional[List[DataJobExecution]]:
         vdk_cfg = VDKConfig()
         job = RemoteDataJob(job_name, team_name, vdk_cfg.control_service_rest_api_url)
         executions_list = job.get_job_executions()
```

### Comparing `vdk-dag-0.1.861974079/src/vdk/plugin/dag/time_based_queue.py` & `vdk-dag-0.1.872432630/src/vdk/plugin/dag/time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/src/vdk_dag.egg-info/PKG-INFO` & `vdk-dag-0.1.872432630/src/vdk_dag.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-dag
-Version: 0.1.861974079
+Version: 0.1.872432630
 Summary: Express dependecies between data jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-dag-0.1.861974079/src/vdk_dag.egg-info/SOURCES.txt` & `vdk-dag-0.1.872432630/src/vdk_dag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/tests/test_dag.py` & `vdk-dag-0.1.872432630/tests/test_dag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import os
+import re
 import time
 from datetime import date
 from datetime import datetime
 from unittest import mock
 
 from click.testing import Result
 from pytest_httpserver.pytest_plugin import PluginHTTPServer
@@ -53,15 +54,15 @@
         return self.dags_max_concurrent_running_jobs_value
 
 
 dummy_config = DummyDAGPluginConfiguration()
 
 
 class TestDAG:
-    def _prepare(self):
+    def _prepare(self, dag_name=None):
         rest_api_url = self.httpserver.url_for("")
         team_name = "team-awesome"
         if self.jobs is None:
             self.jobs = [("job" + str(i), [200], "succeeded", 0) for i in range(1, 5)]
 
         started_jobs = dict()
 
@@ -98,14 +99,15 @@
                         id=job_name,
                         job_name=job_name,
                         logs_url="http://url",
                         deployment=DataJobDeployment(),
                         start_time="2021-09-24T14:14:03.922Z",
                         status=actual_job_status,
                         message="foo",
+                        started_by="manual/" + dag_name,
                     )
                     response_data = json.dumps(
                         execution.to_dict(), indent=4, default=json_serial
                     )
                     return Response(
                         response_data,
                         status=200,
@@ -118,24 +120,64 @@
             self.httpserver.expect_request(
                 uri=f"/data-jobs/for-team/{team_name}/jobs/{job_name}/executions/{job_name}",
                 method="GET",
             ).respond_with_handler(
                 exec_handler(job_name, job_status, execution_duration)
             )
 
+            class MatchExecutionID:
+                def __eq__(self, other):
+                    return (
+                        re.match(
+                            r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}-\d+$",
+                            other.split("/")[-1],
+                        )
+                        is not None
+                    )
+
+            def exec_id_handler(job_name):
+                def _handler_fn(r: Request):
+                    execution: DataJobExecution = DataJobExecution(
+                        id=job_name,
+                        job_name=job_name,
+                        logs_url="http://url",
+                        deployment=DataJobDeployment(),
+                        start_time="2021-09-24T14:14:03.922Z",
+                        status="succeeded",
+                        message="foo",
+                        started_by="manual/" + dag_name,
+                    )
+                    response_data = json.dumps(
+                        execution.to_dict(), indent=4, default=json_serial
+                    )
+                    return Response(
+                        response_data,
+                        status=200,
+                        headers=None,
+                        content_type="application/json",
+                    )
+
+                return _handler_fn
+
+            self.httpserver.expect_request(
+                uri=MatchExecutionID(),
+                method="GET",
+            ).respond_with_handler(exec_id_handler(job_name))
+
             def exec_list_handler(job_name):
                 def _handler_fn(r: Request):
                     execution: DataJobExecution = DataJobExecution(
                         id=f"{job_name}-latest",
                         job_name=job_name,
                         logs_url="http://url",
                         deployment=DataJobDeployment(),
                         start_time="2021-09-24T14:14:03.922Z",
                         status="succeeded",
                         message="foo",
+                        started_by="manual/" + dag_name,
                     )
                     response_data = json.dumps(
                         [execution.to_dict()], indent=4, default=json_serial
                     )
                     return Response(
                         response_data,
                         status=200,
@@ -148,19 +190,19 @@
             self.httpserver.expect_request(
                 uri=f"/data-jobs/for-team/{team_name}/jobs/{job_name}/executions",
                 method="GET",
             ).respond_with_handler(exec_list_handler(job_name))
 
         return rest_api_url
 
-    def _set_up(self, jobs=None, additional_env_vars=None):
+    def _set_up(self, jobs=None, additional_env_vars=None, dag_name=None):
         self.httpserver = PluginHTTPServer()
         self.httpserver.start()
         self.jobs = jobs
-        self.api_url = self._prepare()
+        self.api_url = self._prepare(dag_name)
         self.env_vars = {"VDK_CONTROL_SERVICE_REST_API_URL": self.api_url}
         if additional_env_vars is not None:
             self.env_vars.update(additional_env_vars)
 
     def _run_dag(self, dag_name):
         with mock.patch.dict(
             os.environ,
@@ -184,118 +226,125 @@
             self.env_vars,
         ):
             assert isinstance(result.exception, error)
             # no other request should be tried as the DAG fails
             assert len(self.httpserver.log) == 0
 
     def test_dag(self):
-        self._set_up()
+        dag = "dag"
+        self._set_up(dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag")
+            result = self._run_dag(dag)
             cli_assert_equal(0, result)
             self.httpserver.stop()
 
     def test_dag_error(self):
         jobs = [
             ("job1", [200], "succeeded"),
             ("job2", [200], "succeeded"),
             ("job3", [200], "platform_error"),
             ("job4", [200], "succeeded"),
         ]
-        self._set_up(jobs)
+        dag = "dag"
+        self._set_up(jobs, dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag")
+            result = self._run_dag(dag)
             cli_assert_equal(1, result)
             self.httpserver.stop()
 
     def test_dag_fail_false(self):
         jobs = [
             ("job1", [200], "succeeded"),
             ("job2", [200], "platform_error"),
             ("job3", [200], "succeeded"),
             ("job4", [200], "succeeded"),
         ]
-        self._set_up(jobs)
+        dag = "dag"
+        self._set_up(jobs, dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag")
+            result = self._run_dag(dag)
             cli_assert_equal(0, result)
             self.httpserver.stop()
 
     def test_dag_conflict(self):
         jobs = [
             ("job1", [409, 200], "succeeded"),
             ("job2", [500, 200], "succeeded"),
             ("job3", [200], "succeeded"),
             ("job4", [200], "succeeded"),
         ]
+        dag = "dag"
         env_vars = {
             "VDK_DAGS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS": "0",
             "VDK_DAGS_DELAYED_JOBS_MIN_DELAY_SECONDS": "0",
         }
-        self._set_up(jobs, env_vars)
+        self._set_up(jobs, env_vars, dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag")
+            result = self._run_dag(dag)
             cli_assert_equal(0, result)
             self.httpserver.stop()
 
     def test_dag_cannot_start_job(self):
         jobs = [
             ("job1", [401, 200], "succeeded"),
             ("job2", [200], "succeeded"),
             ("job3", [200], "succeeded"),
             ("job4", [200], "succeeded"),
         ]
-        self._set_up(jobs)
+        dag = "dag"
+        self._set_up(jobs, dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag")
+            result = self._run_dag(dag)
             cli_assert_equal(1, result)
-            # we should have 2 requests in the log, one to get a list
-            # of all executions, and one for the failing data job
-            # no other request should be tried as the DAG fails
-            assert len(self.httpserver.log) == 2
+            # we should have 3 requests in the log, one to get
+            # the execution type of the dag,a list of all
+            # executions and one for the failing data job no
+            # other request should be tried as the DAG fails
+            assert len(self.httpserver.log) == 3
             self.httpserver.stop()
 
     def test_dag_long_running(self):
         jobs = [
             ("job1", [200], "succeeded", 3),  # execution duration is 3 seconds
             ("job2", [200], "succeeded"),
             ("job3", [200], "succeeded"),
             ("job4", [200], "succeeded"),
         ]
+        dag = "dag"
         # we set 5 seconds more than execution duration of 3 set above
         dummy_config.dags_time_between_status_check_seconds_value = 5
         dummy_config.dags_dag_execution_check_time_period_seconds_value = 0
 
-        self._set_up(jobs, [])
+        self._set_up(jobs, dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag")
+            result = self._run_dag(dag)
             cli_assert_equal(0, result)
             job1_requests = [
                 req
                 for req, res in self.httpserver.log
                 if req.method == "GET" and req.base_url.endswith("job1")
             ]
             # We have 1 call during start, 1 call at finish and 1 call that returns running and 1 that returns the final
@@ -304,33 +353,40 @@
             # not a good idea but we need to verify that we are not hammering the API Server somehow ...
             assert len(job1_requests) == 4
 
             # let's make sure something else is not generating more requests then expected
             # if implementation is changed the number below would likely change.
             # If the new count is not that big we can edit it here to pass the test,
             # if the new count is too big, we have an issue that need to be investigated.
-            assert len(self.httpserver.log) == 21
+            assert len(self.httpserver.log) == 22
             self.httpserver.stop()
 
-    """
     def test_dag_concurrent_running_jobs_limit(self):
         jobs = [("job" + str(i), [200], "succeeded", 1) for i in range(1, 8)]
+        dag = "dag-exceed-limit"
 
         dummy_config.dags_max_concurrent_running_jobs_value = 2
         dummy_config.dags_delayed_jobs_min_delay_seconds_value = 1
         dummy_config.dags_delayed_jobs_randomized_added_delay_seconds_value = 1
         dummy_config.dags_time_between_status_check_seconds_value = 1
 
-        self._set_up(jobs, [])
+        env_vars = {
+            "VDK_DAGS_MAX_CONCURRENT_RUNNING_JOBS": "2",
+            "VDK_DAGS_DELAYED_JOBS_RANDOMIZED_ADDED_DELAY_SECONDS": "1",
+            "VDK_DAGS_DELAYED_JOBS_MIN_DELAY_SECONDS": "1",
+            "VDK_DAGS_TIME_BETWEEN_STATUS_CHECK_SECONDS_VALUE": "1",
+        }
+
+        self._set_up(jobs, env_vars, dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag-exceed-limit")
+            result = self._run_dag(dag)
             expected_max_running_jobs = int(
                 os.getenv("VDK_DAGS_MAX_CONCURRENT_RUNNING_JOBS", "2")
             )
             # keep track of the number of running jobs at any given time
             running_jobs = set()
             for request, response in self.httpserver.log:
                 if "executions" in request.path:
@@ -346,15 +402,33 @@
                             execution = execution[0]
                         if execution["status"] == "succeeded":
                             running_jobs.discard(execution["job_name"])
             cli_assert_equal(0, result)
             # assert that all the jobs finished successfully
             assert len(running_jobs) == 0
             self.httpserver.stop()
-    """
+
+    def test_dag_execution_type_propagation(self):
+        dag = "dag"
+        self._set_up(dag_name=dag)
+        with mock.patch.dict(
+            os.environ,
+            self.env_vars,
+        ):
+            self.runner = CliEntryBasedTestRunner(dag_plugin)
+            result = self._run_dag(dag)
+            for request, response in self.httpserver.log:
+                if "executions" in request.path:
+                    if request.method == "GET":
+                        execution = json.loads(response.response[0])
+                        if isinstance(execution, list):
+                            execution = execution[0]
+                        assert execution["started_by"] == "manual/" + dag
+            cli_assert_equal(0, result)
+            self.httpserver.stop()
 
     def _test_dag_validation(self, dag_name):
         self._set_up()
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
@@ -376,35 +450,37 @@
     def test_dag_not_allowed_job_key(self):
         self._test_dag_validation("dag-not-allowed-job-key")
 
     def test_dag_wrong_job_arguments_type(self):
         self._test_dag_validation("dag-wrong-job-arguments-type")
 
     def test_dag_arguments(self):
-        self._set_up()
+        dag = "dag-arguments"
+        self._set_up(dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag-arguments")
+            result = self._run_dag(dag)
             cli_assert_equal(0, result)
             job2_arguments = self._get_job_arguments("job2")
             assert len(job2_arguments) == 2
             assert job2_arguments == {"table_name": "test_table", "counter": 123}
             self.httpserver.stop()
 
     def test_dag_empty_arguments(self):
-        self._set_up()
+        dag = "dag-empty-arguments"
+        self._set_up(dag_name=dag)
         with mock.patch.dict(
             os.environ,
             self.env_vars,
         ):
             self.runner = CliEntryBasedTestRunner(dag_plugin)
-            result = self._run_dag("dag-empty-arguments")
+            result = self._run_dag(dag)
             cli_assert_equal(0, result)
             job2_arguments = self._get_job_arguments("job2")
             assert len(job2_arguments) == 0
             self.httpserver.stop()
 
     def test_dag_wrong_job_key_type(self):
         self._test_dag_validation("dag-wrong-job-key-type")
```

### Comparing `vdk-dag-0.1.861974079/tests/test_dag_object.py` & `vdk-dag-0.1.872432630/tests/test_dag_object.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/tests/test_time_based_queue.py` & `vdk-dag-0.1.872432630/tests/test_time_based_queue.py`

 * *Files identical despite different names*

### Comparing `vdk-dag-0.1.861974079/tests/test_tracking_job_executor.py` & `vdk-dag-0.1.872432630/tests/test_tracking_job_executor.py`

 * *Files identical despite different names*

