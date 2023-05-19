# Comparing `tmp/apache-airflow-providers-ftp-3.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-ftp-3.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.0rc1.tar", last modified: Tue May 16 15:53:50 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-ftp-3.4.0rc2.tar", last modified: Fri May 19 17:52:25 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.4.0rc1.tar` & `apache-airflow-providers-ftp-3.4.0rc2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-ftp-3.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:53:49.000000 apache-airflow-providers-ftp-3.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-ftp-3.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9387 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7869 2023-05-16 15:53:49.000000 apache-airflow-providers-ftp-3.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1372 2023-05-16 15:39:21.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-05-16 15:53:49.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9842 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6093 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9387 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-ftp-3.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1782 2023-05-16 15:53:50.000000 apache-airflow-providers-ftp-3.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-16 15:53:49.000000 apache-airflow-providers-ftp-3.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-ftp-3.4.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-ftp-3.4.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9604 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8086 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-05-19 12:06:30.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9842 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6093 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-02-24 18:43:53.000000 apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9604 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      699 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-ftp-3.4.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-05-19 17:52:25.000000 apache-airflow-providers-ftp-3.4.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-19 17:52:24.000000 apache-airflow-providers-ftp-3.4.0rc2/setup.py
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/LICENSE` & `apache-airflow-providers-ftp-3.4.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/MANIFEST.in` & `apache-airflow-providers-ftp-3.4.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/PKG-INFO` & `apache-airflow-providers-ftp-3.4.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.0rc1
+Version: 3.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
@@ -110,14 +110,17 @@
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/README.rst` & `apache-airflow-providers-ftp-3.4.0rc2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
@@ -77,14 +77,17 @@
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.4.0rc2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,26 +11,39 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-#
+
 # NOTE! THIS FILE IS AUTOMATICALLY GENERATED AND WILL BE
-# OVERWRITTEN WHEN PREPARING DOCUMENTATION FOR THE PACKAGES.
+# OVERWRITTEN WHEN PREPARING PACKAGES.
 #
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
-# `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
-#
-from __future__ import annotations
-
-import packaging.version
+# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
-import airflow
+"""Setup.py for the apache-airflow-providers-ftp package."""
 
-__all__ = ["version"]
+from setuptools import find_namespace_packages, setup
 
 version = "3.4.0"
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
-    raise RuntimeError(f"The package `apache-airflow-providers-ftp:{version}` requires Apache Airflow 2.4.0+")
+
+def do_setup():
+    """Perform the package apache-airflow-providers-ftp setup."""
+    setup(
+        version=version,
+        extras_require={},
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.ftp",
+                "airflow.providers.ftp.*",
+                "airflow.providers.ftp_vendor",
+                "airflow.providers.ftp_vendor.*",
+            ],
+        ),
+    )
+
+
+if __name__ == "__main__":
+    do_setup()
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/hooks/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/operators/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.4.0rc2/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO` & `apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.0rc1
+Version: 3.4.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.0rc1``
+Release: ``3.4.0rc2``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
@@ -110,14 +110,17 @@
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.3.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.4.0rc2/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/pyproject.toml` & `apache-airflow-providers-ftp-3.4.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-ftp-3.4.0rc1/setup.cfg` & `apache-airflow-providers-ftp-3.4.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -51,10 +51,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.ftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.ftp
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

