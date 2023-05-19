# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.2.0rc1.tar", last modified: Tue May 16 15:53:37 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-dbt-cloud-3.2.0rc2.tar", last modified: Fri May 19 17:52:13 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1.tar` & `apache-airflow-providers-dbt-cloud-3.2.0rc2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10938 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9381 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)     1392 2023-05-16 15:39:21.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13638 2023-05-16 07:40:59.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5508 2023-05-03 19:47:07.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4839 2023-04-24 21:04:25.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10938 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1895 2023-05-16 15:53:37.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-05-16 15:53:36.000000 apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11230 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9673 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-05-19 12:05:02.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24269 2023-03-10 19:31:58.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13638 2023-05-16 07:40:59.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-05-03 19:47:07.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2023-04-24 21:04:25.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11230 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-05-19 17:52:13.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-05-19 17:52:12.000000 apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/LICENSE` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
@@ -143,21 +143,25 @@
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 * ``Optimize deferred execution mode in DbtCloudJobRunSensor (#30968)``
+* ``Optimize deferred execution mode for DbtCloudRunJobOperator (#31188)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.1
 .....
 
 Misc
 ~~~~
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/README.rst` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
@@ -109,21 +109,25 @@
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 * ``Optimize deferred execution mode in DbtCloudJobRunSensor (#30968)``
+* ``Optimize deferred execution mode for DbtCloudRunJobOperator (#31188)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.1
 .....
 
 Misc
 ~~~~
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/__init__.py`

 * *Files 12% similar despite different names*

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
+__version__ = "3.2.0"
 
-version = "3.2.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-dbt-cloud:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-dbt-cloud:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
@@ -143,21 +143,25 @@
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 * ``Optimize deferred execution mode in DbtCloudJobRunSensor (#30968)``
+* ``Optimize deferred execution mode for DbtCloudRunJobOperator (#31188)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add cli cmd to list the provider trigger info (#30822)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.1
 .....
 
 Misc
 ~~~~
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dbt.cloud
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.0rc1/setup.py` & `apache-airflow-providers-dbt-cloud-3.2.0rc2/setup.py`

 * *Files identical despite different names*

