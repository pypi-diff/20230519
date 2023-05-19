# Comparing `tmp/fastapi_react_admin-0.2.0.tar.gz` & `tmp/fastapi_react_admin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_react_admin-0.2.0.tar", max compression
+gzip compressed data, was "fastapi_react_admin-1.0.0.tar", max compression
```

## Comparing `fastapi_react_admin-0.2.0.tar` & `fastapi_react_admin-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       35 2023-05-17 17:29:31.844703 fastapi_react_admin-0.2.0/fastapi_react_admin/__init__.py
--rw-r--r--   0        0        0     6884 2023-05-18 12:57:54.202568 fastapi_react_admin-0.2.0/fastapi_react_admin/react_admin.py
--rw-r--r--   0        0        0      149 2023-05-18 08:55:36.202042 fastapi_react_admin-0.2.0/fastapi_react_admin/schemas.py
--rw-r--r--   0        0        0      426 2023-05-18 12:58:23.632828 fastapi_react_admin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4881 2023-05-18 12:57:58.670479 fastapi_react_admin-0.2.0/README.md
--rw-r--r--   0        0        0     5588 1970-01-01 00:00:00.000000 fastapi_react_admin-0.2.0/setup.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 fastapi_react_admin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2023-05-17 17:29:31.844703 fastapi_react_admin-1.0.0/fastapi_react_admin/__init__.py
+-rw-r--r--   0        0        0     7604 2023-05-19 07:29:15.122605 fastapi_react_admin-1.0.0/fastapi_react_admin/react_admin.py
+-rw-r--r--   0        0        0      149 2023-05-18 08:55:36.202042 fastapi_react_admin-1.0.0/fastapi_react_admin/schemas.py
+-rw-r--r--   0        0        0      426 2023-05-19 07:34:46.516088 fastapi_react_admin-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5059 2023-05-19 07:34:35.326366 fastapi_react_admin-1.0.0/README.md
+-rw-r--r--   0        0        0     5766 1970-01-01 00:00:00.000000 fastapi_react_admin-1.0.0/setup.py
+-rw-r--r--   0        0        0     5420 1970-01-01 00:00:00.000000 fastapi_react_admin-1.0.0/PKG-INFO
```

### Comparing `fastapi_react_admin-0.2.0/fastapi_react_admin/react_admin.py` & `fastapi_react_admin-1.0.0/fastapi_react_admin/react_admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,62 +10,84 @@
 
 class ReactAdmin:
     def __init__(self, 
         table: any,
         *,
         router: APIRouter,
         session: async_sessionmaker[AsyncSession],
-        depends: Sequence[Depends] = [],
-        prefix: str = '/ra',
         deleted_field: str = None,
         exclude_deleted: str = True,
         include_in_schema: bool = False,
     ) -> None:
         '''
         Initializes a ReactAdmin instance.
 
         Args:
             table: The SQLAlchemy model representing the database table.
             router: The APIRouter instance to mount the routes.
             session: The async_sessionmaker[AsyncSession] for the database session.
-            depends: The sequence of the dependencies
-            prefix: The URL prefix for the react admin routes.
             deleted_field: The name of the field of the table for mark deleted fields (like is_deleted) (optional).
             exclude_deleted: Whether to exclude deleted records (optional).
             include_in_schema: Whether to include the routes in the generated schema (optional).
         '''
         
         self.table = table
         self.user_router = router
         self.Session = session
-        self.depends = depends
         self.deleted_filed = deleted_field
         self.exclude_deleted = exclude_deleted
-
-        self._router = APIRouter(
-            prefix=prefix, 
-            tags=['React Admin routers'], 
-            include_in_schema=include_in_schema
-        )
+        self.include_in_schema = include_in_schema
     
-    def mount(self):
+    def mount(self,
+        depends: Sequence[Depends] = [],
+        prefix: str = '/ra',
+        tags: list[str] = ['RA routes'],
+        include_get_list: bool = True,
+        include_get_one: bool = True,
+        include_get_many: bool = True,
+        include_create: bool = True,
+        include_update: bool = True,
+        include_update_many: bool = True,
+        include_delete: bool = True,
+        include_delete_many: bool = True,
+    ):
         '''
         Mounts the routes to the user_router.
+
+        Args:  
+            depends: The sequence of the dependencies
+            prefix: The URL prefix for the react admin routes.
+            tags: The FastAPI tags.
+            include_*: The params to include/exclude specific route.
         '''
+
+        router = APIRouter(
+            prefix=prefix, 
+            tags=tags, 
+            include_in_schema=self.include_in_schema
+        )
         
