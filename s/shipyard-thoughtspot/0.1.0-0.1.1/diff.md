# Comparing `tmp/shipyard_thoughtspot-0.1.0.tar.gz` & `tmp/shipyard_thoughtspot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_thoughtspot-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_thoughtspot-0.1.1.tar", max compression
```

## Comparing `shipyard_thoughtspot-0.1.0.tar` & `shipyard_thoughtspot-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-19 03:19:02.295281 shipyard_thoughtspot-0.1.0/README.md
--rw-r--r--   0        0        0      500 2023-05-19 03:19:02.296020 shipyard_thoughtspot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       43 2023-05-19 03:19:02.296300 shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/__init__.py
--rw-r--r--   0        0        0     1748 2023-05-19 03:19:02.296695 shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/export_answer.py
--rw-r--r--   0        0        0     1677 2023-05-19 03:19:02.296946 shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/export_live_report.py
--rw-r--r--   0        0        0     1578 2023-05-19 03:19:02.297115 shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/export_metadata.py
--rw-r--r--   0        0        0     1355 2023-05-19 03:19:02.297313 shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/search_data.py
--rw-r--r--   0        0        0     6596 2023-05-19 03:19:02.297648 shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/thoughtspot.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 shipyard_thoughtspot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 03:19:02.295281 shipyard_thoughtspot-0.1.1/README.md
+-rw-r--r--   0        0        0      500 2023-05-19 17:12:04.286137 shipyard_thoughtspot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-05-19 03:19:02.296300 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/__init__.py
+-rw-r--r--   0        0        0     1719 2023-05-19 16:17:34.706546 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_answer.py
+-rw-r--r--   0        0        0     1648 2023-05-19 15:14:36.178587 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_live_report.py
+-rw-r--r--   0        0        0     1578 2023-05-19 03:19:02.297115 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_metadata.py
+-rw-r--r--   0        0        0     1314 2023-05-19 16:17:44.561544 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/search_data.py
+-rw-r--r--   0        0        0     8125 2023-05-19 17:01:44.064857 shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/thoughtspot.py
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 shipyard_thoughtspot-0.1.1/PKG-INFO
```

### Comparing `shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/export_answer.py` & `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_answer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     args = parser.parse_args()
     return args
 
 
 def main():
     args = get_args()
     args_dict = {
-        "token": args.token,
         "metadata_identifier": args.metadata_identifier,
         "file_format": args.file_format,
         "runtime_filter": None if args.runtime_filter == "" else args.runtime_filter,
         "runtime_sort": None if args.runtime_sort == "" else args.runtime_sort,
         "file_name": args.file_name,
     }
     client = ThoughtSpotClient(token=args.token)
```

### Comparing `shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/export_live_report.py` & `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_live_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     args = parser.parse_args()
     return args
 
 
 def main():
     args = get_args()
     args_dict = {
-        "token": args.token,
         "metadata_identifier": args.metadata_identifier,
         "file_format": args.file_format,
         "runtime_filter": None if args.runtime_filter == "" else args.runtime_filter,
         "runtime_sort": None if args.runtime_sort == "" else args.runtime_sort,
         "file_name": args.file_name,
     }
     client = ThoughtSpotClient(token=args.token)
```

### Comparing `shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/export_metadata.py` & `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/export_metadata.py`

 * *Files identical despite different names*

### Comparing `shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/cli/search_data.py` & `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/cli/search_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import argparse
 from shipyard_thoughtspot import ThoughtSpotClient
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--token", dest="token", required=True)
-    parser.add_argument('--query', dest = 'query', required = True)
-    parser.add_argument('--table-id', dest = 'table_id', required = True)
-    parser.add_argument('--num-rows', dest = 'num_rows', default = '', required = False)
-    parser.add_argument('--file-name', dest = 'file_name', default = 'search_data.csv', required = False)
+    parser.add_argument("--query", dest="query", required=True)
+    parser.add_argument("--table-id", dest="table_id", required=True)
+    parser.add_argument("--num-rows", dest="num_rows", default="", required=False)
+    parser.add_argument(
+        "--file-name", dest="file_name", default="search_data.csv", required=False
+    )
     args = parser.parse_args()
     return args
 
 
 def main():
     args = get_args()
     args_dict = {
-        "token": args.token,
-        "query" : args.query,
-        'table_identifier': args.table_id,
-        'num_rows' : None if args.num_rows == '' else args.num_rows,
+        "query": args.query,
+        "table_identifier": args.table_id,
+        "num_rows": None if args.num_rows == "" else args.num_rows,
     }
     file_name = args.file_name
     client = ThoughtSpotClient(token=args.token)
     try:
         client.logger.info(f"Attempting to export search results")
-        data = client.search_data(**args_dict, file_format = 'csv')
+        data = client.search_data(**args_dict, file_format="csv")
         client.logger.info(f"Writing file to {file_name}")
-        data.to_csv(file_name, index = False)
+        data.to_csv(file_name, index=False)
     except Exception as e:
         client.logger.error("There was an error in exporting the query results")
         client.logger.error(e)
         return client.EXIT_CODE_BAD_REQUEST
 
 
 if __name__ == "__main__":
```

### Comparing `shipyard_thoughtspot-0.1.0/shipyard_thoughtspot/thoughtspot.py` & `shipyard_thoughtspot-0.1.1/shipyard_thoughtspot/thoughtspot.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 import pandas as pd
 import typing
 import sys
 
 from copy import deepcopy
 from shipyard_templates import DataVisualization
 from requests import Response
