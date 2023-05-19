# Comparing `tmp/apache-airflow-providers-snowflake-4.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.1.0rc1.tar", last modified: Tue May 16 15:55:18 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-snowflake-4.1.0rc2.tar", last modified: Fri May 19 17:53:35 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.1.0rc1.tar` & `apache-airflow-providers-snowflake-4.1.0rc2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:17.000000 apache-airflow-providers-snowflake-4.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    18989 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17404 2023-05-16 15:55:17.000000 apache-airflow-providers-snowflake-4.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1392 2023-05-16 15:39:21.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4589 2023-05-16 15:55:17.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17835 2023-04-30 16:55:41.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/hooks/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6053 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/utils/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18989 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1079 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-snowflake-4.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-16 15:55:18.000000 apache-airflow-providers-snowflake-4.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-05-16 15:55:17.000000 apache-airflow-providers-snowflake-4.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-snowflake-4.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    19277 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17692 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-05-19 12:21:57.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4589 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17835 2023-04-30 16:55:41.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6053 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-05-03 19:47:07.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-02-24 18:43:53.000000 apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19277 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-snowflake-4.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-19 17:53:35.000000 apache-airflow-providers-snowflake-4.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-05-19 17:53:34.000000 apache-airflow-providers-snowflake-4.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/LICENSE` & `apache-airflow-providers-snowflake-4.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/MANIFEST.in` & `apache-airflow-providers-snowflake-4.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/PKG-INFO` & `apache-airflow-providers-snowflake-4.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.1.0rc1
+Version: 4.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.1.0rc1``
+Release: ``4.1.0rc2``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
@@ -148,14 +148,18 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
 
 4.0.5
 .....
 
 Misc
 ~~~~
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/README.rst` & `apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,42 @@
+Metadata-Version: 2.1
+Name: apache-airflow-providers-snowflake
+Version: 4.1.0rc2
+Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
+Home-page: https://airflow.apache.org/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Author: Apache Software Foundation
+Author-email: dev@airflow.apache.org
+License: Apache License 2.0
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/
+Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
+Project-URL: Source Code, https://github.com/apache/airflow
+Project-URL: Slack Chat, https://s.apache.org/airflow-slack
+Project-URL: Twitter, https://twitter.com/ApacheAirflow
+Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: Framework :: Apache Airflow
+Classifier: Framework :: Apache Airflow :: Provider
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Monitoring
+Requires-Python: ~=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: common.sql
+Provides-Extra: slack
+License-File: LICENSE
+License-File: NOTICE
+
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -15,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.1.0rc1``
+Release: ``4.1.0rc2``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
@@ -113,14 +148,18 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
 
 4.0.5
 .....
 
 Misc
 ~~~~
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/__init__.py`

 * *Files 17% similar despite different names*

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
+__version__ = "4.1.0"
 
-version = "4.1.0"
+try:
+    from airflow import __version__ as airflow_version
+except ImportError:
+    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow.version.version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
     raise RuntimeError(
-        f"The package `apache-airflow-providers-snowflake:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-snowflake:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.1.0rc2/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.1.0rc2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,7 @@
-Metadata-Version: 2.1
-Name: apache-airflow-providers-snowflake
-Version: 4.1.0rc1
-Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
-Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
-Author: Apache Software Foundation
-Author-email: dev@airflow.apache.org
-License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.1.0/
-Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Source Code, https://github.com/apache/airflow
-Project-URL: Slack Chat, https://s.apache.org/airflow-slack
-Project-URL: Twitter, https://twitter.com/ApacheAirflow
-Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators
-Classifier: Framework :: Apache Airflow
-Classifier: Framework :: Apache Airflow :: Provider
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: common.sql
-Provides-Extra: slack
-License-File: LICENSE
-License-File: NOTICE
-
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
@@ -50,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.1.0rc1``
+Release: ``4.1.0rc2``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
@@ -148,14 +113,18 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+   * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
 
 4.0.5
 .....
 
 Misc
 ~~~~
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.1.0rc2/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/pyproject.toml` & `apache-airflow-providers-snowflake-4.1.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/setup.cfg` & `apache-airflow-providers-snowflake-4.1.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.1.0rc1/setup.py` & `apache-airflow-providers-snowflake-4.1.0rc2/setup.py`

 * *Files identical despite different names*

