# Comparing `tmp/dctrackclient-0.5.0.tar.gz` & `tmp/dctrackclient-0.5.1.tar.gz`

## Comparing `dctrackclient-0.5.0.tar` & `dctrackclient-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.5.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.5.0/.gitignore
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 dctrackclient-0.5.0/../README.md
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 dctrackclient-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 dctrackclient-0.5.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 dctrackclient-0.5.1/.gitignore
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 dctrackclient-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 dctrackclient-0.5.1/../README.md
+-rw-r--r--   0        0        0    12648 2020-02-02 00:00:00.000000 dctrackclient-0.5.1/PKG-INFO
```

### Comparing `dctrackclient-0.5.0/src/dcTrackClient/__init__.py` & `dctrackclient-0.5.1/src/dcTrackClient/__init__.py`

 * *Files identical despite different names*

### Comparing `dctrackclient-0.5.0/pyproject.toml` & `dctrackclient-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-0.5.0/../README.md` & `dctrackclient-0.5.1/../README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 ## Installation
 
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 
 ```shell
-pip install dcTrackClient==0.5.0
+pip install dcTrackClient==0.5.1
 ```
 
 ### JavaScript
 
 ```shell
-npm i dctrackclient@0.5.0
+npm i dctrackclient@0.5.1
 ```
 
 ## Initialize a connection to the dcTrack API
 
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
@@ -42,55 +42,151 @@
 const api = new Client('https://dctrack.example.com/', { username: 'user', password: 'pass' });
 // Using an API token //
 const api = new Client('https://dctrack.example.com/', { apiToken: 'token' });
 ```
 
 ## Usage Example
 
-> This section is currently under construction.
+> This section demonstrates item manipulation with the API client.
 
-### Create an item:
+### Create an item
 
-- This example shows the minimum attributes required to create an item
-- See [the official documentation](#official-dctrack-documentation) for a comprehensive list of attributes
-- This function returns the JSON object for the newly created item
-- If it fails, the function will return a JSON object containing the error message
+> This example shows the minimum attributes required to create an item using the [`createItem`](#createitemreturndetails-payload) function. View the comprehensive list of item attributes in the [official documentation](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/REST_API_JSON_Objects_for_Managed_Items.htm). Make sure to capture the return value of this function to see the created item details, such as the unique numeric item ID, or to determine if an error occurred while creating an item.
 
+#### Python
 ```py
-api.createItem({'cmbLocation': 'SAMPLE LOCATION', 'tiName': 'NEW-ITEM', 'cmbMake': 'Generic', 'cmbModel': 'Generic^Rackable^01'})
+response = api.createItem(True/False, {
+    'cmbLocation': 'item location',
+    'tiName': 'item name',
+    'cmbMake': 'item make',
+    'cmbModel': 'item model'
+})
+print(response)
 ```
 
-### Retrieve item details:
+#### JavaScript
+Notice the `await` keyword before the function call. This is because the JavaScript library is asynchronous and returns a `Promise` to the return value. All the API calls in this library require that keyword.
+```js
+let response = await api.createItem(true/false, {
+    'cmbLocation': 'item location',
+    'tiName': 'item name',
+    'cmbMake': 'item make',
+    'cmbModel': 'item model'
+});
+console.log(response);
+```
+
+#### On Success
+This function returns the JSON object for the newly created item. This is an example response if `returnDetails` was set to false.
+```json
+{ "item": { "id": 1234, "tiName": "item" } }
+```
+
+#### On Failure
+This function returns a JSON object containing the error message.
 
+### Retrieve item details
+> This example shows the usage of the [`getItem`](#getitemid) function.
+
+#### Python
 ```py
