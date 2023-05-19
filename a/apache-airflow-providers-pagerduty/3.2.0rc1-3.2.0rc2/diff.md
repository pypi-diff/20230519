# Comparing `tmp/apache-airflow-providers-pagerduty-3.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-pagerduty-3.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-pagerduty-3.2.0rc1.tar", last modified: Tue May 16 15:54:51 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-pagerduty-3.2.0rc2.tar", last modified: Fri May 19 17:53:09 2023, max compression
```

## Comparing `apache-airflow-providers-pagerduty-3.2.0rc1.tar` & `apache-airflow-providers-pagerduty-3.2.0rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9607 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8071 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/
--rw-r--r--   0 root         (0) root         (0)     1392 2023-05-16 15:39:21.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2587 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6921 2023-05-03 19:47:07.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py
--rw-r--r--   0 root         (0) root         (0)     6276 2023-05-12 08:38:07.000000 apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9607 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      714 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-15 09:39:26.000000 apache-airflow-providers-pagerduty-3.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1862 2023-05-16 15:54:51.000000 apache-airflow-providers-pagerduty-3.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1656 2023-05-16 15:54:50.000000 apache-airflow-providers-pagerduty-3.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-pagerduty-3.2.0rc2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8493 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-05-19 12:18:55.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-02-24 18:43:53.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2023-05-18 08:56:29.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py
+-rw-r--r--   0 root         (0) root         (0)     8326 2023-05-19 11:18:18.000000 apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      714 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-pagerduty-3.2.0rc2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-05-19 17:53:09.000000 apache-airflow-providers-pagerduty-3.2.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-19 17:53:08.000000 apache-airflow-providers-pagerduty-3.2.0rc2/setup.py
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/LICENSE` & `apache-airflow-providers-pagerduty-3.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/MANIFEST.in` & `apache-airflow-providers-pagerduty-3.2.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/PKG-INFO` & `apache-airflow-providers-pagerduty-3.2.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
@@ -116,25 +116,35 @@
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
+Features
+~~~~~~~~
+
+* ``Add test_connection method to PagerdutyHook (#31344)``
+* ``Add test_connection method to PagerdutyEventsHook (#31346)``
+* ``Add Change event V2 API support for pagerduty (#31222)``
+
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 * `` Fixed typo in 'PagerdutyEventsHook' docstring (#31209)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/README.rst` & `apache-airflow-providers-pagerduty-3.2.0rc2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
@@ -83,25 +83,35 @@
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
+Features
+~~~~~~~~
+
+* ``Add test_connection method to PagerdutyHook (#31344)``
+* ``Add test_connection method to PagerdutyEventsHook (#31346)``
+* ``Add Change event V2 API support for pagerduty (#31222)``
+
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 * `` Fixed typo in 'PagerdutyEventsHook' docstring (#31209)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/__init__.py` & `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/__init__.py`

 * *Files 13% similar despite different names*

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
-        f"The package `apache-airflow-providers-pagerduty:{version}` requires Apache Airflow 2.4.0+"
+        f"The package `apache-airflow-providers-pagerduty:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/get_provider_info.py` & `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/__init__.py` & `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py` & `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,7 +155,15 @@
             custom_details=custom_details,
             group=group,
             component=component,
             class_type=class_type,
             images=images,
             links=links,
         )
+
+    def test_connection(self):
+        try:
+            session = pdpyras.APISession(self.token)
+            session.list_all("services", params={"query": "some_non_existing_service"})
+        except Exception:
+            return False, "connection test failed, invalid token"
+        return True, "connection tested successfully"
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py` & `apache-airflow-providers-pagerduty-3.2.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Hook for sending or receiving data from PagerDuty as well as creating PagerDuty incidents."""
 from __future__ import annotations
 
+from datetime import datetime
 from typing import Any
 
 import pdpyras
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 
@@ -147,7 +148,57 @@
         if links is not None:
             data["links"] = links
 
         session = pdpyras.EventsAPISession(self.integration_key)
         resp = session.post("/v2/enqueue", json=data)
         resp.raise_for_status()
         return resp.json()
+
+    def create_change_event(
+        self,
+        summary: str,
+        source: str = "airflow",
+        custom_details: Any | None = None,
+        timestamp: datetime | None = None,
+        links: list[Any] | None = None,
+    ) -> dict:
+        """
+        Create change event for service integration.
+
+        :param summary: Summary for the event
+        :param source: Specific human-readable unique identifier, such as a
+            hostname, for the system having the problem.
+        :param custom_details: Free-form details from the event. Can be a dictionary or a string.
+            If a dictionary is passed it will show up in PagerDuty as a table.
+        :param timestamp: The time at which the emitting tool detected or generated the event.
+        :param links: List of links to include. Each dictionary in the list accepts the following keys:
+            `href`: URL of the link to be attached.
+            `text`: [Optional] Plain text that describes the purpose of the link, and can be used as the
+            link's text.
+        :return: PagerDuty Change Events API v2 response.
+        """
+        payload = {
+            "summary": summary,
+        }
+        if custom_details is not None:
+            payload["custom_details"] = custom_details
+
+        if timestamp is not None:
+            payload["timestamp"] = timestamp.isoformat()
+
+        if source is not None:
+            payload["source"] = source
+
+        data: dict[str, Any] = {"payload": payload}
+        if links is not None:
+            data["links"] = links
+
+        session = pdpyras.ChangeEventsAPISession(self.integration_key)
+        return session.send_change_event(payload=payload, links=links)
+
+    def test_connection(self):
+        try:
+            session = pdpyras.EventsAPISession(self.integration_key)
+            session.resolve("some_dedup_key_that_dont_exist")
+        except Exception:
+            return False, "connection test failed, invalid routing key"
+        return True, "connection tested successfully"
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO` & `apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.2.0rc1
+Version: 3.2.0rc2
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.2.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.2.0rc1``
+Release: ``3.2.0rc2``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
@@ -116,25 +116,35 @@
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
 
+Features
+~~~~~~~~
+
+* ``Add test_connection method to PagerdutyHook (#31344)``
+* ``Add test_connection method to PagerdutyEventsHook (#31346)``
+* ``Add Change event V2 API support for pagerduty (#31222)``
+
 Misc
 ~~~~
 
 * ``Bump minimum Airflow version in providers (#30917)``
 * `` Fixed typo in 'PagerdutyEventsHook' docstring (#31209)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Use 'AirflowProviderDeprecationWarning' in providers (#30975)``
    * ``Add full automation for min Airflow version for providers (#30994)``
    * ``Add mechanism to suspend providers (#30422)``
+   * ``Use '__version__' in providers not 'version' (#31393)``
+   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
+   * ``Prepare docs for May 2023 wave of Providers (#31252)``
 
 3.1.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.3+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt` & `apache-airflow-providers-pagerduty-3.2.0rc2/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/pyproject.toml` & `apache-airflow-providers-pagerduty-3.2.0rc2/pyproject.toml`

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

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/setup.cfg` & `apache-airflow-providers-pagerduty-3.2.0rc2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.pagerduty.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.pagerduty
 
 [egg_info]
-tag_build = rc1
+tag_build = rc2
 tag_date = 0
```

### Comparing `apache-airflow-providers-pagerduty-3.2.0rc1/setup.py` & `apache-airflow-providers-pagerduty-3.2.0rc2/setup.py`

 * *Files identical despite different names*

