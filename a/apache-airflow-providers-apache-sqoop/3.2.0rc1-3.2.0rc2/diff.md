# Comparing `tmp/apache-airflow-providers-apache-sqoop-3.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-apache-sqoop-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-apache-sqoop-3.2.0rc1.tar", last modified: Tue May 16 15:53:18 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-apache-sqoop-3.2.0rc2.tar", last modified: Fri May 19 17:51:55 2023, max compression
```

## Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1.tar` & `apache-airflow-providers-apache-sqoop-3.2.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10172 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8627 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/
--rw-r--r--   0 root         (0) root         (0)     1395 2023-05-16 15:39:21.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2594 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15813 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11404 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10172 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-16 15:53:18.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-05-16 15:53:17.000000 apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10389 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8844 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-05-19 12:03:00.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15813 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11404 2023-02-24 18:43:53.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10389 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-05-19 17:51:55.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-05-19 17:51:54.000000 apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/LICENSE` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/MANIFEST.in` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -124,14 +124,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 * ``Move libjars parameter in Sqoop Hook to Hook parameter (#29500)``
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/README.rst` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -91,14 +91,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 * ``Move libjars parameter in Sqoop Hook to Hook parameter (#29500)``
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/__init__.py`

 * *Files 10% similar despite different names*

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
-        f"The package `apache-airflow-providers-apache-sqoop:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-apache-sqoop:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/get_provider_info.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/hooks/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/hooks/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/airflow/providers/apache/sqoop/operators/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/airflow/providers/apache/sqoop/operators/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
@@ -124,14 +124,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 * ``Move libjars parameter in Sqoop Hook to Hook parameter (#29500)``
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/pyproject.toml` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.cfg` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.sqoop.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.sqoop
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.0rc1/setup.py` & `apache-airflow-providers-apache-sqoop-3.2.0rc2/setup.py`

 * *Files identical despite different names*

