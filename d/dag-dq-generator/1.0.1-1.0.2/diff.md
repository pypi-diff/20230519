# Comparing `tmp/dag-dq-generator-1.0.1.tar.gz` & `tmp/dag-dq-generator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dag-dq-generator-1.0.1.tar", last modified: Mon May 15 20:59:52 2023, max compression
+gzip compressed data, was "dist/dag-dq-generator-1.0.2.tar", last modified: Fri May 19 18:27:44 2023, max compression
```

## Comparing `dag-dq-generator-1.0.1.tar` & `dag-dq-generator-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.600461 dag-dq-generator-1.0.1/
--rw-r--r--   0 hnankam    (501) staff       (20)      937 2023-05-13 18:11:05.000000 dag-dq-generator-1.0.1/CHANGELOG.md
--rw-r--r--   0 hnankam    (501) staff       (20)     1080 2022-08-03 15:58:08.000000 dag-dq-generator-1.0.1/LICENSE
--rw-r--r--   0 hnankam    (501) staff       (20)      133 2022-09-19 21:54:41.000000 dag-dq-generator-1.0.1/MANIFEST.in
--rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-15 20:59:52.600183 dag-dq-generator-1.0.1/PKG-INFO
--rw-r--r--   0 hnankam    (501) staff       (20)     1382 2023-05-10 03:45:14.000000 dag-dq-generator-1.0.1/README.md
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.590978 dag-dq-generator-1.0.1/dag_dq_generator/
--rw-r--r--   0 hnankam    (501) staff       (20)       74 2022-09-19 21:34:24.000000 dag-dq-generator-1.0.1/dag_dq_generator/__init__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.594882 dag-dq-generator-1.0.1/dag_dq_generator/__pycache__/
--rw-r--r--   0 hnankam    (501) staff       (20)      226 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.1/dag_dq_generator/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 hnankam    (501) staff       (20)      154 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.1/dag_dq_generator/__pycache__/__version__.cpython-38.pyc
--rw-r--r--   0 hnankam    (501) staff       (20)       90 2023-05-13 17:37:59.000000 dag-dq-generator-1.0.1/dag_dq_generator/__version__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.596129 dag-dq-generator-1.0.1/dag_dq_generator/configs/
--rw-r--r--   0 hnankam    (501) staff       (20)     6537 2022-11-09 02:56:39.000000 dag-dq-generator-1.0.1/dag_dq_generator/configs/sample.yml
--rw-r--r--   0 hnankam    (501) staff       (20)     3383 2022-11-04 20:33:28.000000 dag-dq-generator-1.0.1/dag_dq_generator/configs/stage_sample.yml
--rw-r--r--   0 hnankam    (501) staff       (20)    11149 2023-05-12 18:41:55.000000 dag-dq-generator-1.0.1/dag_dq_generator/dag_generator.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.597300 dag-dq-generator-1.0.1/dag_dq_generator/dags/
--rw-r--r--   0 hnankam    (501) staff       (20)    16788 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.1/dag_dq_generator/dags/demo-dev-01.py
--rw-r--r--   0 hnankam    (501) staff       (20)     8727 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.1/dag_dq_generator/dags/stage_test_001.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.599242 dag-dq-generator-1.0.1/dag_dq_generator/templates/
--rw-r--r--   0 hnankam    (501) staff       (20)     6955 2023-05-13 17:48:19.000000 dag-dq-generator-1.0.1/dag_dq_generator/templates/_global_macros.py
--rw-r--r--   0 hnankam    (501) staff       (20)    17751 2023-05-13 00:41:39.000000 dag-dq-generator-1.0.1/dag_dq_generator/templates/dag_template.py
--rw-r--r--   0 hnankam    (501) staff       (20)    16800 2023-05-09 23:28:44.000000 dag-dq-generator-1.0.1/dag_dq_generator/templates/dq_sql_template.sql
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.599861 dag-dq-generator-1.0.1/dag_dq_generator/tests/
--rw-r--r--   0 hnankam    (501) staff       (20)        0 2022-09-19 18:15:00.000000 dag-dq-generator-1.0.1/dag_dq_generator/tests/__init__.py
-drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-15 20:59:52.594119 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/
--rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-15 20:59:52.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/PKG-INFO
--rw-r--r--   0 hnankam    (501) staff       (20)      878 2023-05-15 20:59:52.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/SOURCES.txt
--rw-r--r--   0 hnankam    (501) staff       (20)        1 2023-05-15 20:59:52.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/dependency_links.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       71 2023-05-15 20:59:52.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/entry_points.txt
--rw-r--r--   0 hnankam    (501) staff       (20)        1 2022-09-20 16:35:26.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/not-zip-safe
--rw-r--r--   0 hnankam    (501) staff       (20)      125 2023-05-15 20:59:52.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/requires.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       17 2023-05-15 20:59:52.000000 dag-dq-generator-1.0.1/dag_dq_generator.egg-info/top_level.txt
--rw-r--r--   0 hnankam    (501) staff       (20)      124 2023-05-13 17:36:49.000000 dag-dq-generator-1.0.1/requirements.txt
--rw-r--r--   0 hnankam    (501) staff       (20)       38 2023-05-15 20:59:52.600548 dag-dq-generator-1.0.1/setup.cfg
--rw-r--r--   0 hnankam    (501) staff       (20)     1632 2023-05-15 20:59:43.000000 dag-dq-generator-1.0.1/setup.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.499572 dag-dq-generator-1.0.2/
+-rw-r--r--   0 hnankam    (501) staff       (20)     1790 2023-05-19 18:23:03.000000 dag-dq-generator-1.0.2/CHANGELOG.md
+-rw-r--r--   0 hnankam    (501) staff       (20)     1080 2022-08-03 15:58:08.000000 dag-dq-generator-1.0.2/LICENSE
+-rw-r--r--   0 hnankam    (501) staff       (20)      133 2022-09-19 21:54:41.000000 dag-dq-generator-1.0.2/MANIFEST.in
+-rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-19 18:27:44.498938 dag-dq-generator-1.0.2/PKG-INFO
+-rw-r--r--   0 hnankam    (501) staff       (20)     1382 2023-05-10 03:45:14.000000 dag-dq-generator-1.0.2/README.md
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.480163 dag-dq-generator-1.0.2/dag_dq_generator/
+-rw-r--r--   0 hnankam    (501) staff       (20)       74 2022-09-19 21:34:24.000000 dag-dq-generator-1.0.2/dag_dq_generator/__init__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.485912 dag-dq-generator-1.0.2/dag_dq_generator/__pycache__/
+-rw-r--r--   0 hnankam    (501) staff       (20)      226 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.2/dag_dq_generator/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 hnankam    (501) staff       (20)      154 2022-09-21 21:25:09.000000 dag-dq-generator-1.0.2/dag_dq_generator/__pycache__/__version__.cpython-38.pyc
+-rw-r--r--   0 hnankam    (501) staff       (20)       90 2023-05-19 16:59:44.000000 dag-dq-generator-1.0.2/dag_dq_generator/__version__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.488755 dag-dq-generator-1.0.2/dag_dq_generator/configs/
+-rw-r--r--   0 hnankam    (501) staff       (20)     6537 2022-11-09 02:56:39.000000 dag-dq-generator-1.0.2/dag_dq_generator/configs/sample.yml
+-rw-r--r--   0 hnankam    (501) staff       (20)     3383 2022-11-04 20:33:28.000000 dag-dq-generator-1.0.2/dag_dq_generator/configs/stage_sample.yml
+-rw-r--r--   0 hnankam    (501) staff       (20)    11149 2023-05-12 18:41:55.000000 dag-dq-generator-1.0.2/dag_dq_generator/dag_generator.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.491365 dag-dq-generator-1.0.2/dag_dq_generator/dags/
+-rw-r--r--   0 hnankam    (501) staff       (20)    16788 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.2/dag_dq_generator/dags/demo-dev-01.py
+-rw-r--r--   0 hnankam    (501) staff       (20)     8727 2022-09-19 18:50:06.000000 dag-dq-generator-1.0.2/dag_dq_generator/dags/stage_test_001.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.496123 dag-dq-generator-1.0.2/dag_dq_generator/templates/
+-rw-r--r--   0 hnankam    (501) staff       (20)     7482 2023-05-17 22:52:00.000000 dag-dq-generator-1.0.2/dag_dq_generator/templates/_global_macros.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    17900 2023-05-17 22:49:36.000000 dag-dq-generator-1.0.2/dag_dq_generator/templates/dag_template.py
+-rw-r--r--   0 hnankam    (501) staff       (20)    16800 2023-05-09 23:28:44.000000 dag-dq-generator-1.0.2/dag_dq_generator/templates/dq_sql_template.sql
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.498269 dag-dq-generator-1.0.2/dag_dq_generator/tests/
+-rw-r--r--   0 hnankam    (501) staff       (20)        0 2022-09-19 18:15:00.000000 dag-dq-generator-1.0.2/dag_dq_generator/tests/__init__.py
+drwxr-xr-x   0 hnankam    (501) staff       (20)        0 2023-05-19 18:27:44.484387 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/
+-rw-r--r--   0 hnankam    (501) staff       (20)     2292 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/PKG-INFO
+-rw-r--r--   0 hnankam    (501) staff       (20)      878 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)        1 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       71 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/entry_points.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)        1 2022-09-20 16:35:26.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/not-zip-safe
+-rw-r--r--   0 hnankam    (501) staff       (20)      125 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/requires.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       17 2023-05-19 18:27:44.000000 dag-dq-generator-1.0.2/dag_dq_generator.egg-info/top_level.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)      124 2023-05-13 17:36:49.000000 dag-dq-generator-1.0.2/requirements.txt
+-rw-r--r--   0 hnankam    (501) staff       (20)       38 2023-05-19 18:27:44.499818 dag-dq-generator-1.0.2/setup.cfg
+-rw-r--r--   0 hnankam    (501) staff       (20)     1632 2023-05-17 22:52:05.000000 dag-dq-generator-1.0.2/setup.py
```

### Comparing `dag-dq-generator-1.0.1/CHANGELOG.md` & `dag-dq-generator-1.0.2/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.0.2] - 2023-05-19
+
+### Major changes
+- Enabled pip integration with Adobe Artifactory and PyPI. dag-generator can now be installed using `pip install dag-dq-generator`. Please visit the [documentation](https://wiki.corp.adobe.com/pages/viewpage.action?pageId=2849653154#Implementation&Use-Setup&Installation) for more information
+
+### New features
+- Feature: Added support for `TableauOperator` for connecting to Tableau for data refresh. Please visit the [documentation](https://wiki.corp.adobe.com/pages/viewpage.action?pageId=2849653154#Implementation&Use-TableauOperator) for more information
+- Feature: Added support for `TableauJobStatusSensor`, a sensor for TableauOperator. Please visit the [documentation](https://wiki.corp.adobe.com/pages/viewpage.action?pageId=2849653154#Implementation&Use-TableauJobStatusSensor) for more information
+
 ## [1.0.1] - 2023-05-13
 
 ### Major changes
 - Updated `black` from `22.6.0` to `23.3.0`
 - Updated `apache-airflow-providers-databricks` from `3.1.0` to `4.1.0`
 
 ### Changed features
-
 - Feature: Added support for `SubGroupOperator` which enables the creation of subgroups in the DAG, theoritically allowing for infinite nesting of DAGs. Please visit the [documentation](https://wiki.corp.adobe.com/pages/viewpage.action?pageId=2849653154#Implementation&Use-SubGroupOperator) for more information
 - Fix: N/A
 
 ## [1.0.0] - 2023-05-02
 
 We're super excited to announce the release of v1.0 of the `dag-generator`!
```

### Comparing `dag-dq-generator-1.0.1/LICENSE` & `dag-dq-generator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/PKG-INFO` & `dag-dq-generator-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dag-dq-generator
-Version: 1.0.1
+Version: 1.0.2
 Summary: DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator
 Home-page: https://git.corp.adobe.com/ccea/dag-dq-generator
 Author: CI DMe Data Engineering
 Author-email: ccea-data-engineering@adobe.com
 License: MIT
 Description: # dag-dq-generator
         DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator.
```

### Comparing `dag-dq-generator-1.0.1/README.md` & `dag-dq-generator-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/configs/sample.yml` & `dag-dq-generator-1.0.2/dag_dq_generator/configs/sample.yml`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/configs/stage_sample.yml` & `dag-dq-generator-1.0.2/dag_dq_generator/configs/stage_sample.yml`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/dag_generator.py` & `dag-dq-generator-1.0.2/dag_dq_generator/dag_generator.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/dags/demo-dev-01.py` & `dag-dq-generator-1.0.2/dag_dq_generator/dags/demo-dev-01.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/dags/stage_test_001.py` & `dag-dq-generator-1.0.2/dag_dq_generator/dags/stage_test_001.py`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/templates/_global_macros.py` & `dag-dq-generator-1.0.2/dag_dq_generator/templates/_global_macros.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,30 @@
 
     {{task.task_id}} = TriggerDagRunOperator(
         task_id='{{task.task_id}}',
         on_success_callback=_task_on_success_callback,
         **{{task.task_id}}_args
     )
 
+    {% elif task.operator == 'TableauOperator' %} # Generate TableauOperator task
+
+    {{task.task_id}} = TableauOperator(
+        task_id='{{task.task_id}}',
+        on_success_callback=_task_on_success_callback,
+        **{{task.task_id}}_args
+    )
+
+    {% elif task.operator == 'TableauJobStatusSensor' %} # Generate TableauJobStatusSensor task
+
+    {{task.task_id}} = TableauJobStatusSensor(
+        task_id='{{task.task_id}}',
+        on_success_callback=_task_on_success_callback,
+        **{{task.task_id}}_args
+    )
+
     {% elif task.operator == 'DateTimeSensor' %} # Generate DateTimeSensor task
     
     {{task.task_id}}_args['target_time'] = eval({{task.task_id}}_args['target_time'])
 
     {{task.task_id}} = DateTimeSensor(
         task_id='{{task.task_id}}',
         on_success_callback=_task_on_success_callback,
```

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/templates/dag_template.py` & `dag-dq-generator-1.0.2/dag_dq_generator/templates/dag_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 # Airflow Imports
 from airflow import DAG, settings
 from airflow.providers.databricks.hooks.databricks_sql import DatabricksSqlHook
 from airflow.providers.databricks.operators.databricks import DatabricksSubmitRunOperator, DatabricksRunNowOperator
 from airflow.providers.databricks.operators.databricks_sql import DatabricksSqlOperator
 from airflow.operators.trigger_dagrun import TriggerDagRunOperator
+from airflow.providers.tableau.operators.tableau import TableauOperator
+from airflow.providers.tableau.sensors.tableau import TableauJobStatusSensor
 from airflow.models import Variable, TaskInstance, XCom
 from airflow.utils.dates import days_ago
 from airflow.utils.task_group import TaskGroup # Used to group tasks together in the Graph view of the Airflow UI
 from airflow.operators.dummy_operator import DummyOperator
 from airflow.operators.email import EmailOperator
 from airflow.utils.email import send_email
 from airflow.operators.python import PythonOperator, ShortCircuitOperator
```

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator/templates/dq_sql_template.sql` & `dag-dq-generator-1.0.2/dag_dq_generator/templates/dq_sql_template.sql`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator.egg-info/PKG-INFO` & `dag-dq-generator-1.0.2/dag_dq_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dag-dq-generator
-Version: 1.0.1
+Version: 1.0.2
 Summary: DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator
 Home-page: https://git.corp.adobe.com/ccea/dag-dq-generator
 Author: CI DMe Data Engineering
 Author-email: ccea-data-engineering@adobe.com
 License: MIT
 Description: # dag-dq-generator
         DPaaS Airflow DAG (Dynamic Acyclic Graph) and DQ (Data Quality) generator.
```

### Comparing `dag-dq-generator-1.0.1/dag_dq_generator.egg-info/SOURCES.txt` & `dag-dq-generator-1.0.2/dag_dq_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dag-dq-generator-1.0.1/setup.py` & `dag-dq-generator-1.0.2/setup.py`

 * *Files identical despite different names*

