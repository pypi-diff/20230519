# Comparing `tmp/apache-airflow-providers-asana-2.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-asana-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-asana-2.2.0rc2.tar", last modified: Fri May 19 17:51:58 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-asana-3.0.0rc1.tar", last modified: Tue Nov 15 00:14:08 2022, max compression
```

## Comparing `apache-airflow-providers-asana-2.2.0rc2.tar` & `apache-airflow-providers-asana-3.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-asana-2.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:51:57.000000 apache-airflow-providers-asana-2.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-asana-2.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10056 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8532 2023-05-19 17:51:57.000000 apache-airflow-providers-asana-2.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-05-19 12:03:36.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-05-19 17:51:57.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13369 2023-02-24 18:43:53.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/hooks/asana.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5417 2023-02-24 18:43:53.000000 apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/operators/asana_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10056 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-asana-2.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1835 2023-05-19 17:51:58.000000 apache-airflow-providers-asana-2.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-05-19 17:51:57.000000 apache-airflow-providers-asana-2.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7480 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13369 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2022-09-14 19:22:24.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1832 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1460 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/LICENSE` & `apache-airflow-providers-asana-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.0rc2/MANIFEST.in` & `apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.rst
+include CHANGELOG.txt
+include README.md
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/PKG-INFO` & `apache-airflow-providers-asana-3.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-asana
-Version: 2.2.0rc2
+Version: 3.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-asana package
 Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.0/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -48,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-asana``
 
-Release: ``2.2.0rc2``
+Release: ``3.0.0rc1``
 
 
 `Asana <https://app.asana.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``asana`` provider. All classes for this provider package
 are in ``airflow.providers.asana`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +80,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.4.0``
+``apache-airflow``  ``>=2.3.0``
 ``asana``           ``>=0.10``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -108,62 +109,42 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-2.2.0
