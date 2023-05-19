# Comparing `tmp/apache-airflow-providers-databricks-4.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-databricks-4.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-databricks-4.2.0rc1.tar", last modified: Tue May 16 15:53:33 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-databricks-4.2.0rc2.tar", last modified: Fri May 19 17:52:09 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.2.0rc1.tar` & `apache-airflow-providers-databricks-4.2.0rc2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    20044 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18478 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)     1393 2023-05-16 15:39:21.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5547 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16761 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33394 2023-05-04 19:17:30.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    16793 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10015 2023-05-15 07:14:11.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0 root         (0) root         (0)     5558 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-04-24 21:04:25.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20044 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1362 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-databricks-4.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1981 2023-05-16 15:53:33.000000 apache-airflow-providers-databricks-4.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-05-16 15:53:32.000000 apache-airflow-providers-databricks-4.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-databricks-4.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    20261 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18695 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-05-19 12:04:45.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5547 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16761 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26704 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9278 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33394 2023-05-04 19:17:30.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13226 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    16793 2023-05-12 08:38:07.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10015 2023-05-15 07:14:11.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-04-13 08:25:21.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-04-24 21:04:25.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-02-24 18:43:53.000000 apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20261 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-databricks-4.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-05-19 17:52:09.000000 apache-airflow-providers-databricks-4.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-05-19 17:52:08.000000 apache-airflow-providers-databricks-4.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/LICENSE` & `apache-airflow-providers-databricks-4.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/MANIFEST.in` & `apache-airflow-providers-databricks-4.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/PKG-INFO` & `apache-airflow-providers-databricks-4.2.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.2.0rc1
+Version: 4.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.2.0rc1``
+Release: ``4.2.0rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
@@ -160,14 +160,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 4.1.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/README.rst` & `apache-airflow-providers-databricks-4.2.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.2.0rc1``
+Release: ``4.2.0rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
@@ -126,14 +126,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 4.1.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_partition.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.2.0rc2/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.2.0rc1
+Version: 4.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.2.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.2.0rc1``
+Release: ``4.2.0rc2``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
@@ -160,14 +160,17 @@
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Move TaskInstanceKey to a separate file (#31033)``
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 4.1.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.2.0rc2/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/pyproject.toml` & `apache-airflow-providers-databricks-4.2.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/setup.cfg` & `apache-airflow-providers-databricks-4.2.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -56,10 +56,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.databricks.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.databricks
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-databricks-4.2.0rc1/setup.py` & `apache-airflow-providers-databricks-4.2.0rc2/setup.py`

 * *Files identical despite different names*

