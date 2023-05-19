# Comparing `tmp/apache-airflow-providers-microsoft-psrp-2.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-microsoft-psrp-2.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-microsoft-psrp-2.3.0rc1.tar", last modified: Tue May 16 15:54:35 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-microsoft-psrp-2.3.0rc2.tar", last modified: Fri May 19 17:52:53 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1.tar` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8811 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7260 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/
--rw-r--r--   0 root         (0) root         (0)     1397 2023-05-16 15:39:21.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10850 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/psrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/psrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8811 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-16 15:54:35.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1686 2023-05-16 15:54:34.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:52.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7477 2023-05-19 17:52:52.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-19 12:13:47.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-05-19 17:52:52.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-05-03 19:47:07.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/hooks/psrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-02-24 18:43:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/operators/psrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-19 17:52:53.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-05-19 17:52:52.000000 apache-airflow-providers-microsoft-psrp-2.3.0rc2/setup.py
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/LICENSE` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/MANIFEST.in` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/PKG-INFO` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.3.0rc1
+Version: 2.3.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-psrp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.3.0rc1``
+Release: ``2.3.0rc2``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
 
 
@@ -132,14 +132,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Upgrade Mypy to 1.0 (#29468)``
    * ``Revert "Upgrade mypy to 0.991 (#28926)" (#29470)``
    * ``Upgrade mypy to 0.991 (#28926)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 2.2.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/README.rst` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.3.0rc1``
+Release: ``2.3.0rc2``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
 
 
@@ -99,14 +99,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Upgrade Mypy to 1.0 (#29468)``
    * ``Revert "Upgrade mypy to 0.991 (#28926)" (#29470)``
    * ``Upgrade mypy to 0.991 (#28926)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 2.2.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/__init__.py`

 * *Files 11% similar despite different names*

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
+__version__ = "2.3.0"
 
-version = "2.3.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-microsoft-psrp:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-microsoft-psrp:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/get_provider_info.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/hooks/psrp.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/hooks/psrp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/airflow/providers/microsoft/psrp/operators/psrp.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/airflow/providers/microsoft/psrp/operators/psrp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.3.0rc1
+Version: 2.3.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-psrp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.3.0rc1``
+Release: ``2.3.0rc2``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
 
 
@@ -132,14 +132,17 @@
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Upgrade Mypy to 1.0 (#29468)``
    * ``Revert "Upgrade mypy to 0.991 (#28926)" (#29470)``
    * ``Upgrade mypy to 0.991 (#28926)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 2.2.0
 .....
 
 Features
 ~~~~~~~~
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/pyproject.toml` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.cfg` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.psrp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.psrp
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.0rc1/setup.py` & `apache-airflow-providers-microsoft-psrp-2.3.0rc2/setup.py`

 * *Files identical despite different names*