-item = api.getItem(1234)
+response = api.getItem(1234)
 ```
 
-Returns:
+#### JavaScript
+```js
+let response = await api.getItem(1234);
+```
 
+#### Returns
 ```json
 {
     "item": {
-        ... // item attributes in here
+        "cmbLocation": "item location",
+        "tiName": "item name",
+        ...
     }
 }
 ```
 
-### Modify an existing item:
+### Modify an existing item
+> This example shows the usage of the [`updateItem`](#updateitemid-returndetails-payload) function. Any number of attributes can be included in the payload to be modified.
 
+#### Python
 ```py
-api.modifyItem(1234, {'tiSerialNumber': 'SN-12345', 'tiAssetTag': 'DEV-12345'})
+response = api.updateItem(976, False, {'tiSerialNumber': 12345})
+```
+
+#### JavaScript
+```js
+let response = await api.updateItem(977, false, { 'tiSerialNumber': 12345 });
 ```
 
-### Delete an existing item:
+### Search for an item
+> This example demonstrates usage of the [`searchItems`](#searchitemspagenumber-pagesize-payload) function. Follow [this guide](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/v2_Advanced_Search_API.htm) for details on creating the request payload.
 
+#### Python
+```py
+response = api.searchItems(0, 0, {
+    'columns': [
+        {'name': 'tiName', 'filter': {'eq': 'item name'}}
+    ],
+    'selectedColumns': [
+        {'name': 'id'},
+        {'name': 'tiName'},
+    ]
+})
+```
+
+#### JavaScript
+```js
+let response = await api.searchItems(0, 0, {
+    'columns': [
+        { 'name': 'tiName', 'filter': { 'eq': 'item name' } }
+    ],
+    'selectedColumns': [
+        { 'name': 'id' },
+        { 'name': 'tiName' },
+    ]
+});
+```
+
+#### Returns
+```json
+{
+    "selectedColumns": [],
+    "totalRows": 1,
+    "pageNumber": 0,
+    "pageSize": 0,
+    "searchResults": {
+        "items": [
+            {"id": "1234", "tiName": "item name"}
+        ]
+    }
+}
+```
+
+### Delete an item
+> This example demonstrates usage of the [`deleteItem`](#deleteitemid) function.
+
+#### Python
 ```py
 api.deleteItem(1234)
 ```
 
+#### JavaScript
+```js
+await api.deleteItem(1234);
+```
+
+#### Returns
+```json
+{ "itemId": 1234 }
+```
+
 ## Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
 https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm
 
 ## getItem(id)
```

### Comparing `dctrackclient-0.5.0/PKG-INFO` & `dctrackclient-0.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcTrackClient
-Version: 0.5.0
+Version: 0.5.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -23,21 +23,21 @@
 ## Installation
 
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 
 ```shell
-pip install dcTrackClient==0.5.0
+pip install dcTrackClient==0.5.1
 ```
 
 ### JavaScript
 
 ```shell
-npm i dctrackclient@0.5.0
+npm i dctrackclient@0.5.1
 ```
 
 ## Initialize a connection to the dcTrack API
 
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
@@ -58,55 +58,151 @@
 const api = new Client('https://dctrack.example.com/', { username: 'user', password: 'pass' });
 // Using an API token //
 const api = new Client('https://dctrack.example.com/', { apiToken: 'token' });
 ```
 
 ## Usage Example
 
-> This section is currently under construction.
+> This section demonstrates item manipulation with the API client.
 
-### Create an item:
+### Create an item
 
-- This example shows the minimum attributes required to create an item
-- See [the official documentation](#official-dctrack-documentation) for a comprehensive list of attributes
-- This function returns the JSON object for the newly created item
-- If it fails, the function will return a JSON object containing the error message
+> This example shows the minimum attributes required to create an item using the [`createItem`](#createitemreturndetails-payload) function. View the comprehensive list of item attributes in the [official documentation](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/REST_API_JSON_Objects_for_Managed_Items.htm). Make sure to capture the return value of this function to see the created item details, such as the unique numeric item ID, or to determine if an error occurred while creating an item.
 
+#### Python
 ```py