+3.0.0
 .....
 
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
-
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+This release of provider is only available for Airflow 2.3+ as explained in the
+`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
 
-2.1.0
-.....
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.3+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* In AsanaHook, non-prefixed extra fields are supported and are preferred.  So if you should update your
+  connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-In AsanaHook, non-prefixed extra fields are supported and are preferred. You should update your
-connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
-
-
 * ``Allow and prefer non-prefixed extra fields for AsanaHook (#27043)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Enable string normalization in python formatting - providers (#27205)``
    * ``Update docs for September Provider's release (#26731)``
    * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
-   * ``pRepare docs for November 2022 wave of Providers (#27613)``
-   * ``Prepare for follow-up release for November providers (#27774)``
+
 
 2.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
@@ -176,17 +157,16 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.2+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
+  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate Asana example DAGs to new design #22440 (#24131)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Use new Breese for building, pulling and verifying the images. (#23104)``
@@ -260,7 +240,9 @@
    * ``Prepare documentation for July release of providers. (#17015)``
    * ``Removes pylint from our toolchain (#16682)``
 
 1.0.0
 .....
 
 Initial version of the provider.
+
+
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/README.rst` & `apache-airflow-providers-asana-3.0.0rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-asana``
 
-Release: ``2.2.0rc2``
+Release: ``3.0.0rc1``
 
 
 `Asana <https://app.asana.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``asana`` provider. All classes for this provider package
 are in ``airflow.providers.asana`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -46,15 +46,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.4.0``
+``apache-airflow``  ``>=2.3.0``
 ``asana``           ``>=0.10``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -75,62 +75,42 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-2.2.0
+3.0.0
 .....
 
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+This release of provider is only available for Airflow 2.3+ as explained in the
+`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
 
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
-
-2.1.0
-.....
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.3+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* In AsanaHook, non-prefixed extra fields are supported and are preferred.  So if you should update your
+  connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-In AsanaHook, non-prefixed extra fields are supported and are preferred. You should update your
-connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
-
-
 * ``Allow and prefer non-prefixed extra fields for AsanaHook (#27043)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Enable string normalization in python formatting - providers (#27205)``
    * ``Update docs for September Provider's release (#26731)``
    * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
-   * ``pRepare docs for November 2022 wave of Providers (#27613)``
-   * ``Prepare for follow-up release for November providers (#27774)``
+
 
 2.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
@@ -143,17 +123,16 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.2+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
+  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate Asana example DAGs to new design #22440 (#24131)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Use new Breese for building, pulling and verifying the images. (#23104)``
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,31 +11,32 @@
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
+# `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
-import packaging.version
+"""Setup.py for the apache-airflow-providers-asana package."""
 
-__all__ = ["__version__"]
+from setuptools import find_namespace_packages, setup
 
-__version__ = "2.2.0"
+version = "3.0.0"
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
-    raise RuntimeError(
-        f"The package `apache-airflow-providers-asana:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
+def do_setup():
+    """Perform the package apache-airflow-providers-asana setup."""
+    setup(
+        version=version,
+        extras_require={},
+        packages=find_namespace_packages(include=["airflow.providers.asana", "airflow.providers.asana.*"]),
     )
+
+
+if __name__ == "__main__":
+    do_setup()
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/get_provider_info.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,16 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-asana",
         "name": "Asana",
         "description": "`Asana <https://app.asana.com/>`__\n",
-        "suspended": False,
-        "versions": ["2.2.0", "2.1.0", "2.0.1", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
-        "dependencies": ["apache-airflow>=2.4.0", "asana>=0.10"],
+        "versions": ["3.0.0", "2.0.1", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.3.0", "asana>=0.10"],
         "integrations": [
             {
                 "integration-name": "Asana",
                 "external-doc-url": "https://developers.asana.com/docs",
                 "how-to-guide": ["/docs/apache-airflow-providers-asana/operators/asana.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/hooks/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/hooks/asana.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/operators/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.0rc2/airflow/providers/asana/operators/asana_tasks.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/PKG-INFO` & `apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-asana
-Version: 2.2.0rc2
+Version: 3.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-asana package
 Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.0/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -48,28 +49,28 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-asana``
 
-Release: ``2.2.0rc2``
+Release: ``3.0.0rc1``
 
 
 `Asana <https://app.asana.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``asana`` provider. All classes for this provider package
 are in ``airflow.providers.asana`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -79,15 +80,15 @@
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.4.0``
+``apache-airflow``  ``>=2.3.0``
 ``asana``           ``>=0.10``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -108,62 +109,42 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-2.2.0
+3.0.0
 .....
 
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
-
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
+This release of provider is only available for Airflow 2.3+ as explained in the
+`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
 
-2.1.0
-.....
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.3+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* In AsanaHook, non-prefixed extra fields are supported and are preferred.  So if you should update your
+  connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-In AsanaHook, non-prefixed extra fields are supported and are preferred. You should update your
-connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
-
-
 * ``Allow and prefer non-prefixed extra fields for AsanaHook (#27043)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Enable string normalization in python formatting - providers (#27205)``
    * ``Update docs for September Provider's release (#26731)``
    * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
-   * ``pRepare docs for November 2022 wave of Providers (#27613)``
-   * ``Prepare for follow-up release for November providers (#27774)``
+
 
 2.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
@@ -176,17 +157,16 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.2+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
+  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate Asana example DAGs to new design #22440 (#24131)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Use new Breese for building, pulling and verifying the images. (#23104)``
@@ -260,7 +240,9 @@
    * ``Prepare documentation for July release of providers. (#17015)``
    * ``Removes pylint from our toolchain (#16682)``
 
 1.0.0
 .....
 
 Initial version of the provider.
+
+
```

### Comparing `apache-airflow-providers-asana-2.2.0rc2/apache_airflow_providers_asana.egg-info/SOURCES.txt` & `apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.0rc2/setup.cfg` & `apache-airflow-providers-asana-3.0.0rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -42,21 +42,21 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0.dev0
+	apache-airflow>=2.3.0.*
 	asana>=0.10
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.asana.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.asana
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