+from ast import literal_eval
 
 
 class ThoughtSpotClient(DataVisualization):
     EXIT_CODE_LIVE_REPORT_ERROR = 200
     EXIT_CODE_ANSWER_REPORT_ERROR = 201
     EXIT_CODE_BAD_REQUEST = 202
+    EXIT_CODE_INVALID_FILTER = 203
+    EXIT_CODE_INVALID_SORT = 204
 
     def __init__(self, token) -> None:
         self.token = token
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.token}",
         }
@@ -23,52 +26,67 @@
 
     def get_live_report(
         self,
         metadata_identifier: str,
         visualization_identifiers: list = None,
         file_format: str = "csv",
         file_name: str = "liveboard",
-        runtime_filter: str = None,
-        runtime_sort: str = None,
+        runtime_filter: dict = None,
+        runtime_sort: dict = None,
     ) -> Response:
         """
 
         Args:
             metadata_identifier: the id of the associated metadata
             visualization_identifiers: a list of associated visualizations to include. If left blank, then all will be included
             file_format: Option of csv, png, pdf, or xlsx
-            runtime_filter: A column condition to filter the data
-            runtime_sort:  A column sort to sort the output
+            runtime_filter: A column condition to filter the data. Example: {"col1": "column_name", "operator": "EQ", "val1": 2}
+            runtime_sort:  A column sort to sort the output. Example: {"col1": "column_name", "asc1" : "true", "col2": "column_name", "asc2": "false"}
             file_name: The name of the output file
         """
         url = "https://my2.thoughtspot.cloud/api/rest/2.0/report/liveboard"
         payload = {
             "metadata_identifier": metadata_identifier,
             "file_format": str(file_format).upper(),
         }
         if runtime_filter:
             self.logger.info(f"Applying specified filter {runtime_filter}")
-            payload["runtime_filter"] = runtime_filter
+            try:
+                filt = literal_eval(runtime_filter)
+                payload["runtime_filter"] = filt
+            except Exception as e:
+                self.logger.error(f"Could not parse filter {runtime_filter}")
+                return self.EXIT_CODE_INVALID_FILTER
         if runtime_sort:
             self.logger.info(f"Applying specified sort {runtime_sort}")
-            payload["runtime_sort"] = runtime_sort
+            try:
+                sorter = literal_eval(runtime_sort)
+                payload["runtime_sort"] = sorter
+            except Exception as e:
+                self.logger.error(f"Could not parse sort {runtime_sort}")
+                return self.EXIT_CODE_INVALID_SORT
         if visualization_identifiers:
             self.logger.info(
                 f"Apply specified visualizations {visualization_identifiers}"
             )
             payload["visualization_identifiers"] = visualization_identifiers
         file_path = f"{file_name}.{file_format}"
         response = requests.post(url, headers=self.headers, json=payload)
         if response.status_code != 200:
             self.logger.error(
                 f"There was an error in the request. Message from the API is: {response.json()}"
             )
+            return self.EXIT_CODE_LIVE_REPORT_ERROR
         with open(file_path, "wb") as f:
             f.write(response.content)
             f.close()
+
+        if file_format == "csv":
+            df_cleaned = pd.read_csv(file_path, skiprows=4)
+            df_cleaned.to_csv(file_path, index=False)
         self.logger.info(f"Live report saved to {file_path}")
         return response
 
     def get_answer_report(
         self,
         metadata_identifier: str,
         file_format: str = "csv",
@@ -77,32 +95,43 @@
         file_name: str = "export",
     ) -> Response:
         """
 
         Args:
             metadata_identifier: The id for the associated answer report
             file_format: The desired output file format (csv, png, pdf, xlsx)
-            runtime_filter: Column filter to be applied
-            runtime_sort:  Column sort to be applied
+            runtime_filter: A column condition to filter the data. Example: {"col1": "column_name", "operator": "EQ", "val1": 2}
+            runtime_sort:  A column sort to sort the output. Example: {"col1": "column_name", "asc1" : "true", "col2": "column_name", "asc2": "false"}
             file_name: Name of the exported file (default is export)
 
         Returns:  The HTTP response from the api call
 
         """
         url = "https://my2.thoughtspot.cloud/api/rest/2.0/report/answer"
         payload = {
             "metadata_identifier": metadata_identifier,
             "file_format": str(file_format).upper(),
         }
         if runtime_filter:
             self.logger.info(f"Applying specified filter {runtime_filter}")
-            payload["runtime_filter"] = runtime_filter
+            try:
+                filt = literal_eval(runtime_filter)
+                payload["runtime_filter"] = filt
+            except Exception as e:
+                self.logger.error(f"Invalid filter {runtime_filter}")
+                return self.EXIT_CODE_INVALID_FILTER
+
         if runtime_sort:
             self.logger.info(f"Applying specified sort {runtime_sort}")
-            payload["runtime_sort"] = runtime_sort
+            try:
+                sorter = literal_eval(runtime_sort)
+                payload["runtime_sort"] = sorter
+            except Exception as e:
+                self.logger.error(f"Could not parse sort {runtime_sort}")
+                return self.EXIT_CODE_INVALID_SORT
 
         file_path = f"{file_name}.{file_format}"
         response = requests.post(url, headers=self.headers, json=payload)
         if response.status_code != 200:
             self.logger.error(
                 f"There was an error in the request. Message from the API is: {response.json()}"
             )
```

### Comparing `shipyard_thoughtspot-0.1.0/PKG-INFO` & `shipyard_thoughtspot-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-thoughtspot
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

