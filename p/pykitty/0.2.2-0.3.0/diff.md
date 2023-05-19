# Comparing `tmp/pykitty-0.2.2.tar.gz` & `tmp/pykitty-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykitty-0.2.2.tar", max compression
+gzip compressed data, was "pykitty-0.3.0.tar", max compression
```

## Comparing `pykitty-0.2.2.tar` & `pykitty-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-07 13:19:00.028271 pykitty-0.2.2/LICENSE
--rw-r--r--   0        0        0     2195 2023-04-07 13:14:15.727476 pykitty-0.2.2/README.md
--rw-r--r--   0        0        0       34 2023-05-19 19:18:21.950507 pykitty-0.2.2/pykitty/__init__.py
--rw-r--r--   0        0        0     2943 2023-04-06 19:00:01.649008 pykitty-0.2.2/pykitty/cli.py
--rw-r--r--   0        0        0     6071 2023-04-07 10:29:06.231436 pykitty-0.2.2/pykitty/client.py
--rw-r--r--   0        0        0     3016 2023-04-07 10:29:06.231718 pykitty-0.2.2/pykitty/kitty_parser.py
--rw-r--r--   0        0        0      531 2023-05-19 19:19:50.306239 pykitty-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2838 1970-01-01 00:00:00.000000 pykitty-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-07 13:19:00.028271 pykitty-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2252 2023-05-19 20:50:57.649630 pykitty-0.3.0/README.md
+-rw-r--r--   0        0        0       34 2023-05-19 19:18:21.950507 pykitty-0.3.0/pykitty/__init__.py
+-rw-r--r--   0        0        0     2943 2023-04-06 19:00:01.649008 pykitty-0.3.0/pykitty/cli.py
+-rw-r--r--   0        0        0     7247 2023-05-19 20:56:11.028345 pykitty-0.3.0/pykitty/client.py
+-rw-r--r--   0        0        0     7460 2023-05-19 20:53:59.420086 pykitty-0.3.0/pykitty/kitty_parser.py
+-rw-r--r--   0        0        0      551 2023-05-19 20:57:24.226082 pykitty-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 pykitty-0.3.0/PKG-INFO
```

### Comparing `pykitty-0.2.2/LICENSE` & `pykitty-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykitty-0.2.2/README.md` & `pykitty-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -89,10 +89,12 @@
 
 This project is licensed under the MIT License.
 
 ## Next Steps (TODO)
 
 - [x] Parse Kitty URL to extract `kitty_id` 
 - [x] Implement `get_expenses` method to retrieve all expenses.
-- [ ] Add support for updating and deleting expenses.
+- [x] Add support for deleting expenses.
+- [ ] Enhance test coverage.
+- [ ] Add support for updating expenses.
 - [ ] Document CLI usage.
 - [ ] Support for Kittysplit in other languages.
```

### Comparing `pykitty-0.2.2/pykitty/cli.py` & `pykitty-0.3.0/pykitty/cli.py`

 * *Files identical despite different names*

### Comparing `pykitty-0.2.2/pykitty/client.py` & `pykitty-0.3.0/pykitty/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from datetime import datetime
 from typing import Dict, List, Union
-from urllib.parse import urlparse
+from urllib.parse import quote, urlparse
 
 import requests
 
 from pykitty import kitty_parser
 
 
+def fill_query_params(query, *args):
+    return query.format(*[quote(arg, safe="") for arg in args])
+
+
 def parse_kitty_id(kitty_url) -> str:
     kitty_url_parser = urlparse(kitty_url)
 
     if "kittysplit." not in kitty_url_parser.netloc:
         raise ValueError("Invalid Domain! Must be a kittysplit domain.")
 
     kitty_url_parts = kitty_url_parser.path.split(
@@ -111,15 +115,44 @@
             csrf_token=kwargs.pop("csrf_token"),
             data=form_data,
         )
 
     @kitty_endpoint("/entries/", user_needs_to_be_selected=True)
     def get_expenses(self, **kwargs) -> List[dict]:
         response = self._request(kwargs.pop("method"), kwargs.pop("path"))
-        return kitty_parser.parse_expenses(response.text)
+        expenses = kitty_parser.parse_expenses(response.text)
+
+        # add base url to detail expense pages
+        for expense in expenses:
+            detail_url = expense["url"]
+            if detail_url.startswith("/"):  # remove leading slash
+                detail_url = detail_url[1:]
+            expense["url"] = self.base_url + detail_url
+
+        return expenses
+
+    @kitty_endpoint("/entries/{}/edit", user_needs_to_be_selected=True)
+    def get_expense(self, entry_id: str, **kwargs) -> dict:
+        response = self._request(
+            kwargs.pop("method"), fill_query_params(kwargs.pop("path"), entry_id)
+        )
+
+        parsed_flat_expense_detail = kitty_parser.parse_expense(response.text)
+        return kitty_parser.parse_flat_expense_detail(parsed_flat_expense_detail)
+
+    @kitty_endpoint(
+        "/entries/{}/delete",
+        method="POST",
+        csrf_protected=True,
+        user_needs_to_be_selected=True,
+    )
+    def delete_expense(self, entry_id: str, **kwargs) -> None:
+        self._request(
+            kwargs.pop("method"), fill_query_params(kwargs.pop("path"), entry_id)
+        )
 
     @kitty_endpoint(
         "/entries/new/expense/",
         method="POST",
         csrf_protected=True,
         user_needs_to_be_selected=True,
     )
```

### Comparing `pykitty-0.2.2/pyproject.toml` & `pykitty-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykitty"
-version = "0.2.2"
+version = "0.3.0"
 description = "The unofficial Kittysplit wrapper for Python."
 authors = ["Lars Heinen"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.scripts]
 pykitty = "pykitty.cli:app"
@@ -14,11 +14,12 @@
 requests = "^2.28.2"
 typer = {extras = ["all"], version = "^0.7.0"}
 beautifulsoup4 = "^4.12.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
+coverage = "^7.2.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pykitty-0.2.2/PKG-INFO` & `pykitty-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykitty
-Version: 0.2.2
+Version: 0.3.0
 Summary: The unofficial Kittysplit wrapper for Python.
 License: MIT
 Author: Lars Heinen
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -107,11 +107,13 @@
 
 This project is licensed under the MIT License.
 
 ## Next Steps (TODO)
 
 - [x] Parse Kitty URL to extract `kitty_id` 
 - [x] Implement `get_expenses` method to retrieve all expenses.
-- [ ] Add support for updating and deleting expenses.
+- [x] Add support for deleting expenses.
+- [ ] Enhance test coverage.
+- [ ] Add support for updating expenses.
 - [ ] Document CLI usage.
 - [ ] Support for Kittysplit in other languages.
```

