# Comparing `tmp/shipyard_thoughtspot-0.1.1.tar.gz` & `tmp/shipyard_thoughtspot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_thoughtspot-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_thoughtspot-0.1.2.tar", max compression
```

## Comparing `shipyard_thoughtspot-0.1.1.tar` & `shipyard_thoughtspot-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-19 03:19:02.295281 shipyard_thoughtspot-0.1.1/README.md
--rw-r--r--   0        0        0      500 2023-05-19 17:12:04.286137 shipyard_thoughtspot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       43 2023-05-19 03:19:02.296300 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/__init__.py
--rw-r--r--   0        0        0     1719 2023-05-19 16:17:34.706546 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_answer.py
--rw-r--r--   0        0        0     1648 2023-05-19 15:14:36.178587 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_live_report.py
--rw-r--r--   0        0        0     1578 2023-05-19 03:19:02.297115 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_metadata.py
--rw-r--r--   0        0        0     1314 2023-05-19 16:17:44.561544 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/search_data.py
--rw-r--r--   0        0        0     8125 2023-05-19 17:01:44.064857 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/thoughtspot.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 shipyard_thoughtspot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 03:19:02.295281 shipyard_thoughtspot-0.1.2/README.md
+-rw-r--r--   0        0        0      500 2023-05-19 17:56:26.308524 shipyard_thoughtspot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-19 03:19:02.296300 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/__init__.py
+-rw-r--r--   0        0        0      475 2023-05-19 17:54:48.059667 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/authtest.py
+-rw-r--r--   0        0        0     1719 2023-05-19 16:17:34.706546 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/export_answer.py
+-rw-r--r--   0        0        0     1648 2023-05-19 15:14:36.178587 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/export_live_report.py
+-rw-r--r--   0        0        0     1578 2023-05-19 03:19:02.297115 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/export_metadata.py
+-rw-r--r--   0        0        0     1314 2023-05-19 16:17:44.561544 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/search_data.py
+-rw-r--r--   0        0        0     7946 2023-05-19 17:39:51.517910 shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/thoughtspot.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 shipyard_thoughtspot-0.1.2/PKG-INFO
```

### Comparing `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_answer.py` & `shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/export_answer.py`

 * *Files identical despite different names*

### Comparing `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_live_report.py` & `shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/export_live_report.py`

 * *Files identical despite different names*

### Comparing `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_metadata.py` & `shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/export_metadata.py`

 * *Files identical despite different names*

### Comparing `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/search_data.py` & `shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/cli/search_data.py`

 * *Files identical despite different names*

### Comparing `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/thoughtspot.py` & `shipyard_thoughtspot-0.1.2/shipyard_thoughtspot/thoughtspot.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,11 @@
             elif file_format == "json":
                 return response.json()
         else:
             self.logger.error("Error in fetching query results")
             self.logger.error(f"Response code is {response.status_code}")
             self.logger.error(f"Response from API is {response.json()}")
 
-    def connect(self, username: str, password: str):
-        url = "https://my2.thoughtspot.cloud/api/rest/2.0/auth/session/login"
-        headers = deepcopy(self.headers)
-        headers["Accept"] = "application/json"
-        payload = {"username": username, "password": password}
-        response = requests.post(url, headers=headers, json=payload)
+    def connect(self) -> Response:
+        url = "https://my2.thoughtspot.cloud/api/rest/2.0/auth/session/user"
+        response = requests.post(url, headers=self.headers)
         return response
```

### Comparing `shipyard_thoughtspot-0.1.1/PKG-INFO` & `shipyard_thoughtspot-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-thoughtspot
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