-        self._router.add_api_route('/getList', self._get_list, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/getOne/{id}', self._get_one, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/getMany/{id}', self._get_many, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/create', self._create, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/update/{id}', self._update, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/updateMany', self._update_many, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/delete/{id}', self._delete, response_model=RaResponseModel, methods=['POST'])
-        self._router.add_api_route('/deleteMany', self._delete_many, response_model=RaResponseModel, methods=['POST'])
+        if include_get_list: 
+            router.add_api_route('/getList', self._get_list, response_model=RaResponseModel, methods=['POST'])
+        if include_get_one: 
+            router.add_api_route('/getOne/{id}', self._get_one, response_model=RaResponseModel, methods=['POST'])
+        if include_get_many: 
+            router.add_api_route('/getMany/{id}', self._get_many, response_model=RaResponseModel, methods=['POST'])
+        if include_create: 
+            router.add_api_route('/create', self._create, response_model=RaResponseModel, methods=['POST'])
+        if include_update: 
+            router.add_api_route('/update/{id}', self._update, response_model=RaResponseModel, methods=['POST'])
+        if include_update_many: 
+            router.add_api_route('/updateMany', self._update_many, response_model=RaResponseModel, methods=['POST'])
+        if include_delete: 
+            router.add_api_route('/delete/{id}', self._delete, response_model=RaResponseModel, methods=['POST'])
+        if include_delete_many: 
+            router.add_api_route('/deleteMany', self._delete_many, response_model=RaResponseModel, methods=['POST'])
 
-        self.user_router.include_router(self._router, dependencies=self.depends)
+        self.user_router.include_router(self._router, dependencies=depends)
 
     async def _get_list(self, 
         sort: Json = Query(), 
         filter: Json = Query(), 
         range_: Json = Query()
     ):  
         if self.deleted_filed and self.exclude_deleted:
```

### Comparing `fastapi_react_admin-0.2.0/README.md` & `fastapi_react_admin-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -118,24 +118,29 @@
 ### ReactAdmin class params
 - table (required): The SQLAlchemy model representing the database table.
 
 - router (required): The APIRouter instance to mount the routes.
 
 - session (required): The async_sessionmaker[AsyncSession] for the database session.
 
-- depends (optional): The sequence of the dependencies
-
-- prefix (optional): The URL prefix for the React Admin routes. Default is '/ra'.
-
 - deleted_field (optional): The name of the field of the table to mark deleted fields (e.g., 'is_deleted'). Default is None.
 
 - exclude_deleted (optional): Whether to exclude deleted records. Default is True.
 
 - include_in_schema (optional): Whether to include the routes in the generated schema. Default is False.
 
+### ReactAdmin mount params
+- depends (optional): The sequence of the dependencies
+
+- prefix (optional): The URL prefix for the React Admin routes. Default is '/ra'.
+
+- tags (optional): The FastAPI tags.
+
+- include_* (optional): The params to include/exclude specific route. (For example: include_create=false)
+
 ### Route Endpoints
 The following routes are automatically generated by the `ReactAdmin` class:
 
 - POST /ra/getList: Get a list of records from the table. Accepts JSON payload with sort, filter, and range parameters.
 - POST /ra/getOne/{id}: Get a single record by ID.
 - POST /ra/getMany/{id}: Get multiple records by ID. Accepts JSON payload with id parameter.
 - POST /ra/create: Create a new record. Accepts JSON payload with the record data.