-api.createItem({'cmbLocation': 'SAMPLE LOCATION', 'tiName': 'NEW-ITEM', 'cmbMake': 'Generic', 'cmbModel': 'Generic^Rackable^01'})
+response = api.createItem(True/False, {
+    'cmbLocation': 'item location',
+    'tiName': 'item name',
+    'cmbMake': 'item make',
+    'cmbModel': 'item model'
+})
+print(response)
 ```
 
-### Retrieve item details:
+#### JavaScript
+Notice the `await` keyword before the function call. This is because the JavaScript library is asynchronous and returns a `Promise` to the return value. All the API calls in this library require that keyword.
+```js
+let response = await api.createItem(true/false, {
+    'cmbLocation': 'item location',
+    'tiName': 'item name',
+    'cmbMake': 'item make',
+    'cmbModel': 'item model'
+});
+console.log(response);
+```
+
+#### On Success
+This function returns the JSON object for the newly created item. This is an example response if `returnDetails` was set to false.
+```json
+{ "item": { "id": 1234, "tiName": "item" } }
+```
+
+#### On Failure
+This function returns a JSON object containing the error message.
 
+### Retrieve item details
+> This example shows the usage of the [`getItem`](#getitemid) function.
+
+#### Python
 ```py
-item = api.getItem(1234)
+response = api.getItem(1234)
 ```
 
-Returns:
+#### JavaScript
+```js
+let response = await api.getItem(1234);
+```
 
+#### Returns
 ```json
 {
     "item": {
-        ... // item attributes in here
+        "cmbLocation": "item location",
+        "tiName": "item name",
+        ...
     }
 }
 ```
 
-### Modify an existing item:
+### Modify an existing item
+> This example shows the usage of the [`updateItem`](#updateitemid-returndetails-payload) function. Any number of attributes can be included in the payload to be modified.
 
+#### Python
 ```py
-api.modifyItem(1234, {'tiSerialNumber': 'SN-12345', 'tiAssetTag': 'DEV-12345'})
+response = api.updateItem(976, False, {'tiSerialNumber': 12345})
+```
+
+#### JavaScript
+```js
+let response = await api.updateItem(977, false, { 'tiSerialNumber': 12345 });
 ```
 
-### Delete an existing item:
+### Search for an item
+> This example demonstrates usage of the [`searchItems`](#searchitemspagenumber-pagesize-payload) function. Follow [this guide](https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm#APIGuide/v2_Advanced_Search_API.htm) for details on creating the request payload.
 
+#### Python
+```py
+response = api.searchItems(0, 0, {
+    'columns': [
+        {'name': 'tiName', 'filter': {'eq': 'item name'}}
+    ],
+    'selectedColumns': [
+        {'name': 'id'},
+        {'name': 'tiName'},
+    ]
+})
+```
+
+#### JavaScript
+```js
+let response = await api.searchItems(0, 0, {
+    'columns': [
+        { 'name': 'tiName', 'filter': { 'eq': 'item name' } }
+    ],
+    'selectedColumns': [
+        { 'name': 'id' },
+        { 'name': 'tiName' },
+    ]
+});
+```
+
+#### Returns
+```json
+{
+    "selectedColumns": [],
+    "totalRows": 1,
+    "pageNumber": 0,
+    "pageSize": 0,
+    "searchResults": {
+        "items": [
+            {"id": "1234", "tiName": "item name"}
+        ]
+    }
+}
+```
+
+### Delete an item
+> This example demonstrates usage of the [`deleteItem`](#deleteitemid) function.
+
+#### Python
 ```py
 api.deleteItem(1234)
 ```
 
+#### JavaScript
+```js
+await api.deleteItem(1234);
+```
+
+#### Returns
+```json
+{ "itemId": 1234 }
+```
+
 ## Official DcTrack Documentation
 
 Visit this link for the official documentation on request bodies and attrribute names.
 
 https://www.sunbirddcim.com/help/dcTrack/v900/API/en/Default.htm
 
 ## getItem(id)
```

