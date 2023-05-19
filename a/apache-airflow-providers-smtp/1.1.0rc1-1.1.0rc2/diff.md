# Comparing `tmp/apache-airflow-providers-smtp-1.1.0rc1.tar.gz` & `tmp/apache-airflow-providers-smtp-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-smtp-1.1.0rc1.tar", last modified: Tue May 16 15:55:16 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-smtp-1.1.0rc2.tar", last modified: Fri May 19 17:53:33 2023, max compression
```

## Comparing `apache-airflow-providers-smtp-1.1.0rc1.tar` & `apache-airflow-providers-smtp-1.1.0rc2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3925 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/
--rw-r--r--   0 root         (0) root         (0)     1387 2023-05-16 15:39:21.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-04-13 08:25:20.000000 apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/smtp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-smtp-1.1.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1816 2023-05-16 15:55:16.000000 apache-airflow-providers-smtp-1.1.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-16 15:55:15.000000 apache-airflow-providers-smtp-1.1.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-smtp-1.1.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:21:49.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-04-07 21:10:19.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-15 08:58:48.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-04-13 08:25:20.000000 apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/smtp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5663 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-smtp-1.1.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1816 2023-05-19 17:53:33.000000 apache-airflow-providers-smtp-1.1.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-05-19 17:53:32.000000 apache-airflow-providers-smtp-1.1.0rc2/setup.py
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/LICENSE` & `apache-airflow-providers-smtp-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/MANIFEST.in` & `apache-airflow-providers-smtp-1.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/PKG-INFO` & `apache-airflow-providers-smtp-1.1.0rc2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.1.0rc1``
+Release: ``1.1.0rc2``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
@@ -123,14 +123,17 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/README.rst` & `apache-airflow-providers-smtp-1.1.0rc2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.1.0rc1``
+Release: ``1.1.0rc2``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
@@ -90,14 +90,17 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/get_provider_info.py` & `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/__init__.py` & `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/hooks/smtp.py` & `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/hooks/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/__init__.py` & `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/airflow/providers/smtp/operators/smtp.py` & `apache-airflow-providers-smtp-1.1.0rc2/airflow/providers/smtp/operators/smtp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/PKG-INFO` & `apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-smtp
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-smtp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-smtp/1.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-smtp``
 
-Release: ``1.1.0rc1``
+Release: ``1.1.0rc2``
 
 
 `Simple Mail Transfer Protocol (SMTP) <https://tools.ietf.org/html/rfc5321>`__
 
 
 Provider package
 ----------------
@@ -123,14 +123,17 @@
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add full automation for min Airflow version for providers (#30994)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 1.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/apache_airflow_providers_smtp.egg-info/SOURCES.txt` & `apache-airflow-providers-smtp-1.1.0rc2/apache_airflow_providers_smtp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/pyproject.toml` & `apache-airflow-providers-smtp-1.1.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/setup.cfg` & `apache-airflow-providers-smtp-1.1.0rc2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.smtp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.smtp
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-smtp-1.1.0rc1/setup.py` & `apache-airflow-providers-smtp-1.1.0rc2/setup.py`

 * *Files identical despite different names*

