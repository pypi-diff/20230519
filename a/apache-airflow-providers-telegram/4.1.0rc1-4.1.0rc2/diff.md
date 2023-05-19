# Comparing `tmp/apache-airflow-providers-telegram-4.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-telegram-4.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-telegram-4.1.0rc1.tar", last modified: Tue May 16 15:55:27 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-telegram-4.1.0rc2.tar", last modified: Fri May 19 17:53:44 2023, max compression
```

## Comparing `apache-airflow-providers-telegram-4.1.0rc1.tar` & `apache-airflow-providers-telegram-4.1.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-telegram-4.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:26.000000 apache-airflow-providers-telegram-4.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-telegram-4.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10448 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8915 2023-05-16 15:55:26.000000 apache-airflow-providers-telegram-4.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/
--rw-r--r--   0 root         (0) root         (0)     1391 2023-05-16 15:39:21.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-16 15:55:26.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/hooks/telegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/operators/telegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10448 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-telegram-4.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-16 15:55:27.000000 apache-airflow-providers-telegram-4.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-16 15:55:26.000000 apache-airflow-providers-telegram-4.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-telegram-4.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-telegram-4.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10665 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:22:43.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/telegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-02-24 18:43:53.000000 apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/telegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10665 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-telegram-4.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-05-19 17:53:44.000000 apache-airflow-providers-telegram-4.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 17:53:43.000000 apache-airflow-providers-telegram-4.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/LICENSE` & `apache-airflow-providers-telegram-4.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/MANIFEST.in` & `apache-airflow-providers-telegram-4.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/PKG-INFO` & `apache-airflow-providers-telegram-4.1.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.1.0rc1
+Version: 4.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-telegram package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.0rc1``
+Release: ``4.1.0rc2``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
@@ -125,14 +125,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/README.rst` & `apache-airflow-providers-telegram-4.1.0rc2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.0rc1``
+Release: ``4.1.0rc2``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
@@ -92,14 +92,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/__init__.py` & `apache-airflow-providers-telegram-4.1.0rc2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,28 +11,39 @@
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
+"""Setup.py for the apache-airflow-providers-telegram package."""
 
-__all__ = ["version"]
+from setuptools import find_namespace_packages, setup
 
 version = "4.1.0"
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
-    raise RuntimeError(
-        f"The package `apache-airflow-providers-telegram:{version}` requires Apache Airflow 2.4.0+"
+
+def do_setup():
+    """Perform the package apache-airflow-providers-telegram setup."""
+    setup(
+        version=version,
+        extras_require={},
+        packages=find_namespace_packages(
+            include=[
+                "airflow.providers.telegram",
+                "airflow.providers.telegram.*",
+                "airflow.providers.telegram_vendor",
+                "airflow.providers.telegram_vendor.*",
+            ],
+        ),
     )
+
+
+if __name__ == "__main__":
+    do_setup()
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/get_provider_info.py` & `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/hooks/__init__.py` & `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/hooks/telegram.py` & `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/hooks/telegram.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/operators/__init__.py` & `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/airflow/providers/telegram/operators/telegram.py` & `apache-airflow-providers-telegram-4.1.0rc2/airflow/providers/telegram/operators/telegram.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/PKG-INFO` & `apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.1.0rc1
+Version: 4.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-telegram package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.0rc1``
+Release: ``4.1.0rc2``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
@@ -125,14 +125,17 @@
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 4.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
```

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/apache_airflow_providers_telegram.egg-info/SOURCES.txt` & `apache-airflow-providers-telegram-4.1.0rc2/apache_airflow_providers_telegram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/pyproject.toml` & `apache-airflow-providers-telegram-4.1.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-telegram-4.1.0rc1/setup.cfg` & `apache-airflow-providers-telegram-4.1.0rc2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.telegram.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.telegram
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