```

### Comparing `fastapi_react_admin-0.2.0/setup.py` & `fastapi_react_admin-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['fastapi>=0.95.2,<0.96.0', 'sqlalchemy>=2.0.13,<3.0.0']
 
 setup_kwargs = {
     'name': 'fastapi-react-admin',
-    'version': '0.2.0',
+    'version': '1.0.0',
     'description': 'Module to automaticly generate fastapi routes for using react admin',
-    'long_description': '# FastAPI React Admin\n\nThis module provides a class ReactAdmin that allows for the automatic generation of routes for React Admin in a FastAPI application.\n\n## Installation\n```console\npip install fastapi-react-admin\n```\n\n## Base usage\n\nFatstAPI part: \n```python\nfrom fastapi import FastAPI\n\nfrom schemas import MyTableModel\nfrom fastapi_react_admin import ReactAdmin\n\napp = FastAPI()\nrouter = app.router\nSession = async_sessionmaker(AsyncSession)\n\nReactAdmin(\n    table=MyTableModel, \n    router=router, \n    session=Session\n).mount()\n```\n\nReact Admin data provider:\n```js\nexport const sendPost = async (resource: string, method: string, body?: any) => {\n    const response = await axios({\n        method: \'post\',\n        url: resource + "/ra" + method,\n        data: body,\n        headers: {\n            "Admin-Token": sessionStorage.getItem(\'token\')\n        }\n    })\n\n    return response.data\n}\n\nconst dataProvider: DataProvider = {\n    getList: (resource: string, params: any) => {\n        const { page, perPage } = params.pagination\n        const { field, order } = params.sort\n\n        const query = {\n            sort: JSON.stringify([field, order]),\n            range_: JSON.stringify([(page - 1) * perPage, page * perPage - 1]),\n            filter: JSON.stringify(params.filter),\n        }\n\n        return sendPost(resource, `/getList?${queryString.stringify(query)}`)\n    },\n\n    getOne: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/getOne/\' + params.id)\n    },\n\n    getMany: (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return sendPost(resource, `/getMany?${queryString.stringify(query)}`)\n    },\n\n    getManyReference: (resource: string, params: any): any => {\n        const { page, perPage } = params.pagination\n        const { field, order } = params.sort\n\n        const query = {\n            sort: JSON.stringify([field, order]),\n            range_: JSON.stringify([(page - 1) * perPage, page * perPage - 1]),\n            filter: JSON.stringify(params.filter),\n        }\n\n        return sendPost(params.target, `/getList?${queryString.stringify(query)}`)\n    },\n\n    create: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/create\', { \n            ...params.data\n        })\n    },\n\n    update: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/update/\' + params.id, params.data)\n    },\n\n    updateMany: async (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return await sendPost(resource, `/updateMany?${queryString.stringify(query)}`, params.data)\n    },\n\n    delete: (resource: string, params: any) => {\n        return sendPost(resource, \'/delete/\' + params.id)\n    },\n\n    deleteMany: (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return sendPost(resource, `/deleteMany?${queryString.stringify(query)}` )\n    },\n}\n\n```\n\n\n### ReactAdmin class params\n- table (required): The SQLAlchemy model representing the database table.\n\n- router (required): The APIRouter instance to mount the routes.\n\n- session (required): The async_sessionmaker[AsyncSession] for the database session.\n\n- depends (optional): The sequence of the dependencies\n\n- prefix (optional): The URL prefix for the React Admin routes. Default is \'/ra\'.\n\n- deleted_field (optional): The name of the field of the table to mark deleted fields (e.g., \'is_deleted\'). Default is None.\n\n- exclude_deleted (optional): Whether to exclude deleted records. Default is True.\n\n- include_in_schema (optional): Whether to include the routes in the generated schema. Default is False.\n\n### Route Endpoints\nThe following routes are automatically generated by the `ReactAdmin` class:\n\n- POST /ra/getList: Get a list of records from the table. Accepts JSON payload with sort, filter, and range parameters.\n- POST /ra/getOne/{id}: Get a single record by ID.\n- POST /ra/getMany/{id}: Get multiple records by ID. Accepts JSON payload with id parameter.\n- POST /ra/create: Create a new record. Accepts JSON payload with the record data.\n- POST /ra/update/{id}: Update a record by ID. Accepts JSON payload with the updated data.\n- POST /ra/updateMany: Update multiple records. Accepts JSON payload with id parameter and updated data.\n- POST /ra/delete/{id}: Delete a record by ID.\n- POST /ra/deleteMany: Delete multiple records. Accepts JSON payload with id parameter.\n\n### Response Format\nThe response format for all routes is a JSON object with a data field. The data field contains the response data.',
+    'long_description': '# FastAPI React Admin\n\nThis module provides a class ReactAdmin that allows for the automatic generation of routes for React Admin in a FastAPI application.\n\n## Installation\n```console\npip install fastapi-react-admin\n```\n\n## Base usage\n\nFatstAPI part: \n```python\nfrom fastapi import FastAPI\n\nfrom schemas import MyTableModel\nfrom fastapi_react_admin import ReactAdmin\n\napp = FastAPI()\nrouter = app.router\nSession = async_sessionmaker(AsyncSession)\n\nReactAdmin(\n    table=MyTableModel, \n    router=router, \n    session=Session\n).mount()\n```\n\nReact Admin data provider:\n```js\nexport const sendPost = async (resource: string, method: string, body?: any) => {\n    const response = await axios({\n        method: \'post\',\n        url: resource + "/ra" + method,\n        data: body,\n        headers: {\n            "Admin-Token": sessionStorage.getItem(\'token\')\n        }\n    })\n\n    return response.data\n}\n\nconst dataProvider: DataProvider = {\n    getList: (resource: string, params: any) => {\n        const { page, perPage } = params.pagination\n        const { field, order } = params.sort\n\n        const query = {\n            sort: JSON.stringify([field, order]),\n            range_: JSON.stringify([(page - 1) * perPage, page * perPage - 1]),\n            filter: JSON.stringify(params.filter),\n        }\n\n        return sendPost(resource, `/getList?${queryString.stringify(query)}`)\n    },\n\n    getOne: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/getOne/\' + params.id)\n    },\n\n    getMany: (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return sendPost(resource, `/getMany?${queryString.stringify(query)}`)\n    },\n\n    getManyReference: (resource: string, params: any): any => {\n        const { page, perPage } = params.pagination\n        const { field, order } = params.sort\n\n        const query = {\n            sort: JSON.stringify([field, order]),\n            range_: JSON.stringify([(page - 1) * perPage, page * perPage - 1]),\n            filter: JSON.stringify(params.filter),\n        }\n\n        return sendPost(params.target, `/getList?${queryString.stringify(query)}`)\n    },\n\n    create: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/create\', { \n            ...params.data\n        })\n    },\n\n    update: async (resource: string, params: any) => {\n        return await sendPost(resource, \'/update/\' + params.id, params.data)\n    },\n\n    updateMany: async (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return await sendPost(resource, `/updateMany?${queryString.stringify(query)}`, params.data)\n    },\n\n    delete: (resource: string, params: any) => {\n        return sendPost(resource, \'/delete/\' + params.id)\n    },\n\n    deleteMany: (resource: string, params: any) => {\n        const query = {\n            filter: JSON.stringify({ id: params.ids}),\n        }\n\n        return sendPost(resource, `/deleteMany?${queryString.stringify(query)}` )\n    },\n}\n\n```\n\n\n### ReactAdmin class params\n- table (required): The SQLAlchemy model representing the database table.\n\n- router (required): The APIRouter instance to mount the routes.\n\n- session (required): The async_sessionmaker[AsyncSession] for the database session.\n\n- deleted_field (optional): The name of the field of the table to mark deleted fields (e.g., \'is_deleted\'). Default is None.\n\n- exclude_deleted (optional): Whether to exclude deleted records. Default is True.\n\n- include_in_schema (optional): Whether to include the routes in the generated schema. Default is False.\n\n### ReactAdmin mount params\n- depends (optional): The sequence of the dependencies\n\n- prefix (optional): The URL prefix for the React Admin routes. Default is \'/ra\'.\n\n- tags (optional): The FastAPI tags.\n\n- include_* (optional): The params to include/exclude specific route. (For example: include_create=false)\n\n### Route Endpoints\nThe following routes are automatically generated by the `ReactAdmin` class:\n\n- POST /ra/getList: Get a list of records from the table. Accepts JSON payload with sort, filter, and range parameters.\n- POST /ra/getOne/{id}: Get a single record by ID.\n- POST /ra/getMany/{id}: Get multiple records by ID. Accepts JSON payload with id parameter.\n- POST /ra/create: Create a new record. Accepts JSON payload with the record data.\n- POST /ra/update/{id}: Update a record by ID. Accepts JSON payload with the updated data.\n- POST /ra/updateMany: Update multiple records. Accepts JSON payload with id parameter and updated data.\n- POST /ra/delete/{id}: Delete a record by ID.\n- POST /ra/deleteMany: Delete multiple records. Accepts JSON payload with id parameter.\n\n### Response Format\nThe response format for all routes is a JSON object with a data field. The data field contains the response data.',
     'author': 'Enveloss',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi_react_admin-0.2.0/PKG-INFO` & `fastapi_react_admin-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-react-admin
-Version: 0.2.0
+Version: 1.0.0
 Summary: Module to automaticly generate fastapi routes for using react admin
 Author: Enveloss
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -132,24 +132,29 @@
 ### ReactAdmin class params
 - table (required): The SQLAlchemy model representing the database table.
 
 - router (required): The APIRouter instance to mount the routes.
 
 - session (required): The async_sessionmaker[AsyncSession] for the database session.
 
-- depends (optional): The sequence of the dependencies
-
-- prefix (optional): The URL prefix for the React Admin routes. Default is '/ra'.
-
 - deleted_field (optional): The name of the field of the table to mark deleted fields (e.g., 'is_deleted'). Default is None.
 
 - exclude_deleted (optional): Whether to exclude deleted records. Default is True.
 
 - include_in_schema (optional): Whether to include the routes in the generated schema. Default is False.
 
+### ReactAdmin mount params
+- depends (optional): The sequence of the dependencies
+
+- prefix (optional): The URL prefix for the React Admin routes. Default is '/ra'.
+
+- tags (optional): The FastAPI tags.
+
+- include_* (optional): The params to include/exclude specific route. (For example: include_create=false)
+
 ### Route Endpoints
 The following routes are automatically generated by the `ReactAdmin` class:
 
 - POST /ra/getList: Get a list of records from the table. Accepts JSON payload with sort, filter, and range parameters.
 - POST /ra/getOne/{id}: Get a single record by ID.
 - POST /ra/getMany/{id}: Get multiple records by ID. Accepts JSON payload with id parameter.
 - POST /ra/create: Create a new record. Accepts JSON payload with the record data.
```

